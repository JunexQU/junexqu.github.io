---
layout: page
permalink: /blogs/Fu, X., Cheng, J., Peng, L. et al. Co-benefits of transport demand reductions from compact urban development in Chinese cities./index.html
title: Fu, X., Cheng, J., Peng, L. et al. Co-benefits of transport demand reductions from compact urban development in Chinese cities. Nat Sustain 7, 294–304 (2024).
---

## Fu, X., Cheng, J., Peng, L. et al. Co-benefits of transport demand reductions from compact urban development in Chinese cities. Nat Sustain 7, 294–304 (2024). https://doi.org/10.1038/s41893-024-01271-4

### **Objective:**
- An integrated approach and provide presumably the first attempt to investigate the implications of CUD for carbon emissions, energy use, air quality, and human health

### **Case:**
- China

### **Methodology:**
- Regression
- Dynamic projection model for emissions in China
  - GCAM-China: energy
  - MEIC: emissions
- Avoided premature mortality: $Mort_{i,j,k} = Pop_{j,k} \cdot Base_j \cdot (\frac{1}{RR_j(C_{i,k})}-\frac{1}{RR_j(C_{Base,k})})$
  - Where j is age group, k is grid box, RR is therelative rist of air-pollution-induced premature death, with air pollutant concentrations C, i is the policy scenario+
- GEMM: $RR(c)= e^{\frac{\theta+log(c/a+1)}{1+e^{-(c-\mu)/v}}}$  
  - Where c is annual average ambient PM2.5 concentration; e is Euler's number; other coefficients are parameters of the shape of RR curves
- Social cost carbon: $M_c = SCC * E_c$
- Value of statistical life: $M_a = VSL * Mort$
- Energy saving

<center>
<img src="/blogs/review.assets/Fu202403.png">
</center>

### **Data Source: Open**
- [DPEC emission](http://meicmodel.org.cn/?page_id=1917)
- [WRF-chem outputs: princeton archive](http://arks.princeton.edu/ark:/88435/dsp01m039k822h)
- [Emission database](https://aims2.llnl.gov/search/input4mips/)
- [ECLIPSE emission](https://previous.iiasa.ac.at/web/home/research/researchPrograms/air/Global_emissions.html)
- [Global burden of disease database](https://ghdx.healthdata.org/)
- [SSP](https://tntcat.iiasa.ac.at/SspDb/dsd?Action=htmlpage&page=10)
- [Technology](https://atb.nrel.gov/electricity/2021/index)
    
### **Findings:**

- In the baseline scenario, transport remains a major emission source and contributes 13%, 25% and 15% of total CO2, NOx and CO in 2050 (38% higher than 2017)
- CUD policy provides co-benefits for climate, energy, air quality and health
  
<center>
<img src="/blogs/review.assets/Fu202401.png">
</center>

- Through reviewing the 5D's framework, negative impacts on private passenger vehicle use can be observed
- Transport emission reductions mainly occur in eastern urban areas.
- CUD policy leads to emission decreases concentrated in cities of all provinces

<center>   
<img src="/blogs/review.assets/Fu202402.png">
</center>

- CUD delivers health co-benefits and avoids 5.8 thousand premature deaths via reductions in non-exhaust vehicle emissions and upstream emissions of air pollutants

<center>   
<img src="/blogs/review.assets/Fu202404.png">
</center>

<center>   
<img src="/blogs/review.assets/Fu202405.png">
</center>

### **Coding Reference:**

- [Code (2014)](https://github.com/wrf-model/WRF/releases/tag/V3.6.1)
