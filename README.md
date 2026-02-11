🏠 Tehran House Price Prediction
📌 Project Overview
This project focuses on exploratory data analysis (EDA) and machine learning–based price prediction for residential houses in Tehran.

The goal is to analyze the factors affecting house prices and compare multiple regression models to find the most accurate predictor.

📊 Dataset Description
The dataset contains information about residential properties in Tehran, including:

Area (square meters)
Number of Rooms
Address (Location)
Parking
Warehouse
Elevator
House Price
Missing values were handled, data types were corrected, and categorical features were properly encoded.

🔍 Exploratory Data Analysis (EDA)
The following analyses were performed:

Handling missing and invalid values
Distribution analysis of house prices
Correlation analysis between numerical features
Outlier detection using IQR method
Location-based price comparison
Visualization of amenities (Parking, Warehouse, Elevator)
Automated data profiling using ydata-profiling
📈 Libraries used for visualization:

Matplotlib
Seaborn
⚙️ Data Preprocessing
Converted boolean features to numerical format
One-hot encoding applied to Address
Feature scaling handled implicitly by model selection
Train-test split (80% / 20%)
🤖 Machine Learning Models
Multiple regression models were trained and compared using GridSearchCV and K-Fold cross-validation:

Linear Regression
Ridge Regression
Lasso Regression
Elastic Net
Decision Tree Regressor
Random Forest Regressor
K-Nearest Neighbors Regressor
XGBoost Regressor
📐 Evaluation Metrics
R² Score (Train & Test)
Root Mean Squared Error (RMSE)
A custom parameter_finder function was implemented to:

Tune hyperparameters
Evaluate performance
Measure runtime
🏆 Results
Ensemble and tree-based models (Random Forest & XGBoost) achieved the best performance.
Linear models showed lower accuracy but better interpretability.
Overfitting was monitored by comparing train and test scores.
🛠️ Technologies & Libraries
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
XGBoost
ydata-profiling
🚀 How to Run
bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost ydata-profiling
Open the notebook:

bash
jupyter notebook tehranhouses.ipynb
📌 Future Improvements
Feature scaling for distance-based models
Geographical encoding of locations
Time-based price trend analysis
Deployment as a web application
