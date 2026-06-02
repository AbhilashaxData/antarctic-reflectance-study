# The Antarctic Baseline 

### Quantifying Environmental Dynamics Across the Larsen C Ice Shelf Using Machine Learning

## Overview

Antarctic surface albedo plays a critical role in regulating Earth's energy balance by controlling how much incoming solar radiation is reflected back into the atmosphere. Understanding the environmental drivers of surface reflectivity is therefore important for studying cryospheric processes and climate-related change.

This project investigates surface albedo dynamics across the Larsen C Ice Shelf using a decade of satellite-derived environmental observations extracted through Google Earth Engine (GEE). Rather than relying on large geospatial raster workflows, the study converts Earth Observation data into a lightweight machine learning dataset and explores multiple modeling approaches for understanding environmental behavior in one of the planet's most extreme environments.

---

## Study Area

**Larsen C Ice Shelf, Antarctica**

The Larsen C Ice Shelf is one of Antarctica's largest remaining ice shelves and has attracted significant scientific attention due to its environmental sensitivity and long-term structural changes. Its relatively isolated location provides an opportunity to examine environmental signals with minimal direct human influence.

**Observation Period:** 2015-2025

---

## Project Objectives

This study was designed around four central questions:

* Can Antarctic surface albedo be modeled using a small set of satellite-derived environmental indicators?
* Do non-linear relationships exist between environmental conditions and surface reflectivity?
* How do global regression approaches compare with localized tree-based learning methods?
* Which environmental variables contribute most strongly to model predictions?

---

## Project Structure

### Part 1: Polynomial Regression and Gradient Descent

The first phase establishes a statistical baseline using a custom Degree-2 Polynomial Regression model optimized through Gradient Descent.


### Part 2: Ensemble Learning and Explainable AI

The second phase extends the analysis using tree-based machine learning methods and model explainability techniques.


---

## Data Sources

Environmental observations were extracted from MODIS products hosted on Google Earth Engine.

| Dataset | Environmental Variable |
| ------- | ---------------------- |
| MOD11A1 | Surface Temperature    |
| MOD09GA | Solar Zenith Angle     |
| MCD43A3 | Surface Albedo         |

The resulting dataset was processed into a tabular format suitable for machine learning experimentation and analysis.

---

## Repository Contents

```text
.
├── data/
│   └── larsen_c_cleaned_data.csv
│
├── notebooks/
│   ├── antarctica_part1.ipynb
│   └── antarctica_part2.ipynb
│
├── reports/
│   ├── Antarctica_Part1_.pdf
│   └── Antarctica_Part2_.pdf
│
├── images/
│   ├── learningcurveantarctic.png
│   ├── actualvspredictedalbedo.png
│   ├── residualerrorvspredictedalbedo.png
│   ├── residualerrordensitydist.png
│   ├── decisiontree_antarcticasolarzenith.png
│   ├── modelexplanabilityshapantarctica.png
│   └── solarzenithSHAPantarctica.png
│
├── README.md
└── LICENSE
```

---

## Technologies Used

* Python
* Google Earth Engine
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* SHAP

---

## Notes

This repository is intended as an exploratory machine learning study of Antarctic environmental dynamics. The notebooks contain the complete methodology, analysis workflow, visualizations, model diagnostics, and interpretation of results.

---

## Author

**Abhilasha Das**
MSc Data Science

