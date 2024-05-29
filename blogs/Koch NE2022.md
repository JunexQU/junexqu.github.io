---
layout: page
permalink: /blogs/Koch, N., Naumann, L., Pretis, F. et al. Attributing agnostically detected large reductions in road CO2 emissions to policy mixes. Nat Energy 7, 844–853 (2022)/index.html
title: Koch, N., Naumann, L., Pretis, F. et al. Attributing agnostically detected large reductions in road CO2 emissions to policy mixes. Nat Energy 7, 844–853 (2022)
---

## [Koch, N., Naumann, L., Pretis, F. et al. Attributing agnostically detected large reductions in road CO2 emissions to policy mixes. Nat Energy 7, 844–853 (2022)](https://doi.org/10.1038/s41560-022-01095-6)

### **Objective:**
- Introduce an approach to implement and answer the reverse causal question of what reduced CO2 emission ? in the EU road transport sector between 1995 and 2008 by first detecting substantial changes in emissios relative to a control group using machine learning and subsequently attributing them to likely causes such as single or interacting policy interventions

### **Case:**
- EU

### **Methodology:**
- Familiar two-way fixed effects:
  - $log(CO2_{it}) = \alpha_i + \phi_t + \sum_j \sum_s \tau_{j,s} l_{i=j, t \geq s} + x' \beta +\epsilon_{i,t}$
- Sparse model

### **[Data Source](https://zenodo.org/records/6768563)**

- Carbon emission in road sector: EDGAR
- GDP and population: World Bank

### **Findings:**

- Ten successful interventions with emissions reductions between 1995 and 2018 and attribute all detected emissions reductions to policy mixes
- Carbon pricing is a critical element of effective policy packages

<center>
<img src="/blogs/review.assets/Koch NE2022001.png">
</center>
 
- The successsful of carbon, fuel or road-use taxes with additional vehicle taxes or subsidies are implemented in Finland, Sweden, Ireland, and Luxembourg

<center>
<img src="/blogs/review.assets/Koch NE2022002.png">
</center>

- Emission saving

<center>
<img src="/blogs/review.assets/Koch NE2022003.png">
</center>

<center>
<img src="/blogs/review.assets/Koch NE2022004.png">
</center>

<center>
<img src="/blogs/review.assets/Koch NE2022005.png">
</center>

<center>
<img src="/blogs/review.assets/Koch NE2022006.png">
</center>

<center>
<img src="/blogs/review.assets/Koch NE2022007.png">
</center>

### **Coding Reference:**

- [R](https://zenodo.org/records/6768563)