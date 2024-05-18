---
layout: page
permalink: /blogs/femreg/index.html
title: femreg
---

## Fixed Effect Model

- A panel dataset contains observations on multiple entities $i$ at two or more points in time $t$
- Whether some observations are missing: balanced and unbalanced
- **Fixed effects is a method of controlling for all variables, whether they're observed or not, as long as they stay constant within some larger category**
- The idea of fixed effects is that by sweeping away all that variation between individuals
- In panel data, when $corr(\alpha_i, x_{it} \neq 0)$, we should use fixed effect model, otherwise we use random effect model
- The assumption of fixed effect is everyone has a different intercept, and the individual's impacts is the same within the group; while the random effect assume everyone has the same intercept representing the random differences between individuals

### Estimators

- A standard regression equation is:
  - $y_{it} = \beta_i + \beta_1 X_{it} + \epsilon_{it}$
  - fixed effects: relative to others represented by intercept
  - The equation can be written equivalently as: $Y_{it} = \beta_0 + \beta_1 X_{it} + \gamma_2 D2_i + \gamma_3 D3_i + ... + \gamma_n Dn_i + \mu_{it}$
- To estimate a regression with individual intercepts:
  - $Y_{it} - \overline{Y_i} = \beta_0 + \beta_1 (X_{it} - \overline{X_i})+ \epsilon_{it}$
- Two-way fixed effects model
  - $Y_{it} = \beta_i + \beta_t + \beta_1 X_{it} + \epsilon_{it}$
  - We are looking at variation within individual as well as within year at this point

### Test
 
- Hausman
```Stata
xtreg invest mvalue kstock,fe
est store fe_result
xtreg invest mvalue kstock,re
est store re_result
hausman fe_result re_result
```
- Serial correlation test and Heteroskedasticity test
```Stata
xtserial invest mvalue kstock

xtreg invest mvalue kstock,fe
xttest3
```
- Robust Hausman
```Stata
webuse grunfeld, clear
xtset company year
quiet xtreg invest mvalue kstock,re
scalar theta = e(theta)
global xlist2 invest mvalue kstock
sort company
foreach x of varlist $xlist2 {
     by company: egen mean`x' = mean(`x')
     generate md`x' = `x' - mean`x'
     generate red`x' = `x' - theta*mean`x'
      }
quiet reg redinvest redmvalue redkstock mdmvalue mdkstock, vce(cluster company)
test mdmvalue mdkstock
```
- Corrected Hausman
```Stata
xtreg invest mvalue kstock,fe
est store fe_result
xtreg invest mvalue kstock,re
est store re_result
hausman fe_result re_result,sigmamore
```  
- Over-estimation Wald
```Stata
xtreg invest mvalue kstock, re cluster(company)
 xtoverid
```    
- Mundlak
 ```Stata
local xlist "mvalue kstock"
foreach f of local xlist{
  bysort company: egen mean_`f' = mean(`f')
}
xtreg invest mvalue kstock mean_mvalue mean_kstock, re vce(robust)
est store Mundlak_result

test mean_mvalue mean_kstock
```  
- Bootstrap Hausman
 ```Stata
xtreg invest mvalue kstock,fe
est store fe_result
xtreg invest mvalue kstock,re
est store re_result
rhausman fe_result re_result,reps(200) cluster
```
- Interface related inspection
 ```Stata
qui xtreg invest mvalue kstock, fe
xttest2

qui xtreg invest mvalue kstock, re
xtcsd, pesaran
```
