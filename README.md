# Global Socio-Ecological Vulnerability to Mining Indicator

This repository contains the code and data processing workflow used to develop a spatially explicit global indicator of socio-ecological vulnerability to mining impacts, as presented in my Master's Thesis: [LINK TO THESIS].

The indicator identifies regions where ecosystems and societies may be particularly vulnerable to potential mining impacts by combining ecological and social proxy variables within a vulnerability framework. The analysis produces a global raster dataset (5 km resolution) representing relative socio-ecological vulnerability across terrestrial areas.

For a detailed discussion of the results, interpretation context, and limitations, please refer to the Master's thesis.

---

## Research Objective

Mining activities can generate significant environmental and social impacts, including biodiversity loss, water pollution, and conflicts with local communities. However, vulnerability to these impacts varies strongly depending on existing ecological and socio-economic conditions.

This project addresses the following research question:

> **How can a spatially explicit socio-ecological indicator of vulnerability to mining impacts be developed at the global scale, and what are its conceptual and methodological limitations?**

The resulting indicator is designed as an **exploratory and comparative tool** to identify spatial patterns of vulnerability rather than to predict impacts at specific mining sites.

---

## Indicator Concept

The indicator follows the **IPCC AR6 vulnerability framework**, where vulnerability is conceptualized as the combination of **Sensitivity** and **Lack of Adaptive Capacity**.

```
Vulnerability = Sensitivity + Lack of Adaptive Capacity
```

Higher values represent higher relative vulnerability.

---

## Variables Used

### Sensitivity
- Biodiversity intactness (Biodiversity Intactness Index)
- Protected areas  
- Key biodiversity areas  
- Indigenous peoples’ and local communities’ lands  
- Water risk  
- Poverty  

### Lack of Adaptive Capacity
- Land rights  
- Environmental democracy  
- Rule of law  
- Conflict index  

All variables are normalized to a **0–1 scale** and aggregated using **simple additive aggregation**.

---

## Spatial Scope

- Global terrestrial coverage  
- Resolution: **5 km raster grid**  
- Projection: **World Cylindrical Equal Area (EPSG:6933)**  

All spatial datasets were rasterized to a common grid, and country-level indicators were spatially joined to country polygons.

---

## Limitations

- **Data availability and spatial coverage**  
  The indicator relies on globally harmonized datasets that contain missing values and uneven spatial coverage. Some datasets have incomplete coverage across regions (including parts of Europe), which affects spatial representation. The resulting patterns therefore partly reflect data availability and structure.

- **Mixed spatial scales**  
  The indicator combines spatially explicit datasets (e.g., protected areas, water risk) with country-level indicators (e.g., governance, poverty). Although all layers were harmonized to a 5 km grid, country-level variables cannot capture subnational variation.

- **Proxy variables and simplification**  
  Several variables act as proxies for complex socio-ecological processes. As with any composite indicator, variable selection, normalization, and aggregation involve normative methodological choices.

- **Colonial continuities and global power asymmetries**  
  Some governance indicators are produced within Global North–dominated institutional frameworks. As highlighted during expert consultations, such indicators risk reinforcing narratives that frame vulnerability primarily as a governance issue in the Global South, while overlooking historical and structural drivers such as colonial extraction and global commodity chains.

- **No mining exposure layer**  
  The indicator measures vulnerability to potential mining impacts, not the presence or intensity of mining activity itself. Results should therefore be interpreted as **comparative vulnerability patterns**, not precise predictions of mining impacts.

---

## Citation

If you use this repository or derived datasets, please cite:

**Jana Brenn (2026)**  
*A Spatially Explicit Global Indicator of Socio-Ecological Vulnerability to Mining Impacts*  
Master’s Thesis, University of Zurich  
[URL]
