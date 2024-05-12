---
layout: page
permalink: /blogs/Elbers, B. Explaining changes in US residential segregation through patterns of population change. Nat Cities 1, 194–204 (2024)/index.html
title: Elbers, B. Explaining changes in US residential segregation through patterns of population change. Nat Cities 1, 194–204 (2024)
---

## [Elbers, B. Explaining changes in US residential segregation through patterns of population change. Nat Cities 1, 194–204 (2024)](https://doi.org/10.1038/s44284-024-00032-w)

### **Objective:**
- Which racial groups are driving changes in segregation
- Where in the metropolitan area these changes are produced

### **Case:**
- US, blocks

### **Methodology:**
- Theoretical foundation: spatial assimilation theory & place strafication theory
- Entropy-based segregation index: $H(T) = \frac{100}{E(T)}\sum_u \sum_g p_{ug} log \frac{p_{ug}}{p_u p_g}$
- Decomposition:
  - $H(B) = H_{macro}(B) + H_{micro}(B)$, where $H_{macro}(B) = H(P)$, $H_{micro}(B) = \sum_{s=1}^{S} \frac{E(B_s)}{E(B)} p_s H(B_s)$
  - game theory
### **Data Source: Open**
- Block-level racial group counts: census through IPUMS NHGIS

### **Findings:**

- Black-white segregation decreased from 58 to 45, while this is still an extremely high level of average segregation

<center>
<img src="/blogs/review.assets/Elbers2024001.png">
</center>

- A large majority of the decrease is due to changes in the population distribution of the Black population; while the distribution of the white people acted in the opposite direction

<center>
<img src="/blogs/review.assets/Elbers2024002.png">
</center>

- The large contributions of the Black population toward decreasing segregation are indeed due to population growth in the suburbs and fringe areas.
- There is also ongoing sorting within suburbs: for white people, both growth and decline in suburban places contributed toward increasing segregation

<center>
<img src="/blogs/review.assets/Elbers2024003.png">
</center>

<center>
<img src="/blogs/review.assets/Elbers2024004.png">
</center>

### **Coding Reference:**

- [Code 2024 (do)](https://osf.io/ykj4r/)
