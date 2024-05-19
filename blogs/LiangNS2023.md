---
layout: page
permalink: /blogs/Liang, J., Qiu, Y., Liu, P. et al. Effects of expanding electric vehicle charging stations in California on the housing market. Nat Sustain 6, 549–558 (2023)/index.html
title: Liang, J., Qiu, Y., Liu, P. et al. Effects of expanding electric vehicle charging stations in California on the housing market. Nat Sustain 6, 549–558 (2023)
---

## [Liang, J., Qiu, Y., Liu, P. et al. Effects of expanding electric vehicle charging stations in California on the housing market. Nat Sustain 6, 549–558 (2023)](https://doi.org/10.1038/s41893-022-01058-5)

### **Objective:**
- Apply a reduced-form hedonic property value approach where access nearby EV charging infrastructure is capitalized into property values

### **Case:**
- California

### **Methodology:**
- Two-way fixed effects model (generalized DID)
  - Control group: house without proximate EV charging stations (EVCs)
  - Test: Parallel trend
- Endogeneity: IV
- Semiparametric approach


### **Data Source: partial open**
- EVCS: US department of Energy's Alternative Fuels Data Center
- Housing transaction: Zillow
- Population density and income: Bureau of Economic analysis
- EV sales share: California Energy Commission
- Electricity price: EIA
- Environmental awareness: Yale Program on Climate Change Communication
- Traffic flow and PM2.5: monitoring sites in the California highway system
- Establishments: US census bereau

### **Findings:**

- EVCs increased house prices and the magnitudes of the price premium vary across different distance bins
- The largest price premium is 5.8% for houses located about 0.4-0.5 km from charging stations

<center>
<img src="/blogs/review.assets/LiangNS2023001.png">
</center>

- Higher-income residents are significantly more likely to pay a higher premium for houses near public EVCSs, other positive factors including lower market shares, higher environmental awareness
 
<center>
<img src="/blogs/review.assets/LiangNS2023002.png">
</center>

- Installation of charging stations increases the annual traffic by 0.3% and increases the peak month traffic by 0.5%
- PM2.5 decrease by 1.3-2.2%

<center>
<img src="/blogs/review.assets/LiangNS2023003.png">
</center>

- People in multifamily houses do have a higehr willingness to pay for EVCSs
- Houses located fewer than 300 m away from highway chargers experience negative impacts
- Exclusive EVCSs have a lower housing premium at 1.0-3.6%

### **Coding Reference:**

- [Stata and R](https://github.com/jingliang727/evcs_housing_2022)
