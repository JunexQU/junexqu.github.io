---
layout: page
permalink: /blogs/Liotta, C., Viguié, V. & Creutzig, F. Environmental and welfare gains via urban transport policy portfolios across 120 cities. Nat Sustain 6, 1067–1076 (2023)/index.html
title: Liotta, C., Viguié, V. & Creutzig, F. Environmental and welfare gains via urban transport policy portfolios across 120 cities. Nat Sustain 6, 1067–1076 (2023)
---

## [Liotta, C., Viguié, V. & Creutzig, F. Environmental and welfare gains via urban transport policy portfolios across 120 cities. Nat Sustain 6, 1067–1076 (2023)](https://doi.org/10.1038/s41893-023-01138-0)

### **Objective:**
- Use a spatially explicit land-use transportation interaction model to systematically assess and compare, on a collection of 120 cities worldwide, the consequence of four urban transport policies on public finance, transportation emissions reduction and housing affordability, as well as health benefits due to variations in air pollution, noise, car accidents and exercise through active transport modes

### **Case:**
- Global 120 cities

### **Methodology:**
- Non-equilibrium dynamic urban model
  - Transport allocation model
  - land-use model based on the monocentric standard urban model (Alonso-Muth-Mills model)


### **Data Source: partial open**
- Grid population: Global human settlement population grid
- Land cover: Europe Space Agency Climate Change Initiative 
- Transport: Google maps
- Real estate: website
- Modal share: Deloitte, CDP, European Platform on Mobility Management Data
- Income per capital growth: 
  - Global IAM-IMACLIM-R (Shared Socioeconomic Pathway 2)
  - [city level GDP per capita](https://stats.oecd.org/Index.aspx?DataSetCode=CITIES)
  - [Brooking GDP per capita](https://www.brookings.edu/research/redefining-global-cities)
  - [World Bank GDP](https://data.worldbank.org/indicator/NY.GDP.PCAP.PP.CD)
  - [FAO agricultural GDP](https://www.fao.org/faostat/en/#home)
- City level population growth: [United Nations](https://population.un.org/wup/Download)
- Marginal cost of air pollution, noise and car accident: [Essen 2019](https://trid.trb.org/view/1646234)
- [Owned grid data](https://zenodo.org/records/7086267)
- Gasoline price: [World Bank](https://data.worldbank.org/indicator/EP.PMP.SGAS.CD)
- Average car fuel consumption: [International Energy Agency](https://www.iea.org/reports/fuel-economy-in-major-car-markets)
- Monetary cost of PT:
  - [Numbeo](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=18)
  - [kiwi.fr](https://www.kiwi.com/stories/cheapest-and-most-expensive-public-transport-revealed)
  - [Wordatlas](https://www.worldatlas.com/articles/cost-of-public-transportation-around-the-world.html)
- GHG dataset

### **Findings:**

- Four policies contribute to the emission reductions

<center>
<img src="/blogs/review.assets/LiottaNS2023001.png">
</center>

- The four policies increase household's financial burden due to the public investment required by the construction of the BRT system, the increased fuel cost for the fuel tax or the icnreased housing prices
- This burden is counterbalanced by health benefits through decreases in air pollution, car accidents and noise, together with an increase in active mode use
 
<center>
<img src="/blogs/review.assets/LiottaNS2023002.png">
</center>

- Fuel tax revenues decrease if vehicles are becoming more fuel-efficient or if the share of electric vehicles increases
- Benefits do not seem to fully compensate for the financial losses

<center>
<img src="/blogs/review.assets/LiottaNS2023003.png">
</center>

- BRT increases welfare and largely mitigates emissions in highly populated, low-income and rapidly growing cities with little PT
- PT availability strongly determines the emissions and welfare effects of the fuel tax
- Fuel tax has the largest impact on emissions mitigation and the largest positive impact on welfare in large and dense cities; while it has a smaller impact on emissions and a negative welfare impact in big and sprawled or small cities with little PT
- The restrictive land-use regulations policy largely mitigates emissions in compact cities with high modal shift potential or in large, poor and growing cities. It also has the large negative welfare impacts
- The fuel efficiency is more efficient at mitigating emissions and increasing welfare in small, high-income or big, poor and sprawled cities with little PT

<center>
<img src="/blogs/review.assets/LiottaNS2023004.png">
</center>

- Mixed policy is more efficient

### **Coding Reference:**

- [Python](https://github.com/CIRED/policy_portfolios)
