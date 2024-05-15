---
layout: page
permalink: /blogs/CGE/index.html
title: CGE
---

## CGE model

### Data

#### Closed economy
- Input-output table
- Social accounting matrix (SAM)

- SAM is a square matrix: $T= {t_{ij}}$, where $t_{ij}$ is the income from $i$ to $j$, meanwhile it is also the expenditure from $j$ to $i$
- The income must equal to expenditure: $\sum_j t_{jk} = \sum_j t_{kj}$
- For a closed economy, economic activity is divided into three categories: Consumption (C), Capital income (I) and Expenditure on production factor (Y); the income (Y) is used to consume goods and consumptions (C) and saving (S), then the saving is transformed to investment (represented by capital income (I)). 

<center>
<img src="/blogs/review.assets/CGE001.png">
</center>

- The macro-equilibrium equation can be expressed as:
  - $Y = C + I$
  - $C + S = Y$
  - $I = S$

#### Open economy
- In the new table, production and consumption account is redefined as producer and residens (consumer); government is also included as an agent. In addition, the economy is open, representing by the rest of world (ROW)
- In this table, producers get income through selling the final products to residents (C) and government (G), getting profit from capital investment (I), also exporting products to ROW (E). The income is allocated into factor cost for residents (Y) and ROW (M).
- Residents' expenditure include consumption (C), Tax (T) and saving $S_h$.
- Government's expenditure includes consumption (G) and government saving ($S_g$)
- Income of ROW is represented by export (E) and foreign saving ($S_f$). $S_f$ is the negative value of domestic trade balance

<center>
<img src="/blogs/review.assets/CGE002.png">
</center>

- The macro-equilibrium equation can be expressed as:
  - Gross domestic production: $Y +M = C + G + I + E$
  - Income: $C + T + S_h = Y$
  - Government Budget: $G + S_g = T$
  - Saving-investment: $I = S_g + S_h + S_f$
  - International trade balance: $E + S_f = M$

- A genral SAM is:
<center>
<img src="/blogs/review.assets/CGE003.png">
</center>

- Update SAM:
  - RAS algorithm
  - Minimizing of a constrained quadratic loss function
  - Maximum entropy tabular reconciliation
- Global trade:
  - Gravity model

### Model development
#### Production theory

- Constant elasticity of substitution (CES)
  - For a producer, production technology is given by a CES equation under current optimal combination of factor inputs in a competitive market
    - $min \sum_i^n P_i X_i$, where $X_i$ is the production input, $P_i$ is the price
    - s.t. $ V = A[\sum_i^n a_i(\lambda_i X_i)^{\rho}]^{1/\rho}$, where $V$ is the production, $a_i$ is the share parameters. $A$ is the transformation parameter; $\lambda$ is the transformation parameter for each input
    - Specifically, neutral productivity growth is achieved by $A$, Hicks neutral production growth can only be achieved by $\lambda$
  - For the optimizaiton of producer, we set the Lagrangian equation:
    - $L = \sum_i P_i X_i + P(V-A[\sum_i a_i(\lambda_i X_i)^{\rho}]^{1/\rho})$
  - Calculate the partial differentiation for $X_i$ and $P$ and set the calculated equation equals to 0:
    - $P_i = P[\sum_i c_i X_i^{\rho}]^{\frac{1-\rho}{\rho}} c_i X_i^{\rho-1} = P V^{1-\rho} c_i X_i^{\rho-1} $
    - $V = [\sum_i c_i X_i^{\rho}]^{1/\rho}$
    - $c_i = a_i (A\lambda_i)^{\rho}$ 
  - Thus, we can obtain:
    - $X_i = [\frac{c_i P}{P_i}]^{\frac{1}{1-\rho}} V$
    - $V = [\sum_i c_i [\frac{c_i P}{P_i}]^{\frac{\rho}{1-\rho}} V^{\rho}]^{\frac{1}{\rho}}$
    - $P = [\sum_i c_i^{\sigma} P_i^{1-\sigma}]^{\frac{1}{1-\sigma}} = [\sum_i a_i^{\sigma}(\frac{P_i}{A \lambbda_i})^{1-\sigma}]^{\frac{1}{1-\sigma}} = \frac{1}{A} [\sum_i a_i^{\sigma}(\frac{P_i}{\lambda_i})^{1-\sigma}]^{\frac{1}{1-\sigma}}$
      - Where the relationship between substitution elasticity and CES parameter is: $\sigma = \frac{1}{1-\rho}$, and $\rho = \frac{\sigma-1}{\sigma}$
  - Concequently, the factor input can be derived:
    - $X_i =  (A\lambda_i)^{\sigma-1} a_i^{\sogma} (\frac{P}{P_i})^{\sigma}V$
  - If $A$ is simplified as 1 and $\lambda$ is introduced into initial share parameter:
    - $P = [\sum_i \alpha_i (\frac{P_i}{\lambda_i})^{1-\sigma}]\frac{1}{1-sigma}$
    - $X_i = \alpha_i \lambda_i^{\sigma-1}(\frac{P}{P_i})^{\sigma} V$, where $\alpha_i = a_i^{\sigma}$