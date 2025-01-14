---
layout: page
permalink: /blogs/Hsu, A., Wang, X., Tan, J. et al. Predicting European cities’ climate mitigation performance using machine learning. Nat Commun/index.html
title: Hsu, A., Wang, X., Tan, J. et al. Predicting European cities’ climate mitigation performance using machine learning. Nat Commun
---

## [Hsu, A., Wang, X., Tan, J. et al. Predicting European cities’ climate mitigation performance using machine learning. Nat Commun](https://doi.org/10.1038/s41467-022-35108-5)

### **Objective:**
- Employ a ML-driven approach to estimating and evaluating the mitigation performance of nearly all local and municipal actors in EU and UK

### **Case:**
- EU + UK

### **Methodology:**
- XGBoost
- SVM
- Random forest
- Feature selection: recursive feature elimination
- Time series: interrupted time series modelling

### **Data Source**
- Self-reported emissions inventory
- Climate action policy
- ODIAC
- Building energy: NASA MERRA
- Emission
- GDP
- Population

### **Findings:**

- Strong correlation between reported emission inventory and stationary fossil-fule CO2 emission
<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221201.png">
</center>

- EUCoM cities have on average, likely reduced annual per capita emissions from 2001 to 2018; 53% of external cities are likely to have experienced a negative trend in emission reductions
<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221202.png">
</center>

- Cities self-reporting emission inventory data are likely to have achieved greater average emissions reductions
<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221203.png">
</center>

<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221204.png">
</center>

<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221205.png">
</center>

<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221206.png">
</center>

<center>
<img src="/blogs/review.assets/NatCom/Hsu NatCom 20221207.png">
</center>

### **Coding Reference:**
- [R](https://github.com/datadrivenenvirolab/citiesML)