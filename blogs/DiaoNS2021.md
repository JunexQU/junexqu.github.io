---
layout: page
permalink: /blogs/Diao, M., Kong, H. & Zhao, J. Impacts of transportation network companies on urban mobility. Nat Sustain 4, 494–500 (2021)/index.html
title: Diao, M., Kong, H. & Zhao, J. Impacts of transportation network companies on urban mobility. Nat Sustain 4, 494–500 (2021)
---

## [Diao, M., Kong, H. & Zhao, J. Impacts of transportation network companies on urban mobility. Nat Sustain 4, 494–500 (2021)](https://doi.org/10.1038/s41893-020-00678-z)

### **Objective:**
- How transportation network company (TNC) have changed urban mobility as measured by road congestion

### **Case:**
- US, MSA

### **Methodology:**
- Fixed effects model
  - IV: distance to the nearest TNC hub city
  - Robust: include non-TNC MSA and DID
- Temporal change
  - $y_{it} = \alpha + \beta_1 Year_1 +...+ \beta_n Year_n + \theta_i + \tau_t + \epsilon_{it}$   

### **Data Source: partial open**
- [National transit database](https://www.transit.dot.gov/ntd/ntd-data)
- [Federal highway administration](https://ops.fhwa.dot.gov/perf_measurement/ucr/)
- [Bureau of economic analysis](https://www.bea.gov/data/gdp)
- [American community survey](https://www.census.gov/programs-surveys/acs/data.html)

### **Findings:**

- TNCs increased road congestion in terms of both intensity and duration
- TNC leads to a decline of PT ridership and reduce vehicle ownership

<center>
<img src="/blogs/review.assets/Diao2021001.png">
</center>

- The entry of the second TNC operator increased congestion hour
 
<center>
<img src="/blogs/review.assets/Diao2021002.png">
</center>

<center>
<img src="/blogs/review.assets/Diao2021003.png">
</center>

<center>
<img src="/blogs/review.assets/Diao2021004.png">
</center>

### **Coding Reference:**

- [Python 2020](https://github.com/ccolon/disrupt-supply-chain-model)
