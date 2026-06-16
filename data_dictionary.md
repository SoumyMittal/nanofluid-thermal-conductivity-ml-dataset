# Data Dictionary

This document describes the variables included in the **Unified Thermal Conductivity Dataset of Nanofluids**.

---

# Dataset Information

| Property        | Value                                      |
| --------------- | ------------------------------------------ |
| Records         | 987                                        |
| Features        | 12                                         |
| Target Variable | TC (W/mK)                                  |
| Problem Type    | Regression                                 |
| Domain          | Thermal Engineering / Material Informatics |

---

# Feature Descriptions

## 1. Nanoparticle

**Type:** Categorical

**Description:**
Represents the type of nanoparticle dispersed within the base fluid to form the nanofluid.

**Examples:**

* Al₂O₃
* CuO
* TiO₂
* SiO₂
* ZnO
* Graphene
* CNT

**Importance:**
Different nanoparticles possess different thermal conductivities, significantly influencing overall nanofluid performance.

---

## 2. BaseFluid

**Type:** Categorical

**Description:**
Represents the carrier fluid in which nanoparticles are suspended.

**Examples:**

* Water
* Ethylene Glycol
* Propylene Glycol
* Water-EG Mixtures
* Oils

**Importance:**
The thermal properties of the base fluid directly affect heat transfer characteristics.

---

## 3. Temperature (°C)

**Type:** Numerical

**Unit:** Degrees Celsius (°C)

**Description:**
Experimental operating temperature at which thermal conductivity was measured.

**Importance:**
Temperature influences particle motion, fluid properties, and thermal conductivity behavior.

---

## 4. Particle Size (nm)

**Type:** Numerical

**Unit:** Nanometers (nm)

**Description:**
Average size of nanoparticles used in the nanofluid.

**Importance:**
Smaller particles often exhibit stronger Brownian motion and different heat transfer characteristics.

---

## 5. Particle Volume Fraction (%)

**Type:** Numerical

**Unit:** Percentage (%)

**Description:**
Concentration of nanoparticles present within the base fluid.

**Importance:**
One of the most influential variables affecting nanofluid thermal conductivity.

---

## 6. TC (W/mK)

**Type:** Numerical

**Unit:** Watts per meter-Kelvin (W/mK)

**Description:**
Measured thermal conductivity of the nanofluid.

**Role:**
🎯 **Target Variable**

**Importance:**
This is the quantity to be predicted using machine learning models.

---

## 7. Thermal Conductivity of Particle (kp)

**Type:** Numerical

**Unit:** W/mK

**Description:**
Thermal conductivity of the nanoparticle material.

**Importance:**
Materials with higher thermal conductivity generally contribute to improved heat transfer performance.

---

## 8. Thermal Conductivity of Liquid (km)

**Type:** Numerical

**Unit:** W/mK

**Description:**
Thermal conductivity of the base fluid.

**Importance:**
Serves as a baseline reference for thermal conductivity enhancement.

---

## 9. kp/km Ratio

**Type:** Numerical

**Description:**
Ratio between nanoparticle thermal conductivity and base fluid thermal conductivity.

### Formula

kp/km

**Importance:**
Captures the relative conductivity advantage of the nanoparticle compared to the fluid.

**Feature Type:** Engineered Feature

---

## 10. Temp_Volume

**Type:** Numerical

**Description:**
Interaction feature combining temperature and particle concentration.

### Formula

Temperature × Particle Volume Fraction

**Importance:**
Represents coupled effects of temperature and nanoparticle loading.

**Feature Type:** Engineered Feature

---

## 11. Inverse_Particle_Size

**Type:** Numerical

**Description:**
Reciprocal of particle size.

### Formula

1 / Particle Size

**Importance:**
Captures nanoscale effects that may not be fully represented by raw particle size values.

**Feature Type:** Engineered Feature

---

## 12. Brownian_Feature

**Type:** Numerical

**Description:**
Engineered feature designed to represent the influence of Brownian motion on thermal transport.

**Importance:**
Brownian motion is often considered a contributing mechanism for thermal conductivity enhancement in nanofluids.

**Feature Type:** Engineered Feature

---

# Recommended Machine Learning Task

**Task Type:** Supervised Regression

**Target Variable:** TC (W/mK)

Suitable algorithms include:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost
* Support Vector Regression (SVR)
* Neural Networks
* Ensemble Learning Models

---

# Notes

* Data was compiled from multiple peer-reviewed nanofluid studies.
* Feature values were standardized and harmonized for machine learning applications.
* Several domain-informed engineered features were introduced to improve predictive modeling performance.
* Researchers are encouraged to perform additional feature selection, normalization, and exploratory analysis based on their specific use case.
