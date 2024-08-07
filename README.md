**Crop-Yield Prediction
Project Overview**
This project aims to predict crop yields based on various factors such as rainfall, pesticide usage, temperature, and area. The dataset includes features like the year, average rainfall, pesticide usage, average temperature, area, crop type, and yield per hectare.

**Dataset**
The dataset consists of the following columns:

**Year**: Year of the data record
**average_rain_fall_mm_per_year**: Average rainfall in millimeters per year
**pesticides_tonnes**: Amount of pesticides used in tonnes
**avg_temp**: Average temperature
**Area**: Area of cultivation
**Item**: Type of crop
**hg/ha_yield**: Yield per hectare

**Steps Involved**

**1. Data Preprocessing**
Checked for Null Values: Verified the dataset for any missing values and handled them appropriately.
**Data Visualization:**
Count Plot with Area: Visualized the distribution of data across different areas.
Bar Plot with Country and Yield per Country: Analyzed yield distribution across different countries.
Bar Plot between Crops and Yield per Crop: Examined the yield distribution across different crop types.

**2. Feature Engineering**

Encoding Categorical Variables: Converted categorical variables such as area and crop type into numerical format using encoding techniques.
Scaling the Values: Applied scaling to normalize the feature values for better model performance.

**3. Model Training**

Train-Test Split: Split the dataset into training and testing sets to evaluate model performance.
Model Selection: Trained multiple regression models, including:
Linear Regression
Lasso Regression
Ridge Regression
K-Nearest Neighbors (KNN)
Decision Tree Regressor

**4. Model Evaluation**

Mean Absolute Error (MAE): Calculated the MAE for each model to measure the average magnitude of errors.
R² Score: Calculated the R² score for each model to assess how well the independent variables explain the variability of the dependent variable (yield).

**5. Model Selection**

Selected the Decision Tree Regressor as the final model based on its superior performance in terms of MAE and R² score.

**6. Prediction on New Data**

Tested the selected model on new data points and obtained accurate predictions, validating the model's effectiveness.

**Results**
The model evaluation results for different algorithms were as follows:

**Linear Regression**: MAE = 29907.53512614917, R² Score = 0.7473117803683427
**Lasso Regression**: MAE = 29893.99762450549, R² Score = 0.7473261756207235
**Ridge Regression**: MAE = 29864.88375663324, R² Score = 0.7473044447803092
**Decision Tree Regressor**: MAE = 3817.598419124735, R² Score = 0.9808630051556833

**The Decision Tree Regressor was selected as the final model due to its best performance.**

**Visualizations**

Several visualizations were created to understand the data distribution and feature relationships:

**Count Plot with Area**: Showed the distribution of data across different areas.
**Bar Plot with Country and Yield per Country**: Highlighted the yield distribution across different countries.
**Bar Plot between Crops and Yield per Crop**: Displayed the yield distribution across different crop types.

**Conclusion**

The Decision Tree Regressor model demonstrated excellent performance in predicting crop yields based on the provided features. The model's accurate predictions on new data points further validate its effectiveness. Future work may involve experimenting with more advanced machine learning models and feature selection techniques to enhance performance.
