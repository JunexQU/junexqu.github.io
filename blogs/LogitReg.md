---
layout: page
permalink: /blogs/logitreg/index.html
title: logitreg
---

## Logit (0,1) model

### [0-1 logit model](https://www.lianxh.cn/news/e18031ffad4f3.html)

- Dependent variable only includes two value: 0-1. 
- **Need a probability model**

- Consider the probability of choose 1 ($\pi_i$), random variable $Y_i$ follow a $(0-1)$ distribution of $\pi_i$
  - $P_{Y_i = y_i} = \pi_i^{y_i}(1-\pi_i)^{1-y_i}$, $y_i = 0,1$
- The expectation and variance are respectively:
  - $E(Y_i) = \pi_i$
  - $Var(Y_i) = \pi_i (1-\pi)$

- Define odd ratio:
  - $\Omega_i = \frac{\pi_i}{1-\pi_i}$
  - $logit (\Omega_i) = ln(\Omega_i) = ln (\frac{\pi_i}{1-\pi_i})$
- If we assume $\pi_i$ follows the linear model:
  - $logit (\Omega_i) = ln (\frac{\pi_i}{1-\pi_i}) = x_i' \beta$
- The probability can be estimated from the antlogit:
  - $\pi_i (x_i) = \frac{exp(x_i' \beta)}{1+exp(x_i' \beta)}$
  - and, $y_i = \pi(xi) + \epsilon_i$

- $\beta_i$ measures when change in $x_j$ unit, $ln(\Omega_j)$ change $\beta_j$ unit
  - **It's too difficult to display the economic content of the coefficient**
- So we calculate odd ratio:
  - $\Omega_i = exp(x_i'\beta)$
  - $\Omega_i(x_i, x_{ij}+1) = exp(x_i'\beta) exp(\beta_j)$
  - $\frac{\Omega(x, x_j+1)}{x, x_j} = exp(\beta_j)$
  - $\beta_j$ measures when change in $x_j$ unit, the odds of winning are $exp(\beta_j)$ times the original
- Besides, we usually use average marginal effect:
  - When $x$ increases by 1 unit, the probability that the $Y$ change by $\beta%$

### Test
 
- $\Chi^2$
- $df$
- $AIC$
- $BIC$
