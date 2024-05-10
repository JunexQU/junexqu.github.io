---
layout: page
permalink: /blogs/surreg/index.html
title: surreg
---

## Understanding seemingly unrelated regression

### SUR regression

- A generalization of a linear model that consists of several regression equations, each having its own dependent variable and potentially differnts sets of exogenous explanatory variables. 
- **Error terms are assumed to be correlated across the equations**

- Consider a basic function: 
  - Urban function: $Y_{ij} = X_{ij}^{\beta_{ij}} + \mu_{ij}$
  - Rural function: $Y_j = X_{j}^{\beta_{j}} + \mu_j$

- If $Corr(\mu_{ij}, \mu_j) = 0$, we can employ OLS regression directly
- While $Corr(\mu_{ij}, \mu_j) \neq 0$, the separate OLS estimates are no longer valid (the standard errors of the coefficients is too high). A joint estimation (GLS) of the two equations to take into account the correlation between the interference terms of the two can produce a more confidence estimate 
  - Simultaneous equation models: right side includes dependent variable
  - Seemingly unrelated models: right side doesn't include dependent variable

- Model assumption:
  - $E(\mu_{ij} \mu_{ik} | {X_i}) = \sigma_{jk} \neq 0$
- According to the variance-covariance matrix $E(\mu_i \mu_i)$, for a equation $j$ and $k$:
  - $E(\mu_j | X) = 0$ 
  - $E(\mu_j \mu_j | {X}) = \sigma_j I_n$
  - $E(\mu_j \mu_k | {X}) = \sigma_{jk} I_n$
- Variance-covariance matrix of the system of equations:
  - $\Omega = E(\mu \mu' | {X} = \sum \bigotimes I_n )$  
- Estimation:
  - $\widehat{\sum} = = \frac{1}{n}  \widehat{\mu}_{ols} \widehat{\mu'} _{ols}$
  - $\widehat{\Omega}  = \widehat{\sum} \bigotimes I_n$ 
  - $\widehat{\beta} _{sur} = \widehat{\beta} _{gls} \widehat{\Omega} = (X' \widehat{\Omega}^{-1} X) ^{-1} X' \widehat{\Omega}^{-1} y$

### Test
 
- In general, we may carry group differences if the sample includes groups in advance:
  - t-test
  - ANOVA
  - ...

- Based on significant difference between groups, we further apply coefficient differences in SUR estimation:
  - $\chi$: if $p \geq 0.05$, null hypothesis cannot be rejected. 

### Scenario

- Compare various groups, with correlation

