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
    - $P = [\sum_i c_i^{\sigma} P_i^{1-\sigma}]^{\frac{1}{1-\sigma}} = [\sum_i a_i^{\sigma}(\frac{P_i}{A \lambda_i})^{1-\sigma}]^{\frac{1}{1-\sigma}} = \frac{1}{A} [\sum_i a_i^{\sigma}(\frac{P_i}{\lambda_i})^{1-\sigma}]^{\frac{1}{1-\sigma}}$
      - Where the relationship between substitution elasticity and CES parameter is: $\sigma = \frac{1}{1-\rho}$, and $\rho = \frac{\sigma-1}{\sigma}$
  - Concequently, the factor input can be derived:
    - $X_i =  (A\lambda_i)^{\sigma-1} a_i^{\sigma} (\frac{P}{P_i})^{\sigma}V$
  - If $A$ is simplified as 1 and $\lambda$ is introduced into initial share parameter:
    - $P = [\sum_i \alpha_i (\frac{P_i}{\lambda_i})^{1-\sigma}]\frac{1}{1-sigma}$
    - $X_i = \alpha_i \lambda_i^{\sigma-1}(\frac{P}{P_i})^{\sigma} V$, where $\alpha_i = a_i^{\sigma}$
    - This equation implies that the CES is a dual price system, representing the average weighted price of production inputs by productivity and input share.
    - If the price of input $i$ increases, the demand for this input will decline, and the extent of decline is determined by the substitution elasticity.
    - When the substitution elasticity equals to 0, the proportion of input demand is fixed, which is unrelated to relative price. This is the Leotief technology or fixed coefficients technology.
  - For two inputs $i$ and $j$:
    - $\frac{X_i}{X_j} = \frac{\alpha_i \lambda_i^{\sigma-1}}{\alpha_j \lambda_j^{\sigma-1}}(\frac{P_j}{P_i})^{\sigma}$
    - The substitute elasticity measures the currency value of the percentage change of the two investment ratios and the relative price percentage change
    - $\frac{\partial{\frac{X_i}{X_j}} \frac{P_i}{P_j}}{\partial{\frac{P_i}{P_j}} \frac{X_i}{X_j}}=-\sigma $
    - In the price of labor increased by 10% relative to capital, the ratio of labor demand and capital demand will decrease 10%$\sigma$
  - In most cases, we do not need the share parameter $a_i$ and $\rho$, they are defined as:
    - $a_{a,0} = (\frac{P_{i,0}}{P_0})^{\sigma}\frac{X_{i,o}}{V_0}$
    - $\alpha_i = \frac{\alpha_{i,0}}{\sum_i \alpha_{i,0}}$
    - $A = (\sum_i \alpha_{i,0})^{1/{\sigma-1}}$
- Cobb-Douglas production function
  - When the $\sigma$ is 1 and $\rho \to 0$, the production function can be written as:
    - $V = A \prod_i (\lambda_i X_i)^{\alpha_i}$, and teh $\sum_i alpha_i = 1$
    - $P = \frac{1}{A}\prod_i(\frac{P_i}{\alpha_i \lambda_i})^{\alpha_i}$
    - $X_i = \alpha_i \frac{P}{P_i}V$
    - Sometimes, we need use $PV = \sum_i P_i V_i$ to replace the dual price, making the substitute elasticity is approximate to 1.
- Leontief production function
  - When the substitute elasticity equals to 0 ($\rho \to -\infty$):
    - $V = min(\frac{\lambda_i X_i}{\alpha_i})$
    - $P = \sum_i \alpha_i(\frac{P_i}{\lambda_i})$
    - $X_i = \frac{\alpha_i}{\lambda_i}V$
- Constant-elasticity-of-transformation (CET):
  - CET is given the constraints of CET production technology, while the CES is given the CES production technology or utility function
    - max $\sum_i^n P_i X_i$
    - s.t. $V = (\sum_i^n g_i X_i^v)^{1/v}$
    - These two equations depict the producer how to distribute their goods in each market to maximize the profit
    - $X_i$ is the supply in market $i$ with a price $P_i$, and $V$ is the aggregation from all markets.
    - Where $P = (\sum_i \gamma_i P_i^{1+w})^{1/(1+w)}$, and $X_i = \gamma_i(\frac{P_i}{P})^w V$
    - And $w = \frac{1}{v-1}, w>0$, and $\gamma_i=g_i^{-w}$, $w$ is the transformed elasticity.
    - In general, $\gamma_i$ id given by: $\gamma_i = (\frac{X_{i,0}}{V_0})(\frac{P_0}{P_{i,0}})^w$
    - The difference is the definition of dual price. In CET, the substitute elasticity is positive. In supply equation, $P_i$ is in the numerator, as our expected, the increasei in price leading the increase in production.
