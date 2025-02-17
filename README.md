Diamond Price Prediction

📌 Project Overview

This project aims to predict the price of diamonds using various features such as carat, cut, color, clarity, and dimensions (x, y, z). The primary objective is to build a machine learning model that accurately estimates diamond prices based on historical data. Additionally, comprehensive Exploratory Data Analysis (EDA) is performed to gain insights into the data and its relationships.


## About the Data

The dataset The goal is to predict the price of a given diamond (Regression Analysis).

There are 10 independent variables (including id):

 - id: the unique identifier of each diamond
 - carat: Carat (ct.) refers to the unique unit of weight measurement used exclusively to weigh gemstones and diamonds.
 - cut: Quality of Diamond Cut
 - color: Color of Diamond
 - clarity: Diamond clarity is a measure of the purity and rarity of the stone, graded by the visibility of these characteristics under 10-power magnification.
 - depth: The depth of the diamond is its height (in millimetres) measured from the culet (bottom tip) to the table (flat, top surface)
 - table: A diamond's table is the facet which can be seen when the stone is viewed face up.
 - x : Diamond X dimension
 - y: Diamond Y dimension
 - z: Diamond Z dimension

### Target variable: 
- price: Price of the given Diamond.

Dataset Source Link : ```https://www.kaggle.com/competitions/playground-series-s3e8/data?select=train.csv```


🕵️ Exploratory Data Analysis (EDA)

Key Insights:

Distribution of Prices:

Prices are highly skewed, with most diamonds priced under $10,000.

A few outliers exist, representing extremely high-priced diamonds.

Feature Relationships:

Higher carat values are positively correlated with higher prices.

Diamonds with an "Ideal" cut tend to have higher average prices.

Visualizations:

Price Distribution: A histogram shows the skewed nature of diamond prices.

Carat vs. Price: A scatter plot reveals a strong positive correlation.

Cut Quality vs. Price: Boxplots highlight the price differences by cut categories.

Correlation Heatmap: Displays the relationships between features and price.



🛠️ Data Handling

Handling Missing Data:

Missing values were imputed using the median or mode, depending on the feature type.

Outlier Detection:

Outliers were identified using boxplots and z-score analysis, and extreme outliers were removed to improve model performance.

Feature Encoding:

Categorical features (e.g., cut, color, clarity) were encoded using One-Hot Encoding to convert them into numerical format.

Feature Scaling:

Continuous features were scaled using StandardScaler to ensure uniform distribution.

🏗️ Model Training

Models Used:

Linear Regression: A baseline model to understand the linear relationship between features and price.

Random Forest Regressor: Chosen for its ability to handle non-linear relationships and categorical features.

XGBoost: A gradient boosting model used for its robustness and high performance.

Training Process:

The dataset was split into 80% training and 20% testing sets.

Cross-validation was performed to prevent overfitting.

Hyperparameter tuning was done using GridSearchCV to find the best model parameters.

📈 Model Evaluation

Evaluation Metrics:

R² Score: Measures the proportion of variance explained by the model.

Root Mean Squared Error (RMSE): Evaluates the average error in predictions.

Mean Absolute Error (MAE): Provides the average magnitude of prediction errors.

Performance Comparison:

Model

RMSE

R² Score

Linear Regression

1500

0.91

Decision Tree

1200

0.95

Random Forest

900

0.98

XGBoost

950

0.97

Random Forest achieved the best performance with an R² score of 0.98 and the lowest RMSE.

Visualizations:

Predicted vs. Actual Prices: A scatter plot comparing model predictions with actual prices.

Feature Importance: Bar chart showing the importance of each feature in the best-performing model.

🌟 Key Challenges

Skewed Data: Price distribution was highly skewed, requiring transformations for better model performance.

Categorical Encoding: Handling multiple categorical variables without introducing multicollinearity.

Hyperparameter Tuning: Finding the optimal parameters for complex models like Random Forest and XGBoost.





🤝 Contribution

Feel free to fork this repository, create a new branch, and submit a pull request with enhancements. Suggestions and improvements are always welcome!

📩 Contact

📌 Sanika Meghraj Erande📧 sanika.erande14@gmail.com🔗 GitHub: Sanika1422

📌 This project aims to improve diamond price prediction using machine learning techniques, enabling better decision-making in diamond pricing and valuation. 💎