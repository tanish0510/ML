# 🌽 Spectral Data Analysis for DON Concentration Prediction

## 📌 Overview
This project aims to analyze **spectral data** and predict **Deoxynivalenol (DON) concentration** using **Machine Learning (ML) techniques**. The workflow includes **data preprocessing, feature scaling, dimensionality reduction (PCA & t-SNE), model training using Random Forest, and evaluation using MAE, RMSE, and R² score**.

## 📂 Dataset
- The dataset (`TASK-ML-INTERN.csv`) contains spectral features and DON concentration values.
- The **target variable** is the DON concentration.

## ⚙️ Preprocessing Steps
1. **Missing Values Handling**: Checked for missing values and handled them appropriately.
2. **Feature Scaling**: Used `StandardScaler` to normalize spectral data for better model performance.
3. **Outlier Detection**: Used boxplots to detect and visualize outliers.
4. **Univariate & Bivariate Analysis**:
   - Histograms & KDE plots for feature distributions.
   - Correlation heatmap for feature relationships.

## 📊 Dimensionality Reduction
- **PCA (Principal Component Analysis)**:
  - Reduced the dataset to 2 components.
  - Explained variance ratio observed.
  - Scatter plot visualization.

### PCA Visualization
![RESULTS](https://github.com/tanish0510/ML/blob/main/image.png)
  
- **t-SNE (t-Distributed Stochastic Neighbor Embedding)**:
  - Visualized high-dimensional data in a 2D space.
  - Highlighted clustering patterns.

 ### t-SNE Visualization
![RESULTS](https://github.com/tanish0510/ML/blob/main/tsne.png)

## 🏗️ Model Training
- **Algorithm Used**: `RandomForestRegressor`
- **Hyperparameters**: `n_estimators=100, random_state=42`
- **Cross-Validation**: Implemented **k-fold cross-validation** for better generalization.

## 📈 Model Evaluation
- **Mean Absolute Error (MAE)**: `3765.0568`
- **Root Mean Squared Error (RMSE)**: `≈ High`
- **R² Score**: `≈ Low`

> **Key Insight**: The model needs improvement due to a high error rate. Possible solutions include:
> - Trying **different models** (e.g., XGBoost, Gradient Boosting).
> - Performing **feature selection** to remove irrelevant features.
> - **Hyperparameter tuning** using Grid Search or Bayesian Optimization.

## 📌 Visualizations
- **Feature Distributions** (Histograms, KDE plots)
- **PCA & t-SNE Scatter Plots**
- **Correlation Heatmap**
- **Actual vs Predicted Scatter Plot**

 ## Result Visualization
![RESULTS](https://github.com/tanish0510/ML/blob/main/result.png)

## 🚀 Future Improvements
- Implement more **advanced ML models** for better accuracy.
- Use **Deep Learning (ANNs, CNNs)** for spectral feature learning.
- Optimize hyperparameters using **Grid Search / Bayesian Optimization**.
- Explore **domain-specific feature engineering**.

## 🛠️ Installation & Usage
1. **Clone the Repository**
   ```bash
   git clone https://github.com/tanish0510/ML
   cd ML
```
