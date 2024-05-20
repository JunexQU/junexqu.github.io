---
layout: page
permalink: /blogs/Camilleri, S.F., Montgomery, A., Visa, M.A. et al. Air quality, health and equity implications of electrifying heavy-duty vehicles. Nat Sustain 6, 1643–1653 (2023)/index.html
title: Camilleri, S.F., Montgomery, A., Visa, M.A. et al. Air quality, health and equity implications of electrifying heavy-duty vehicles. Nat Sustain 6, 1643–1653 (2023)
---

## [Camilleri, S.F., Montgomery, A., Visa, M.A. et al. Air quality, health and equity implications of electrifying heavy-duty vehicles. Nat Sustain 6, 1643–1653 (2023)](https://doi.org/10.1038/s41893-023-01219-0)

### **Objective:**
- The associated air-quality and public health implications that have not yet been widely assessed at the fine spatial resolutions needed to determine different exposure between population subgroups in urban setting

### **Case:**
- Lake Michigan

### **Methodology:**
- WRF-CMAQ model
- SMOKE system
- Multiscale air quality model: [CMAQ](https://github.com/USEPA/CMAQ)


### **Data Source: [Open](https://zenodo.org/records/8234544)**
- Vehicle-to-EGU electricity assignment and emission remapping algorithm: EPA
- Population and demographic: American community survey
- Incidence rate: Industrial economic, incorporated

### **Findings:**

- An instantaneous transition to 30% eHDVs results in on-road emission reductions that more than offset emission increases from EGUs
- The highest-magnitude emission reductions occur along major road networks and within densely populated areas

<center>
<img src="/blogs/review.assets/CamilleriNS2023001.png">
</center>

- 30% adoption of eHDVs reduces population-weighted PM2.5 concentrations
 
<center>
<img src="/blogs/review.assets/CamilleriNS2023002.png">
</center>

- 0.42%-0.05% decreases of all-cause baseline mortality are associated with reductions in NO2 and PM 2.5 

<center>
<img src="/blogs/review.assets/CamilleriNS2023003.png">
</center>

- The deforestation method is a key assumption driving the OC emissions increases

<center>
<img src="/blogs/review.assets/CamilleriNS2023004.png">
</center>

<center>
<img src="/blogs/review.assets/CamilleriNS2023005.png">
</center>

### **Coding Reference:**

- [C++](https://www2.mmm.ucar.edu/wrf/users/download/get_sources.html)
- [Python and R](https://github.com/NU-CCRG/Camilleri-et-al-2022_WRFCMAQ-eHDVstudy)
