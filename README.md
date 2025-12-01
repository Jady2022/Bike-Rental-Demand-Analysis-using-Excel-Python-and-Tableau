### Tools & Technologies

| Category | Tools |
|---------|--------|
| **Data Analysis** | Excel (Regression, ANOVA, VIF, variable selection) |
| **Programming** | Python (Prophet, Holt-Winters, Matplotlib, Statsmodels, Pandas) |
| **Visualization** | Tableau Desktop (.twbx) |

---

### Key Analyses & Findings

#### **1. Regression Analysis (Excel + Python)**
- Strong seasonality and weather-driven demand patterns.
- `temp`, `workingday`, and `weathersit` are key predictors of total rentals.
- Removed due to multicollinearity:
  - `atemp` (highly redundant with `temp`)
  - `instant` (meaningless serial index)

Model achieved **Adjusted R² ≈ 0.998**, indicating high explanatory power.


#### **2. Time Series Forecasting (Python)**

##### **Prophet Model**
- Captures seasonality and weekly patterns.
- **MAE ≈ 1613**, **RMSE ≈ 1905**, **R² ≈ 0.46** (holiday anomalies reduce accuracy)

##### **Holt-Winters Model**
- Uses additive trend/seasonality.
- **MAE ≈ 2362**, **RMSE ≈ 7108**, **R² ≈ 0.99**

➡ Prophet performed better but still struggled due to irregular short-term fluctuations.


#### **3. Tableau Insights**
Includes:
- Seasonal rental patterns  
- Working vs. non-working day comparison  
- Weather sensitivity  
- Registered vs. casual user distribution  

Insight: **Bike rentals spike on working days → strong commuter-driven usage.**


### Business Recommendations

Based on regression + forecasting + Tableau insights:

- Increase bike availability during **clear-weather weekdays**.
- Reduce staffing or reallocate bikes on **cold/winter days**.
- Use **dynamic pricing** for extreme temperature periods.
- Schedule **maintenance during seasonal lows**.
- Deploy more bikes in **office zones during commuting hours**.


### Dataset Information & License

This project uses the **Bike Sharing Dataset** from the  
**UCI Machine Learning Repository**.

#### **Cite the following publication when using this dataset:**

Fanaee-T, Hadi, and Gama, João.  
“Event labeling combining ensemble detectors and background knowledge.”  
*Progress in Artificial Intelligence* (2013): 1–15.  
https://doi.org/10.1007/s13748-013-0040-3

@article{
year={2013},
issn={2192-6352},
journal={Progress in Artificial Intelligence},
doi={10.1007/s13748-013-0040-3},
title={Event labeling combining ensemble detectors and background knowledge},
url={http://dx.doi.org/10.1007/s13748-013-0040-3}
,
publisher={Springer Berlin Heidelberg},
keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
author={Fanaee-T, Hadi and Gama, Joao},
pages={1-15}
}


---

### 👤 Author

**Ruocheng Jiang**
Master’s in Business Analytics @ UT Dallas
Skills: Data Analysis • Python • Tableau • Excel Modeling
LinkedIn: *(optional)*

---

### Summary

This project demonstrates a full end-to-end analytics workflow:

* Data understanding
* Regression modeling
* Time series forecasting
* Business interpretation
* Visualization
* Documentation & reproducibility

Ideal for demonstrating analytical thinking, technical skill, and business understanding.

```
