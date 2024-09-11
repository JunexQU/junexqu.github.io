---
layout: page
permalink: /blogs/Wang, S., Zheng, Y., Wang, G. et al. Infrequent activities predict economic outcomes in major American cities. Nat Cities/index.html
title: Wang, S., Zheng, Y., Wang, G. et al. Infrequent activities predict economic outcomes in major American cities. Nat Cities
---

## [Wang, S., Zheng, Y., Wang, G. et al. Infrequent activities predict economic outcomes in major American cities. Nat Cities](https://doi.org/10.1038/s44284-024-00051-7)

### **Objective:**
- The fundamental link between mobility and economy is still missing
- Key: method ref

### **Case:**
- Global cities

### **Methodology:**
- Network
- Power law
- ML: 
  - linear regression with elastic net regularization to tackle overfitting
  - Gradient boosting regressions to identify non-linearly predictive activities
- Sensitivity:
  - Gauassian noise: randomly omitting 10% of the data and dropp the data below the lower bounds and above the upper bound
  - Transferability test
  - Benchmarking frequent activities
  - Grouping activities
- Temporal regression

### **Data Source**
- Mobility: MIT IRB office
- Socioeconomic: American community survey
- 

### **Findings:**

- Mobility activities can predict more than 50% of variation in income and property values

<center>
<img src="/blogs/review.assets/Wang NCities 202405001.png">
</center>
 
- A small fraction of infrequent activities is needed to achieve relatively high performance

<center>
<img src="/blogs/review.assets/Wang NCities 202405002.png">
</center>

<center>
<img src="/blogs/review.assets/Wang NCities 202405003.png">
</center>

<center>
<img src="/blogs/review.assets/Wang NCities 202405004.png">
</center>

### **Coding Reference:**

- [Python](https://github.com/cjsyzwsh/economic_growth_usa)