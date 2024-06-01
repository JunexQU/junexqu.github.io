---
layout: page
permalink: /science/Prieto-Curiel, Rafael, Jorge E. Patino, and Brilé Anderson. Scaling of the morphology of African cities. Proceedings of the National Academy of Sciences 120.9 (2023)/index.html
title: Prieto-Curiel, Rafael, Jorge E. Patino, and Brilé Anderson. Scaling of the morphology of African cities. Proceedings of the National Academy of Sciences 120.9 (2023)
---

## [Prieto-Curiel, Rafael, Jorge E. Patino, and Brilé Anderson. Scaling of the morphology of African cities. Proceedings of the National Academy of Sciences 120.9 (2023)](https://doi.org/10.1073/pnas.2214254120)

### **Objective:**
- Analyze the scaling impact of population size on urban form and the challenge of accommodating the growing number of people in a more efficient and sustainable way

### **Case:**
- China, EU, US, India and Brazil

### **Methodology:**
- Mean interbuilding distance: $D_i = \frac{128}{45\pi}(B_i A_i S_i E_i)^{1/2}$
- City shape: $E_i = \frac{\pi^{1/2}M_i}{2(B_i A_i)^{1/2}}$
- Sprawl of a city: $S_i = \frac{45^2 \pi^{3/2}D_i^2}{2^{13}M_i ((B_i A_i)^{1/2})} = \gamma\frac{D_i^2}{M_i (B_i A_i)^{1/2}}$
- Polycentrism index: $\phi_i = \frac{1}{v_1} \sum_k kv_k$
- BASE model: $B_i = \alpha P_i^{\beta}$

### **Data Source**
- [Google AI Africa Open Building](https://mapping-africa-transformations.org/)

### **Findings:**

- The number of buildings within a city grows with population, but decreases slightly with size

<center>
<img src="/science/review.assets/Prieto-Curiel PNAS2023001.png">
</center>

<center>
<img src="/science/review.assets/Prieto-Curiel PNAS2023002.png">
</center>

- Small buildings (68.5%), and big buildings represent a large part of the constructed surface of a city
- Buildings average size scales with the city's population

<center>
<img src="/science/review.assets/Prieto-Curiel PNAS2023003.png">
</center>

- A city with ten times the population will demand 34 times more energy than transport
- The densest point in a city with more than 1 million people has 30 or 40% of the surface built up, as opposed to small towns with less than 100,000inhabitants (less than 10%)

<center>
<img src="/science/review.assets/Prieto-Curiel PNAS2023004.png">
</center>

<center>
<img src="/science/review.assets/Prieto-Curiel PNAS2023005.png">
</center>

<center>
<img src="/science/review.assets/Prieto-Curiel PNAS2023006.png">
</center>

### **Coding Reference:**

- [R](https://github.com/rafaelprietocuriel/UrbanFragmentation)
