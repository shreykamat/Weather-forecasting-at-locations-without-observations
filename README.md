# Weather Forecasting at Unobserved Locations

This repository contains work from an **MSc Data Science dissertation** conducted at the **University of Leeds (UK)** in collaboration with the **UK Met Office**.

The project investigates how **machine learning–based climatology models** can be used to improve temperature predictions at **unobserved locations**, with the ultimate goal of enhancing numerical weather forecast post-processing.

---

## 📌 Project Overview

Accurate weather forecasts rely heavily on observations, yet many regions of the world remain sparsely observed. This project explores whether **machine learning models trained on large-scale temperature observations** can better represent climatology and improve forecast skill, particularly in data-scarce locations.

The study uses a large temperature observation dataset consisting of:

- **9+ million observations**
- **7000+ locations**
- **Global spatial coverage across all continents**

Using this data, the project evaluates the performance of machine learning methods for temperature climatology modelling and their integration into operational forecast post-processing workflows.

---

## 🎯 Objectives

The key objectives of this project are:

- To evaluate the performance of **machine learning methods** (Neural Networks and Random Forests) for temperature climatology modelling  
- To compare **regional (UK-only)** training against **global** training strategies  
- To identify model configurations that generalise well across different spatial scales  
- To integrate selected machine learning climatology models with the **Standard Anomaly Model Output Statistics (SAMOS)** framework in order to improve forecast skill  

---

## 🧠 Methodology

The repository focuses on the **machine learning climatology component** of the workflow. Specifically, it includes notebooks that:

- Build temperature climatology models using:
  - Neural Networks
  - Random Forests
- Compare model performance under different configurations:
  1. **UK-only training domain vs global training domain**
  2. **Neural Networks vs Random Forests**
- Evaluate performance across two spatial scopes:
  - **UK-focused evaluation**
  - **Global-scale evaluation**

This dual-scope evaluation allows assessment of **regional adaptability** and highlights trade-offs between locally trained and globally trained models.

---

## 🔒 Data Availability & Restrictions

> **Important note on data access**

The full datasets used in this project include **UK Met Office observational data** and internal model outputs. These datasets, along with code related to direct integration with the SAMOS framework, **cannot be publicly redistributed** due to licensing and institutional restrictions.

As a result:
- Raw data files are **not included**
- SAMOS integration code is **not included**
- The repository focuses on **model development, experimentation, and comparative analysis**

The provided notebooks are intended to demonstrate **methodology, modelling choices, and evaluation strategies**, and can be adapted to equivalent open or synthetic datasets.

---

## 📂 Repository Contents

This repository contains notebooks that:

- Construct temperature climatology models using machine learning
- Compare regional vs global training strategies
- Analyse and visualise model performance
- Support reproducibility of the modelling approach (excluding restricted data)

---

## 🧪 Key Comparisons Performed

- **Training domain**
  - UK-only vs global observations
- **Model type**
  - Neural Networks vs Random Forests
- **Spatial generalisation**
  - Regional performance vs global performance

---

## 📊 Results Summary

The results show that both **training domain** and **model choice** have a significant impact on climatology performance at unobserved locations.

### Training Domain Effects

- **Globally trained models** consistently demonstrated stronger generalisation, particularly in regions with sparse observations.
- **UK-only models** performed well within the UK but showed reduced robustness when applied beyond the local training domain.
- These findings highlight the value of **large and diverse training datasets** for transferable climatology modelling.

### Model Performance

- **Random Forests** provided strong, stable baseline performance with minimal tuning.
- **Neural Networks** achieved improved performance in data-rich settings, capturing complex nonlinear spatial patterns more effectively.
- Neural networks benefited most from **global training**, where increased data diversity supported better generalisation.

### SAMOS Integration

- Selected machine learning climatology configurations were integrated into the **Standard Anomaly Model Output Statistics (SAMOS)** framework.
- ML-based climatology improved the representation of temperature anomalies compared to baseline approaches.
- This demonstrates the potential of **machine learning–enhanced climatology** for operational forecast post-processing.

Overall, the results indicate that **globally trained machine learning climatology models**, combined with established post-processing frameworks, offer a robust approach for improving temperature forecasts at unobserved locations.


## 🚀 Potential Applications

- Improving forecast skill at **unobserved or sparsely observed locations**
- Enhancing post-processing frameworks such as SAMOS
- Informing strategies for **regional vs global model training**
- Supporting scalable, data-driven climatology modelling
---

## 📖 Disclaimer

This repository represents academic research conducted as part of an MSc dissertation. It is **not an operational forecasting system**, but rather an exploration of modelling strategies that may inform future operational workflows.
