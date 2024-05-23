---
layout: page
permalink: /blogs/Nilforoshan, H., Looi, W., Pierson, E. et al. Human mobility networks reveal increased segregation in large cities. Nature 624, 586–592 (2023)/index.html
title: Nilforoshan, H., Looi, W., Pierson, E. et al. Human mobility networks reveal increased segregation in large cities. Nature 624, 586–592 (2023)
---

## [Nilforoshan, H., Looi, W., Pierson, E. et al. Human mobility networks reveal increased segregation in large cities. Nature 624, 586–592 (2023)](https://doi.org/10.1038/s41586-023-06757-3)

### **Objective:**
- A nationwide study of socioeconomic mixing and urbanization has not been undertaken because of difficulties in ascertaining individual-level socioeconomic status (SES), determining when dyadic exposure occur, and amassing the data needed to compare across cities or counties

### **Case:**
- US

### **Methodology:**
- Exposure segregation: $ES = Corr(SES, \overline{SES_es}) = \frac{cov(SES, \overline{SES})}{\sigma_{SES}\sigma_{\overline{SES}}}$

### **Data Source**
- Mobile phone and POIs: SafeGraph
- Home: CoreLogit real estate database
- Rent: Zillow
- Census: American Community Survey
- Transport: Tiger

### **Findings:**

- Exposure segregation is higher in large MSAs
- Exposure segregation is lower because when people venture outside their home tracts, they experience more diversity
- Segregation can be mitigated when frequently visited POIs

<center>
<img src="/blogs/review.assets/Nilforoshan Nature 2023001.png">
</center>
 
<center>
<img src="/blogs/review.assets/Nilforoshan Nature 2023002.png">
</center>

- Larger MSAs offer residents a greater number of leisure choices

<center>
<img src="/blogs/review.assets/Nilforoshan Nature 2023003.png">
</center>

<center>
<img src="/blogs/review.assets/Nilforoshan Nature 2023004.png">
</center>

<center>
<img src="/blogs/review.assets/Nilforoshan Nature 2023005.png">
</center>

### **Coding Reference:**

- [Python](https://github.com/snap-stanford/exposure-segregation)
