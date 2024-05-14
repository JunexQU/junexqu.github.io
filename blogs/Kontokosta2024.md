---
layout: page
permalink: /blogs/Kontokosta, C.E., Hong, B. & Bonczak, B.J. Socio-spatial inequality and the effects of density on COVID-19 transmission in US cities. Nat Cities 1, 83–93 (2024)/index.html
title: Kontokosta, C.E., Hong, B. & Bonczak, B.J. Socio-spatial inequality and the effects of density on COVID-19 transmission in US cities. Nat Cities 1, 83–93 (2024)
---

## [Kontokosta, C.E., Hong, B. & Bonczak, B.J. Socio-spatial inequality and the effects of density on COVID-19 transmission in US cities. Nat Cities 1, 83–93 (2024)](https://doi.org/10.1038/s44284-023-00008-2)

### **Objective:**
- How did neighborhoods in different urban and socioeconomic contexts respond to social distancing policies during the early stage of the pandemic
- What are the effects of land use and density on social distancing behaviors and COVID-19 infection rates
- How do racial and income disparities influence mitigating behaviors in higher-density neighborhoods

### **Case:**
- Census tract, US

### **Methodology:**
- Land use: 1-square-meter resolution, and each pixel represents a specific land use/land cover class
- k-means: identify 5 types of community
  
### **Data Source: Open**
- Exposure density index: Smartphone from VenPath
- Road network, buildings, land use, POIs: OSM
- Infections
- Demographics: American community survey
- Disease and health indicators: Centers for disease control and prevention

### **Findings:**

- The overall activity volume in downtown areas decreased after the stay-at-home compared with pre-COVID; while activities in the peripheral areas remained relatively constant or decreased, a result of a shift to more localized activity around residential areas
- Heterogeneity between cities

<center>
<img src="/blogs/review.assets/Kontokosta2024001.png">
</center>

- Residents in higher-density neighborhoods may perceive a higher risk of infection 
- Quadratic function as the best-fit relationship between residential population density and neighborhood infection rates

<center>
<img src="/blogs/review.assets/Kontokosta2024002.png">
</center>

<center>
<img src="/blogs/review.assets/Kontokosta2024003.png">
</center>

- Race and ethnicity are found to be significant factors in mitigating behavior for higher density neighborhoods
- Educational attainment and job occupation are also important determinants of social distancing and exposure density change

<center>
<img src="/blogs/review.assets/Kontokosta2024004.png">
</center>

<center>
<img src="/blogs/review.assets/Kontokosta2024005.png">
</center>

### **Coding Reference:**

- [Code 2024 (Python)](https://github.com/UrbanIntelligenceLab/socio-spatial-inequality-and-the-effects-of-density-on-covid19-transmission-in-us-cities)
