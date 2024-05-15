---
layout: page
permalink: /blogs/Pangallo, M., Aleta, A., del Rio-Chanona, R.M. et al. The unequal effects of the health–economy trade-off during the COVID-19 pandemic. Nat Hum Behav 8, 264–275 (2024)/index.html
title: permalink: /Pangallo, M., Aleta, A., del Rio-Chanona, R.M. et al. The unequal effects of the health–economy trade-off during the COVID-19 pandemic. Nat Hum Behav 8, 264–275 (2024)/index.html

---

## [Pangallo, M., Aleta, A., del Rio-Chanona, R.M. et al. The unequal effects of the health–economy trade-off during the COVID-19 pandemic. Nat Hum Behav 8, 264–275 (2024)](https://doi.org/10.1038/s41562-023-01747-x)

### **Objective:**
- Develop an ABM model to simulate the epidemic and economic impacts on a large synthetic population

### **Case:**
- New York-Newark-Jersey city

### **Methodology:**
- ABM:  
  - Infected probability: $P(S_i+I_j \rightarrow L_i+I_j) = 1-e^{-\beta_{type}w_{i,j,p}(t)\Delta t}$
  
### **Data Source: Open**
- Global positioning system location data: Cuebig
- American community survey
- Bureau of economic analysis
- Bureau of labor statistics

### **Findings:**

- Employment declined more strongly than GDP

<center>
<img src="/blogs/review.assets/Pangallo2023001.png">
</center>

- Consumption of goods and services produced by customer-facing industries declined more strongly than consumption of goods and services produced by industries that are not customer facing (i.e., manufacturing, financial service)

<center>
<img src="/blogs/review.assets/Pangallo2023002.png">
</center>

- Fear of infection parameter distribution implies a 14% consumption demand reduction in customer-facing industries

<center>
<img src="/blogs/review.assets/Pangallo2023003.png">
</center>

<center>
<img src="/blogs/review.assets/Pangallo2023004.png">
</center>

<center>
<img src="/blogs/review.assets/Pangallo2023005.png">
</center>

<center>
<img src="/blogs/review.assets/Pangallo2023006.png">
</center>

### **Coding Reference:**

- [Code and data (Python)](https://zenodo.org/records/7946868)
