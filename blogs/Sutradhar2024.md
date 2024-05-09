---
layout: page
permalink: /blogs/Sutradhar, U., Spearing, L. & Derrible, S. Depopulation and associated challenges for US cities by 2100/index.html
title: Sutradhar, U., Spearing, L. & Derrible, S. Depopulation and associated challenges for US cities by 2100. Nat Cities 1, 51–61 (2024).
---

## [Sutradhar, U., Spearing, L. & Derrible, S. Depopulation and associated challenges for US cities by 2100. Nat Cities 1, 51–61 (2024)](https://doi.org/10.1038/s44284-023-00011-7)

### **Objective:**
- What are the future population trends in all US cities up to 2100
- Where are depopulating cities
- What are the characteristics of these cities

### **Case:**
- China

### **Methodology:**
- $growth = 0.1 * \frac{P_{20}-P_{10}}{P_{10}}$
  - 5%: severely
  - 1-5%: moderately
  - 0-1%: slowly
- Distribute population to cities
  - area ratio
  - population density
  - projected population
  - Weights: actual and projected
  - MK test: whether time-series data have a monotonic increasing trend or not
- Validation
  - Mean absolute percent error
  - Weighted-(M)APE

### **Data Source: Open**
- US Census
- Population in 2100: Hauer (US), Gao (Global)

    
### **Findings:**

- Major cities in the Midwest regions are slowly losing population
- Urban cities are likely to increase
  
<center>
<img src="/blogs/review.assets/SSP01.png">
</center>

- Higher population density are more likely gain population

<center>   
<img src="/blogs/review.assets/SSP02.png">
</center>

- Urban cities with lower median household income are more likely to experience depopulation

<center>   
<img src="/blogs/review.assets/SSP03.png">
</center>

- Urban cities with low vehicle ownership as well as some suburban and periurban cities with low vehicle owners are likely to experience population growth
- Periurban and rural cities with high vehicle ownership are more likely to gain population

<center>   
<img src="/blogs/review.assets/SSP04.png">
</center>

### **Coding Reference:**

- [Code (2024)](https://github.com/usutradhar/Population-Trend-Analysis)
