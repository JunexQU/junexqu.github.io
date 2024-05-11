---
layout: page
permalink: /blogs/Kraemer, M.U.G., Sadilek, A., Zhang, Q. et al. Mapping global variation in human mobility. Nat Hum Behav 4, 800–810 (2020)/index.html
title: Kraemer, M.U.G., Sadilek, A., Zhang, Q. et al. Mapping global variation in human mobility. Nat Hum Behav 4, 800–810 (2020)
---

## [Kraemer, M.U.G., Sadilek, A., Zhang, Q. et al. Mapping global variation in human mobility. Nat Hum Behav 4, 800–810 (2020)](https://doi.org/10.1038/s41562-020-0875-0)

### **Objective:**
- Globally comprehensive and comparable estimates of human movement are lacking

### **Case:**
- 242 countries, 5 km * 5 km

### **Methodology:**
- Scaling component $\alpha$
  - $p(x) = x^{-\alpha} e^{-\lambda x}$, where $x$ is time value
- $\widehat{\alpha} \approx 1+n[\sum_i^n log(\frac{x_i}{x_min})]^{-1}$
- Regression:
  - $log x_i \approx HAQI * SDI_q + \epsilon$
  - $KS - Distance \approx s(SDI) + s(Nobs) + s(Size) + \epsilon$

### **Data Source: Open**
- [Human movement: only aggregated data](https://bit.ly/2L7FXxc)
- [Spatial grid system](http://s2geometry.io/)
- GDP: World Bank

### **Findings:**

- Data from low-income regions are more concentrated in and around urban areas and along major road
- The lowest frequency of movement is observed in Jan

<center>
<img src="/blogs/review.assets/Kraemer001.png">
</center>

- Global mobility is concentrated primarily between northern latitude 30 and 50
- Weather patterns and length of daylight influence movements

<center>
<img src="/blogs/review.assets/Kraemer002.png">
</center>

- Global mean trip distance is large at 170 km (meadian 11.97 km)
- Trips with length over 60 km make up only 10% of all recorded flows

<center>
<img src="/blogs/review.assets/Kraemer003.png">
</center>

- Trip is highly correlated with sociodemographic index
- When countries are grouped by SDI, the distribution of trip frequencies differ substantially between groups but show strong consistency with each group
- Human movements decline much faster as a function of distance in low-income settings than in high-income settings
- 55% of the countries follow the power law (lognormal distribution); Heterogeneity: income, urban and rural

<center>
<img src="/blogs/review.assets/Kraemer004.png">
</center>

- For cross border movements, the people travel predominantely between countries that are in close proximity and have similar GDP
- The smaller the country, the higher likelihood of travelling internationally as sahre of all movements 
- The frequency of international travel increases remarkedly with proximity to the border

<center>
<img src="/blogs/review.assets/Kraemer005.png">
</center>

### **Coding Reference:**

- Code: Not applicable
