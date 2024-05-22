---
layout: page
permalink: /blogs/Rode, A., Carleton, T., Delgado, M. et al. Estimating a social cost of carbon for global energy consumption. Nature 598, 308–314 (2021)/index.html
title: Rode, A., Carleton, T., Delgado, M. et al. Estimating a social cost of carbon for global energy consumption. Nature 598, 308–314 (2021)
---

## [Rode, A., Carleton, T., Delgado, M. et al. Estimating a social cost of carbon for global energy consumption. Nature 598, 308–314 (2021)](https://doi.org/10.1038/s41586-021-03883-8)

### **Objective:**
- Design a fully modular bottom up architechture, Data-driven spatial climate impact model to develop partial socia cost of carbon (SCC) for individual subsectors of the global economy

### **Case:**
- Global countries

### **Methodology:**
- DSCIM mode:
  - Match data
  - OLS: historical temperature distributions on national annual per-capita energy consumption
  - Coupled model intercomparison project phase 5
  - damage function
  - probabilistic climate-carbon cycle model

### **[Data Source](https://zenodo.org/records/5099834)**
- Energy consumption: IEA (0.25*0.25), electricity and direct fuel consumption across reisidential, commercial, industrial and agricultural end-uses in 146 countries
- Daily temperature: Global meteorological forcing dataset
- Future temporature: Nasa earth exchange global daily downscaled projections
- National income per capita are derived from the shared socioeconomic pathways

### **Findings:**

- Population's income per capita is a key determinant of how its end-use energy consumption responds to temperature
- U-shaped electricity-temperature relationship can be observed, and L-shaped fuels-temperature relationship is identified; these impacts can be enhanced by income growth

<center>
<img src="/blogs/review.assets/Rode Nature2021001.png">
</center>
 
<center>
<img src="/blogs/review.assets/Rode Nature2021002.png">
</center>

- Population adapt to their long-run climate in ways that change their energy consumption during hot and cold periods
- Most of the world is expected to increase net annual per-capital electricity consumption and decrease consumption of other fuels due to climate change
- Hot and wealthy locations show large net increases in electricity consumption

<center>
<img src="/blogs/review.assets/Rode Nature2021003.png">
</center>

- 1 t of CO2 emitted today generates a total energy expenditure burden valued at -US $13.93 to -US0.69

<center>
<img src="/blogs/review.assets/Rode Nature2021004.png">
</center>

### **Coding Reference:**

- [Python, Stata and R](https://github.com/ClimateImpactLab/energy-code-release-2020/)
