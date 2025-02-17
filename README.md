# 💎 Diamond Price Prediction

## 📌 Project Overview

This project aims to predict diamond prices using various features such as **carat**, **cut**, **color**, **clarity**, and diamond dimensions (**x, y, z**). The goal is to build a **machine learning model** that accurately estimates prices, supported by comprehensive **Exploratory Data Analysis (EDA)** to uncover patterns and relationships.

---

## 📊 About the Data

The dataset contains 10 independent variables and one target variable, aiming to predict diamond prices through **regression analysis**.

### 🔍 Independent Variables:

- **id**: Unique identifier for each diamond.
- **carat**: Unit of weight for gemstones and diamonds.
- **cut**: Quality of the diamond cut.
- **color**: Diamond color grade.
- **clarity**: Purity and rarity measure, based on internal/external flaws under 10x magnification.
- **depth**: Height of the diamond (culet to table), expressed as a percentage.
- **table**: Width of the diamond’s top flat facet when viewed face up.
- **x**: Length of the diamond (in millimeters).
- **y**: Width of the diamond (in millimeters).
- **z**: Height of the diamond (in millimeters).

### 🎯 Target Variable:

- **price**: The price of the given diamond, which the model aims to predict.

### 📥 Dataset Source:
[Kaggle Playground Series S3E8](https://www.kaggle.com/competitions/playground-series-s3e8/data?select=train.csv)

---

## 🕵️ Exploratory Data Analysis (EDA)

### Key Insights:

1. **Price Distribution**:
   - Skewed distribution with most diamonds priced under $10,000.
   - A few high-priced outliers.

2. **Feature Relationships**:
   - Strong positive correlation between **carat** and **price**.
   - Diamonds with "Ideal" cuts generally have higher prices.

### 🔍 Visual Insights:

1. **Price Distribution**: Histogram showing skewed price distribution.
2. **Carat vs. Price**: Scatter plot revealing a strong positive correlation.
3. **Cut Quality vs. Price**: Boxplots highlighting price differences by cut categories.
4. **Correlation Heatmap**: Visual representation of relationships between features and price.

---

## 🛠️ Data Handling

### 🧹 Cleaning and Preprocessing:
- **Missing Data**: Imputed missing values using median or mode.
- **Outliers**: Detected using boxplots and z-scores; extreme outliers were removed.

### 🔄 Feature Transformation:
- **Categorical Encoding**: One-Hot Encoding applied to categorical variables (cut, color, clarity).
- **Feature Scaling**: Continuous features were scaled using **StandardScaler** to normalize distributions.

---

## 🏗️ Model Training

### ⚙️ Models Used:

1. **Linear Regression**: Baseline model for understanding linear relationships.
2. **Random Forest Regressor**: Handles non-linear relationships effectively.
3. **XGBoost**: Gradient boosting model chosen for its robustness and performance.

### 🔍 Training Process:
- **Train-Test Split**: 80% training, 20% testing.
- **Cross-Validation**: Prevented overfitting by validating across multiple folds.
- **Hyperparameter Tuning**: Used **GridSearchCV** to optimize model parameters.

---

## 📈 Model Evaluation

### 📊 Evaluation Metrics:

- **R² Score**: Measures the proportion of variance explained by the model.
- **Root Mean Squared Error (RMSE)**: Evaluates the average prediction error.
- **Mean Absolute Error (MAE)**: Provides the average magnitude of errors.

### 📌 Performance Comparison:

| Model             | RMSE    | R² Score |
| ----------------- | ------- | -------- |
| Linear Regression | 1500    | 0.91     |
| Decision Tree     | 1200    | 0.95     |
| Random Forest     | **900** | **0.98** |
| XGBoost           | 950     | 0.97     |

- **Random Forest** achieved the best performance, with an R² score of **0.98** and the lowest RMSE.

### 🔍 Visual Comparisons:

1. **Predicted vs. Actual Prices**: Scatter plot comparing model predictions to actual prices.
2. **Feature Importance**: Bar chart showing the importance of each feature in the best-performing model.

---

## 🌟 Key Challenges and Solutions

1. **Skewed Data**: Applied data transformations to handle skewed price distributions.
2. **Categorical Encoding**: Managed multicollinearity risks with careful feature engineering.
3. **Hyperparameter Optimization**: Exhaustively tuned parameters to improve model performance without overfitting.

---

## 🤝 Contribution

Feel free to **fork** this repository, create a new branch, and submit a pull request with enhancements. Suggestions and improvements are always welcome!

---

## 📩 Contact

📌 **Sanika Meghraj Erande**  
📧 [sanika.erande14@gmail.com](mailto:sanika.erande14@gmail.com)  
🔗 **GitHub:** [Sanika1422](https://github.com/Sanika1422)

---

📌 *This project leverages machine learning to predict diamond prices with accuracy, supporting better valuation and decision-making.* 💎

