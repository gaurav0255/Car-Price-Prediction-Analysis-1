🚗 Car Price Prediction using Machine Learning
📌 Project Overview

This project develops a Machine Learning Regression model to predict the selling price of cars based on their technical specifications and design features. The project was built using Python and several regression algorithms to identify the key factors that influence car prices and generate accurate price predictions.

The project simulates a real-world business scenario where Geely Auto, a Chinese automobile manufacturer, plans to enter the US automobile market. Before launching its products, the company wants to understand how different vehicle characteristics influence car prices in the American market.

Through Exploratory Data Analysis (EDA), Statistical Testing, Feature Engineering, and Machine Learning, this project provides data-driven insights that can support pricing strategy, product planning, and market positioning.

🎯 Business Problem

Geely Auto intends to establish its manufacturing operations in the United States and compete with well-established American and European automobile companies.

However, the company lacks a clear understanding of:

Which vehicle features have the greatest impact on price.
How customer preferences differ between the Chinese and US markets.
How to price their vehicles competitively while maintaining profitability.

Without these insights, the company risks overpricing or underpricing its products, leading to reduced sales or lower profit margins.

🎯 Project Objective

The primary objective of this project is to build a machine learning model capable of accurately predicting car prices using vehicle specifications.

The project also aims to:

Identify the most influential factors affecting car prices.
Analyze relationships between different vehicle features and selling price.
Compare multiple regression algorithms to determine the best-performing model.
Provide actionable business insights that help manufacturers make informed pricing and product development decisions.
📊 Dataset Description

The dataset contains 205 car records with 26 features, including both numerical and categorical variables. The target variable is Price, while the remaining columns describe various technical and physical characteristics of the vehicles.

Important Features
Car Brand
Fuel Type
Aspiration
Number of Doors
Body Type
Drive Wheel
Engine Location
Wheelbase
Car Length
Car Width
Car Height
Curb Weight
Engine Type
Number of Cylinders
Engine Size
Fuel System
Bore Ratio
Stroke
Compression Ratio
Horsepower
Peak RPM
City MPG
Highway MPG

Target Variable

Price
🛠️ Technologies Used
Python
NumPy
Pandas
Matplotlib
Seaborn
SciPy
Statsmodels
Scikit-learn
🔄 Project Workflow
1. Data Understanding

The first step involved understanding the dataset, identifying numerical and categorical variables, checking data types, and studying the business meaning of each feature.

Why?

Understanding the dataset helps determine the appropriate preprocessing techniques and modeling approach.

2. Data Cleaning

The dataset was inspected for:

Missing values
Duplicate records
Incorrect data types
Data consistency

This ensured that the dataset was clean and suitable for further analysis.

3. Exploratory Data Analysis (EDA)

EDA was performed to understand the data distribution and uncover relationships between variables.

Distribution Analysis

The distribution of the target variable (Price) was examined to identify skewness and outliers.

Correlation Analysis

A correlation matrix was used to measure relationships between numerical features.

Key findings included:

Engine Size
Horsepower
Curb Weight
Car Width
Car Length

showed strong positive correlations with car price.

Features such as:

City MPG
Highway MPG

showed strong negative correlations with price, indicating that more fuel-efficient vehicles generally belonged to lower-priced segments.

4. Univariate Analysis

Each numerical feature was analyzed individually using histograms and boxplots to understand its distribution and detect skewness or potential outliers.

Categorical variables were analyzed using count plots and pie charts to understand their frequency distributions.

5. Bivariate Analysis

Relationships between variables were explored using:

Numerical vs Numerical analysis
Numerical vs Categorical analysis
Categorical vs Categorical analysis

This helped identify how different vehicle categories influence car prices.

6. Statistical Testing

ANOVA tests were performed to determine whether categorical variables significantly affected car prices.

The analysis revealed that:

Aspiration
Car Body
Drive Wheel
Engine Location
Engine Type
Fuel System
Company Name

had statistically significant impacts on car prices.

Fuel Type showed no statistically significant effect on price within this dataset.

7. Feature Engineering
Principal Component Analysis (PCA)

PCA was applied to reduce dimensionality and remove redundancy among highly correlated numerical features.

Benefits of PCA:

Reduced multicollinearity
Lower computational complexity
Improved model efficiency
Preserved maximum information with fewer features
8. Data Preprocessing

Categorical variables were transformed into numerical values using One-Hot Encoding, allowing machine learning algorithms to process them correctly.

The dataset was then divided into:

Training Set
Testing Set

to evaluate model performance on unseen data.

🤖 Machine Learning Models

Multiple regression algorithms were trained and compared.

Linear Regression

A baseline regression model used to establish a simple linear relationship between car features and price.

Decision Tree Regressor

Captures nonlinear relationships by recursively splitting the data based on feature values.

Random Forest Regressor

An ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

AdaBoost Regressor

A boosting algorithm that sequentially improves weak learners by focusing on previously mispredicted observations.

Gradient Boosting Regressor

Builds trees sequentially, where each new tree minimizes the prediction errors made by previous trees, making it highly effective for complex regression problems.

📈 Model Evaluation

The regression models were evaluated using standard regression metrics such as:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score

These metrics were used to compare model performance and identify the most accurate algorithm for predicting car prices.

📌 Key Insights

The analysis revealed several important business insights:

Engine Size is one of the strongest predictors of car price.
Horsepower has a significant positive relationship with price.
Larger and heavier vehicles generally have higher selling prices.
Premium brands command significantly higher prices.
Fuel efficiency (City MPG and Highway MPG) is negatively correlated with price.
Brand name plays a major role in determining vehicle price.
💼 Business Impact

The developed model enables automobile manufacturers to:

Predict the selling price of new vehicles before launch.
Identify the features that contribute most to pricing.
Optimize product design based on customer preferences.
Develop competitive pricing strategies.
Make data-driven decisions for entering new markets.
📁 Project Structure
Car-Price-Prediction/
│
├── CarPrice.csv                 # Dataset
├── Car_Price_Prediction.ipynb   # Jupyter Notebook
├── README.md                    # Project Documentation
├── requirements.txt             # Required Python Libraries
└── images/                      # Visualizations (Optional)
🚀 Future Improvements
Perform Hyperparameter Tuning using GridSearchCV or RandomizedSearchCV.
Evaluate advanced boosting models such as XGBoost, LightGBM, and CatBoost.
Deploy the best-performing model using Flask or FastAPI.
Create an interactive web application for real-time car price prediction.
Integrate additional market factors such as demand, resale value, and regional pricing trends.
👨‍💻 Author

Gaurav Thakur

Role: Aspiring Data Analyst | Data Science & Machine Learning Enthusiast

Skills: Python • SQL • Power BI • Machine Learning • Deep Learning • Statistics • Data Visualization
