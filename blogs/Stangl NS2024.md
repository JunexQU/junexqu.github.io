---
layout: page
permalink: /blogs/Stangl, J., Borsos, A., Diem, C. et al. Firm-level supply chains to minimize unemployment and economic losses in rapid decarbonization scenarios. Nat Sustain 7, 581–589 (2024)/index.html
title: Stangl, J., Borsos, A., Diem, C. et al. Firm-level supply chains to minimize unemployment and economic losses in rapid decarbonization scenarios. Nat Sustain 7, 581–589 (2024)
---

## [Stangl, J., Borsos, A., Diem, C. et al. Firm-level supply chains to minimize unemployment and economic losses in rapid decarbonization scenarios. Nat Sustain 7, 581–589 (2024)](https://doi.org/10.1038/s41893-024-01321-x)

### **Objective:**
- The role of the firm-level production network in the propagation and amplification of economic shocks originating from rapid decarbonization

### **Case:**
- Hungary

### **Methodology:**
- The loss of economic output (OW-ESRI):
  - $OW-ESRI_j = \sum_i \frac{s_i^{out}}{\sum_l s_l^{out}}[1-h_i(T)]$
- Remove firms

### **Data Source**

- Financial transactions: National Bank of Hungary

### **Findings:**

- Summarize IAM model
- For the firm joined ETS, most of them cluster around low emissions and low economic relevance 

<center>
<img src="/blogs/review.assets/Stangl NS2024001.png">
</center>
 
- The firm with the highest CO2 emissions in 2019 accounts for 6.98% of total carbon emissions
- 1% of job would be lost in the short term if firms were to stop its production but 7% of annual co2 emissions could be saved

<center>
<img src="/blogs/review.assets/Stangl NS2024002.png">
</center>

- The 'Remove largest emitters first' can reach the highest emission savings

<center>
<img src="/blogs/review.assets/Stangl NS2024003.png">
</center>

<center>
<img src="/blogs/review.assets/Stangl NS2024004.png">
</center>

### **Coding Reference:**

- [Python EU Transaction Log](https://github.com/jabrell/pyeutl)
- [R and Python](https://github.com/jo-stangl/reducing_employment_and_economic_output_loss_in_rapid_decarbonization_scenarios)