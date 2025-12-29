# Bankruptcy-Prediction-using-Autogluon
3rd Place Solution for Kaggle Bankruptcy Prediction Competition using AutoGluon and Weighted Ensembles.

🏆 3rd Place Solution: Corporate Bankruptcy Prediction
This repository contains the winning strategy for the MGMT 571 Data Mining Kaggle competition. Our team, Neural Nomads, achieved a private score of 0.9231 by leveraging automated machine learning and advanced feature engineering.

🚀 Key Highlights
Rank: 3rd out of 37 teams.
Core Model: AutoGluon Weighted Ensemble.
Primary Metric: High ROC-AUC for ranking financial risk.
🛠️ The Strategy
1. Data Preprocessing
Financial data is often skewed. We implemented:

- Infinite Value Handling: Replaced inf values with NaN to stabilize training.
- arcsinh Transformation: Used the Inverse Hyperbolic Sine transformation to reduce skewness and handle extreme outliers without losing signal.
  
2. The Modeling Pipeline
We utilized AutoGluon to run a "champion-challenger" tournament across multiple algorithms:

- Gradient-Boosted Trees (LightGBM, CatBoost, XGBoost)
- Deep Neural Networks
- Random Forests
  
3. Validation
To ensure the model was robust, we used a 5-fold cross-validation split, repeated 20 times. This ensured our high accuracy was consistent across different subsets of data.

📁 Repository Structure
notebooks/: Contains the full Python implementation.
presentation/: The final deck explaining the business logic and insights.

👨‍🏫 Acknowledgments
Special thanks to Will Wei Sun for leading the MGMT 571 course and providing the guidance to bridge theory and practice.

Team Neural Nomads: Satish, Sana Majeed, and Iscel Manalo.
