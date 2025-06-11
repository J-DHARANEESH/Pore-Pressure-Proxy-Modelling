# Pressure Prophet : Pore Pressure Proxy Modeling

This repository contains a machine learning project aimed at modeling **pore pressure proxies** using well log facies data. The project uses geological and petrophysical features from the Well Log Facies Dataset to build regression models that predict synthetic pore pressure values derived from well log measurements.

---

## Project Overview

Accurate estimation of pore pressure is critical in subsurface geological studies and drilling operations. However, direct pore pressure measurements are often unavailable or costly. This project demonstrates how well log data can be leveraged to predict a **pore pressure proxy**—a synthetic estimate based on petrophysical logs—using various machine learning regression techniques.

---

## Dataset

* **Source:** Well Log Facies Dataset (Kaggle)
* **Features:** Gamma Ray (GR), Resistivity (ILD\_log10), Photoelectric Effect (PE), Porosity (DeltaPHI, PHIND), Lithology indicators (NM\_M, RELPOS), and more.
* **Target:** Simulated pore pressure proxy constructed from the well log features.

---

## Methodology

1. **Data Preprocessing:** Handling missing values, feature scaling, and exploratory data analysis.
2. **Feature Engineering:** Using key well log measurements relevant to pore pressure.
3. **Proxy Generation:** Creating a synthetic pore pressure proxy as the prediction target.
4. **Model Training:** Training and evaluating multiple regression models.
5. **Performance Evaluation:** Comparing models using Mean Squared Error (MSE) and R² score.
6. **Visualization:** Pair plots, correlation heatmaps, and residual analysis.

---

## Models Used

The project implements and compares the following regression models:

* **Linear Regression:** Baseline linear model.
* **Ridge Regression:** Linear model with L2 regularization to reduce overfitting.
* **Random Forest Regressor:** Ensemble of decision trees to capture nonlinear relationships.
* **Support Vector Regression (SVR):** Uses kernels for regression in high-dimensional space.
* **XGBoost Regressor:** Gradient boosting method for high-performance regression.

---

## Results

* Ridge Regression and Linear Regression models achieved the best performance with MSE \~0.01 and R² \~0.998.
* Other models like Random Forest and XGBoost performed moderately well but with higher error.
* This highlights the potential of well log data to approximate pore pressure proxies effectively.

---

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/pore-pressure-proxy-modeling.git
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:

   ```bash
   jupyter notebook PorePressureProxyModeling.ipynb
   ```

---

## Requirements

* Python 3.x
* pandas
* numpy
* seaborn
* matplotlib
* scikit-learn
* xgboost

---

## Future Work

* Incorporate real pore pressure data to validate and refine models.
* Apply hyperparameter tuning and advanced ensemble methods.
* Expand feature engineering with domain-specific geological inputs.
* Deploy as a predictive tool integrated into drilling workflows.


---

## Contact

For questions or collaboration, please reach out:
**Email:** j.dharaneesh12@gmail.com<br>
**GitHub:** https://github.com/J-DHARANEESH

---
