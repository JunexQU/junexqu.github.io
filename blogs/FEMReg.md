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

### Estimators

- A standard regression equation is:
  - $y_{it} = \beta_i + \beta_1 X_{it} + \epsilon_{it}$
  - fixed effects: relative to others represented by intercept
  - The equation can be written equivalently as: $Y_{it} = \beta_0 + \beta_1 X_{it} + \gamma_2 D2_i + \gamma_3 D3_i + ... + \gamma_n Dn_i + \mu_{it}$
- To estimate a regression with individual intercepts:
  - $Y_{it} - \overline{Y}_i = \beta_0 + \beta_1 (X_{it}-\overline{X_{i}})+\epsilon_{it}$
- Two-way fixed effects model
  - $Y_{it} = \beta_i + \beta_t + \beta_1 X_{it} + \epsilon_{it}$
  - We are looking at variation within individual as well as within year at this point

### Test
 
- Hausman

