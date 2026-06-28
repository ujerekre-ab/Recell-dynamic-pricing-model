# Recell-dynamic-pricing-model
An end-to-end machine learning regression pipeline built to automate and optimize resale price valuations for used and refurbished electronic devices.

## Business Objective
Develop a predictive model that dynamically estimates the optimal resale price of refurbished devices. By analyzing hardware specifications, historical market trends, and product degradation metrics, the model maximizes profit margins while maintaining marketplace competitiveness.

## Dataset Overview
- Number of observations: 3454
- Number of features: 49
- Target Variable: Price
- Industry: Consumer Electronics

## Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Statistical Modeling:** Statsmodels
* **Data Visualization:** Matplotlib, Seaborn

## Business Questions
- What factors most strongly influence resale value?
- How much does device age affect price?
- Does brand reputation justify premium pricing?
- Can machine learning improve pricing consistency over manual methods?
  
## Skills Demonstrated
- Data Cleaning
- Feature Engineering
- Statistical Analysis
- Regression Modeling
- Machine Learning
- Model Validation
- Data Visualization
- Python
- Pandas
- Scikit-Learn
- Statsmodels
  
## Feature Engineering & Predictors
To maximize the predictive power of the model, the feature matrix utilizes:
* **Hardware Tiering:** Processor specifications, RAM, storage capacities, and screen dimensions.
* **Temporal Decay:** Mathematical age of the device from its original market release date.
* **Brand equity:** Categorical encoding of brand tiers based on historical market premiums.
* **Market Dynamics:** Historical baseline transactional pricing data.

## Technical Workflow & Statistical Execution

### 1. Data Pipeline & Preprocessing
* Handled structural anomalies, missing values, and encoded high-cardinality categorical features (Brands/Specs) using target/one-hot encoding.
* Transformed skewed numeric distributions using logarithmic scaling to stabilize variance.

### 2. Exploratory Data Analysis (EDA)
* Conducted correlation matrices to isolate strong non-linear relationships between device degradation and price decay.
* Evaluated feature importance metrics to eliminate redundant architectural variables.

### 3. Rigorous Statistical Diagnostics (Statsmodels)
* Conducted validation checks on classical Linear Regression assumptions [1].
* Evaluated **Multicollinearity** using Variance Inflation Factors (VIF) to remove highly correlated predictors [1].
* Tested for **Heteroscedasticity** and residual normality to ensure stable error variances across price tiers [1].

### 4. Regression Modeling & Evaluation
* Developed and tuned Linear Regression architectures alongside regularized variants via Scikit-learn.
* Evaluated model generalization using structural metrics: **R-squared (R²)**, **Root Mean Squared Error (RMSE)**, and **Mean Absolute Error (MAE)**.

## Model Performance & Business Impact

### Test Set Validation Metrics
The model demonstrated strong generalization capabilities on unseen testing data, demonstrating strong predictive performance on unseen test data and potential applicability to pricing decision support.
* **Coefficient of Determination ($R^2$ Score):** **0.829191** — The engineered features successfully explain **82.9%** of the variance in device pricing.
* **Root Mean Squared Error (RMSE):** **0.241178** — Indicates a highly constrained error margin, ensuring tight, reliable automated pricing valuations.

### Core Analytical Insights
* **The Decay Factor:** Device age demonstrated a severe, non-linear negative correlation with price, serving as the heaviest statistical weight in the valuation matrix.
* **Brand Premium Quantification:** Brand reputation was a significant predictor of resale value, with premium brands consistently retaining higher market prices. allowing for automated margin inflation on premium stock.
* **Operational Accuracy:** Transitioning from manual pricing rules to this ML-driven approach minimizes human valuation errors and optimizes inventory turnover speeds.

## Diagnostic & Performance Plots
<img width="1585" height="262" alt="Screenshot 2026-05-27 153706" src="https://github.com/user-attachments/assets/fba37bb0-6cc1-4494-96bf-cbad58dc9a6e" />

<img width="589" height="463" alt="download" src="https://github.com/user-attachments/assets/90ecbbec-222d-46fc-b7d0-a8fd19ef5c84" />

<img width="1795" height="813" alt="Screenshot (55)" src="https://github.com/user-attachments/assets/686c7d83-01db-45a7-8138-260e2fddf7e0" />

<img width="1742" height="161" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/16d7abc8-548f-49ac-a781-b58fbf14921b" />

<img width="1732" height="684" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/e0e5780a-1d9d-4290-95eb-95217adaf016" />
