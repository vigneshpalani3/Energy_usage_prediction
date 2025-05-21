⚡ Energy Usage Prediction
This project focuses on predicting household energy consumption using machine learning techniques. By leveraging historical energy usage data, the goal is to develop models that can accurately forecast future energy demands, aiding in efficient energy management and planning.

📁 Repository Structure
Data_preprocessing.ipynb: Notebook dedicated to data cleaning, feature engineering, and exploratory data analysis.

model_building.ipynb: Notebook for training and evaluating machine learning models.

📊 Dataset
The dataset utilized is the Individual Household Electric Power Consumption Data Set from the UCI Machine Learning Repository.

Dataset Details:

Duration: December 2006 to November 2010.

Frequency: 1-minute intervals.

Features:

Global_active_power: Household global minute-averaged active power (kilowatts).

Global_reactive_power: Household global minute-averaged reactive power (kilowatts).

Voltage: Minute-averaged voltage (volts).

Global_intensity: Minute-averaged current intensity (amperes).

Sub_metering_1: Energy sub-metering No. 1 (watt-hours).

Sub_metering_2: Energy sub-metering No. 2 (watt-hours).

Sub_metering_3: Energy sub-metering No. 3 (watt-hours).

🛠️ Methodology
1. Data Preprocessing
Handling Missing Values: Identified and addressed missing entries to ensure data integrity.

Feature Engineering: Extracted temporal features such as hour, day, and month to capture time-based consumption patterns.

Normalization: Applied scaling techniques to standardize the feature set.

2. Model Building
Linear Regression:

Validated using 5-fold cross-validation to assess model stability.

Random Forest Regressor:

Hyperparameters tuned using RandomizedSearchCV to optimize performance given the large dataset size.

3. Evaluation Metrics
R² Score: Measures the proportion of variance explained by the model.

Mean Squared Error (MSE): Penalizes larger errors more significantly.

Mean Absolute Error (MAE): Provides the average magnitude of errors.

📈 Results
Model	R² Score	MSE	MAE
Linear Regression	0.99	0.001	0.02
Random Forest	0.99	0.003	0.03


🙏 Acknowledgements
Dataset sourced from the UCI Machine Learning Repository.

Utilized libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn.
