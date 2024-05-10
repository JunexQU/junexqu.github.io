---
layout: page
permalink: /blogs/Arvidsson, M., Lovsjö, N. & Keuschnigg, M. Urban scaling laws arise from within-city inequalities/index.html
title: Arvidsson, M., Lovsjö, N. & Keuschnigg, M. Urban scaling laws arise from within-city inequalities. Nat Hum Behav 7, 365–374 (2023).
---

## [Arvidsson, M., Lovsjö, N. & Keuschnigg, M. Urban scaling laws arise from within-city inequalities. Nat Hum Behav 7, 365–374 (2023)](https://doi.org/10.1038/s41562-022-01509-1)

### **Objective:**
- Do phenomena that have heavier tails scale more or less than those with smaller tails?
- How much of the variance in scaling exponents across complexity categories (i.e. industries and occupations) can be explained by differences in the tails?
- What mechnism underlie the emergence of tail differences by city size?

### **Case:**
- Russia, Ukraine, Swedish, US

### **Methodology:**
- Scaling component $\beta$
  - $log Y_c = log Y_0 + \beta log N_c + \epsilon_c$, where $Y$ is population size
- d: $d = \sum_i^N (y \geq p_{90}) / \sum_i^N (y < p_{90})$
- Agent simulation:
  - Probability that an individual $i$ of type $j$ interacts with another agent of type $k$ in city $c$ at time $t$:
    - $p_{ijkct} = \frac{F_{kc}(C_{jk}^{\theta}+D_{ilt-1}^{\psi})}{\sum_l F_{lc}(C_{jl}^{\theta}+D_{ilt-1}^{\psi})}$, where $F_{kc}$ is the fraction,$C_{jk}$ is the complementarity between agents, $D_{ilt-1}$ is the distance, $\theta$ captures how the probability interaction is affected by complementarity, $\psi$ governs the path dependency 
  - Individual-level productivity:
    - $y_{it} = y_{it-1} (1+\alpha_0 \frac{C_{it}^w}{S_i^{\tau}})$, where $S_i$ is the integar qualifying specialization rank, $w$ controls the returns to complementarity, $\tau$ specifies how return to complementarity are moderated by specilization, $\alpha$ defines the learning rate

### **Data Source: Open**
- [Open Science Framework](https://osf.io/uhsmz/)
- [On line networking](https://dev.vk.com/ru/api/open-api/getting-started?ref=old_portal)
- [US Patent](https://patentsview.org/)
- Population: Statistics and Census

### **Findings:**

- Interconnectivity, productivity and innovation are highly skewed in cities, and their tailedness increases with city size

<center>
<img src="/blogs/review.assets/Arividsson001.png">
</center>

- Tail differences by city size

<center>
<img src="/blogs/review.assets/Arividsson002.png">
</center>

- Individuals' productivity depends on the local social environment

<center>
<img src="/blogs/review.assets/Arividsson003.png">
</center>

- Agents who from an early stage draw on big-city benefits achieve sustained growth
- Average wage of those workers who earned median or tail wages at age 30

<center>
<img src="/blogs/review.assets/Arividsson004.png">
</center>

### **Coding Reference:**

- [Code (2022)](https://osf.io/uhsmz/)
