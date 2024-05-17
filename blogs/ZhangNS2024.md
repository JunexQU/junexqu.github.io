---
layout: page
permalink: /blogs/Zhang, P., Carleton, T., Lin, L. et al. Estimating the role of air quality improvements in the decline of suicide rates in China. Nat Sustain 7, 260–269 (2024)/index.html
title: permalink: /Zhang, P., Carleton, T., Lin, L. et al. Estimating the role of air quality improvements in the decline of suicide rates in China. Nat Sustain 7, 260–269 (2024)/index.html

---

## [Zhang, P., Carleton, T., Lin, L. et al. Estimating the role of air quality improvements in the decline of suicide rates in China. Nat Sustain 7, 260–269 (2024)](https://doi.org/10.1038/s41893-024-01281-2)

### **Objective:**
- Whether improvements in air quality may contribute to reductions in suicide rates

### **Case:**
- China counties

### **Methodology:**
- 2SLS
  - Kleibergen-paap F-statistics of the first stage regression is 41.84
- IV  
  - two-sided t-test statistic of t = 2.75 and p = 0.006
- Robust:
  - Replace variables 
### **[Data Source: Open](https://zenodo.org/records/10433250)**
- PM 2.5: China National Environmental Monitoring Center
- Thermal inversion: Modern-Era Retrospective Analysis for Research and Application
- Suicide: Chineses Center for Disease Control and Prevention
- Population: yearbook
- Global national suicide: world health organization

### **Findings:**

- One additional inversion per week raises weekly county-level PM2.5 by 0.51 $\mu$g$m^-3$

<center>
<img src="/blogs/review.assets/Guan2020001.png">
</center>

- The importance of propagation through global supply chains-even countries that are not directly affected by the virus experience large losses, and low- and middle-income countries are more vulnerable to indirect effects

<center>
<img src="/blogs/review.assets/Guan2020002.png">
</center>

- Using thermal inversions as an instrumental variable for PM 2.5, 1 s.t. increase PM 2.5 causes an increase in weekly suiside rates of 0.24 per 1 million individuals (25%)

<center>
<img src="/blogs/review.assets/Guan2020003.png">
</center>

- The suicide rate in people aged 65-85 are far more sensitive to PM 2.5 than in other groups
- The suicide rate for women aged 65-85 increased by 0.04
- No evidence proves displays the relationship between income and suicide 

<center>
<img src="/blogs/review.assets/Guan2020004.png">
</center>

- Suicide rates respond very quickly to climate conditions that increase PM 2.5; weekly suiside rates rise with contemporaneous thermal inversions, which raise PM 2.5
- PM 2.5 improvements policy across China in 2013-17 prevented 45970 suicides

<center>
<img src="/blogs/review.assets/Guan2020005.png">
</center>

### **Coding Reference:**

- [Code (Stata)](https://github.com/tcarleton/suicide-pm)
