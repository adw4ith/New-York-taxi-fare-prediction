🚖 NYC Taxi Fare Prediction using Apache Spark

📘 Overview



This project analyzes the New York City Taxi Trip dataset to forecast taxi fare amounts using Apache Spark for large-scale data handling and automated learning workflows. The workflow integrates data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning model evaluation.



⚙️ Project Workflow



1\. Data Ingestion \& Cleaning

* Loaded large NYC Taxi Trip datasets using Spark DataFrames.
* Removed missing, duplicate, and invalid records.
* Converted timestamps to usable formats and encoded categorical variables.



2\. Exploratory Data Analysis (EDA)



* Identified ride volume patterns by hour and day.
* Observed strong correlations between fare amount, trip distance, and average speed.



3\. Feature Engineering



* Created new variables such as trip duration and average speed.
* Extracted temporal features from pickup and drop-off times.



4\. Modeling \& Evaluation



* Implemented and compared multiple regression models:

&nbsp;      Decision Tree Regression 

&nbsp;      Random Forest Regression

&nbsp;      Random Forest with Bagging Regression

&nbsp;      Linear Regression and Lasso Regression (as baselines)

* Tuned hyperparameters to improve performance.
* Evaluated models using RMSE, MAE, and R² metrics.



5\. Key Results



* Linear Regression slightly outperformed Lasso (R² ≈ 0.92).
* Random Forest achieved R² ≈ 0.90, showing solid non-linear performance.
* Trip distance and trip duration were the strongest predictors of fare.



🧰 Technologies Used



* Apache Spark (PySpark)



* Python (pandas, NumPy, matplotlib, seaborn)



* scikit-learn



📊 Insights



* Fare increases linearly with distance and duration.
* Ride demand peaks during rush hours and weekends.
* Simple linear models perform competitively with complex ensemble methods for this dataset.



🚀 How to Run



1. Clone this repository or open the .ipynb file in Jupyter Notebook.
2. Ensure dependencies are installed:

&nbsp;    pip install pyspark pandas numpy scikit-learn matplotlib seaborn

3\. Run the notebook cells sequentially to reproduce results.



📈 Future Improvements



* Incorporate geospatial clustering for route-based fare analysis.
* Experiment with Gradient Boosting or XGBoost models.
* Deploy the best model as an API for real-time fare prediction.
