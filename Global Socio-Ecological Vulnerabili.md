**Global Socio-Ecological Vulnerability to Mining Indicator**



This repository contains the code and data processing workflow used to develop a spatially explicit global indicator of socio-ecological vulnerability to mining impacts, as presented in my Master's Thesis: LINK ZU ARBEI The indicator identifies regions where ecosystems and societies may be particularly vulnerable to potential mining impacts by combining ecological and social proxy variables within a vulnerability framework. The analysis produces a global raster dataset (5 km resolution) representing relative socio-ecological vulnerability across terrestrial areas. For the discussion of the indicator's results as well as it's Interpretation context and limitations, please take into account the explanations in the master's thesis.





**Research Objective**



Mining activities can generate significant environmental and social impacts, including biodiversity loss, water pollution, and conflicts with local communities. However, vulnerability to these impacts varies strongly depending on existing ecological and socio-economic conditions. This project aims to answer the following research question:



How can a spatially explicit socio-ecological indicator of vulnerability to mining impacts be developed at the global scale, and what are its conceptual and methodological limitations?



The resulting indicator is designed as an exploratory and comparative tool to identify spatial patterns of vulnerability rather than to predict impacts at specific mining sites.





**Indicator Concept**



The indicator follows the IPCC AR6 vulnerability framework, where vulnerability is conceptualized as the combination of Sensitivity and Lack of adaptive capacity. The final vulnerability score is calculated as:



Vulnerability = Sensitivity + Lack of Adaptive Capacity



Higher values represent higher relative vulnerability.





**Variables Used**



Sensitivity



* Biodiversity intactness (Biodiversity Intactness Index)
* Protected areas
* Key biodiversity areas
* Indigenous peoples’ and local communities’ lands
* Water Risk
* Poverty



Lack of Adaptive Capacity



* Land rights
* Environmental democracy
* Rule of law
* Conflict index



All variables are normalized to a 0–1 scale and aggregated using simple additive aggregation.





**Spatial Scope**



* Global terrestrial coverage
* Resolution: 5 km raster grid
* Projection: World Cylindrical Equal Area (EPSG:6933)



Spatial datasets were rasterized to the common grid and country-level indicators were spatially joined to country polygons.





**Limitations**



* Data availability and spatial Coverage: The indicator relies on globally harmonized datasets that contain missing values and uneven spatial coverage. Some datasets have incomplete coverage across regions, including parts of Europe, and missing values can affect the spatial representation of certain variables. Consequently, the resulting patterns alsopartly reflect the availability and structure of the underlying datasets.
* Mixed spatial scales: The indicator combines spatially explicit datasets (e.g., protected areas or water risk) with country-level indicators (e.g. governance and poverty measures). Although all layers were harmonized to a common 5 km grid, country-level variables cannot capture subnational variation.
* Proxy variables and simplification: Several variables represent proxies for complex socio-ecological processes. As with any composite indicator, the selection, normalization, and aggregation of variables involve normative methodological choices.
* Colonial continuities and global power asymmetries: Some governance indicators are produced within Global North dominated institutional frameworks. As highlighted during expert consultations, such indicators risk reproducing narratives that frame vulnerability primarily as a problem of governance in the Global South while overlooking historical and structural drivers such as colonial resource extraction and global commodity chains.
* No mining exposure layer: The indicator measures vulnerability to potential mining impacts, not the presence or intensity of mining activity itself. The results should therefore be interpreted as comparative patterns of vulnerability rather than precise predictions of mining impacts.





**Citation**



If you use this repository or the derived datasets, please cite:

Jana Brenn (2026): A Spatially Explicit Global Indicator of Socio-Ecological Vulnerability to Mining Impacts. Master’s Thesis, University of Zurich: URL

