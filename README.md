# Unified Thermal Conductivity Dataset of Nanofluids

## Dataset Preview

| Nanoparticle | BaseFluid | Temperature (°C) | Particle Size (nm) | TC (W/mK) |
|-------------|------------|-------------------|-------------------|-----------|
| Al₂O₃ | Water | 25 | 30 | 0.67 |
| CuO | EG | 40 | 50 | 0.82 |

## Overview

The **Unified Thermal Conductivity Dataset of Nanofluids** is a machine-learning-ready dataset containing **987 experimental records** collected and consolidated from multiple peer-reviewed nanofluid studies.

This dataset was developed to support research in:

* Machine Learning for Material Informatics
* Thermal Conductivity Prediction
* Data-Driven Thermal Engineering
* Scientific Computing
* Feature Engineering for Engineering Applications

The dataset combines experimental measurements and engineered features to facilitate predictive modeling and analysis of nanofluid thermal conductivity.

---

## Dataset Statistics

| Attribute     | Value                                      |
| ------------- | ------------------------------------------ |
| Total Records | 987                                        |
| Features      | 12                                         |
| Domain        | Thermal Engineering / Material Informatics |
| Data Source   | Peer-Reviewed Research Studies             |
| Task Type     | Regression                                 |
| Format        | CSV                                        |

---

## Features

| Feature                               | Description                                             |
| ------------------------------------- | ------------------------------------------------------- |
| Nanoparticle                          | Type of nanoparticle used                               |
| BaseFluid                             | Base fluid used in the nanofluid                        |
| Temperature (°C)                      | Experimental temperature                                |
| Particle Size (nm)                    | Average nanoparticle size                               |
| Particle Volume Fraction (%)          | Concentration of nanoparticles                          |
| TC (W/mK)                             | Thermal conductivity of nanofluid (Target Variable)     |
| Thermal Conductivity of Particle (kp) | Thermal conductivity of nanoparticle                    |
| Thermal Conductivity of Liquid (km)   | Thermal conductivity of base fluid                      |
| kp/km ratio                           | Ratio of particle to fluid conductivity                 |
| Temp_Volume                           | Temperature-volume interaction feature                  |
| Inverse_Particle_Size                 | Reciprocal particle size feature                        |
| Brownian_Feature                      | Engineered feature representing Brownian motion effects |

---

## Applications

This dataset can be used for:

* Thermal Conductivity Prediction
* Machine Learning Regression Models
* Feature Importance Analysis
* Material Informatics Research
* Engineering Data Analytics
* Scientific Machine Learning
* Comparative Model Evaluation

---

## Potential Machine Learning Models

Researchers and students can use this dataset with:

* Linear Regression
* Random Forest Regressor
* XGBoost
* Gradient Boosting
* Support Vector Regression (SVR)
* Artificial Neural Networks
* Ensemble Learning Methods

---

## Feature Engineering

To improve machine learning performance, several domain-informed features were engineered:

* **kp/km Ratio** to represent relative conductivity effects
* **Temperature-Volume Interaction** to capture coupled thermal behavior
* **Inverse Particle Size** to model nanoscale size-dependent effects
* **Brownian Feature** to represent particle motion influence on heat transfer

These features were designed using engineering knowledge from nanofluid heat-transfer literature.

---

## Research Motivation

Nanofluids have gained significant attention due to their enhanced thermal properties and applications in heat transfer systems.

The objective of this dataset is to provide a standardized and machine-learning-ready benchmark for researchers interested in applying artificial intelligence and data-driven techniques to thermal conductivity prediction.

---

## Citation

If you use this dataset in academic work, research projects, or publications, please cite this repository and acknowledge the original experimental studies from which the data was compiled.

---

## Author

**Soumy Mittal**

B.Tech Artificial Intelligence & Data Science
Amrita Vishwa Vidyapeetham

### Research Interests

* Machine Learning
* Material Informatics
* Scientific Computing
* Computational Modelling
* Data-Driven Engineering
* Intelligent Systems

---

## License

This dataset is released under the MIT License.
