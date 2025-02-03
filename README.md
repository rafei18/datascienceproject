# End to End Data Science Project


## Wine Quality Prediction

This project is an **end-to-end machine learning pipeline** designed to predict the quality of wine based on its physicochemical properties. It uses the **Elastic Net regression model** and provides a streamlined workflow for training, evaluation, and prediction. Additionally, a **Flask interface** enables users to interact with the model for real-time predictions.

---

## Dataset Description

The **Wine Quality** dataset contains physicochemical properties (e.g., acidity, sugar, pH) of red and white wines, along with a **quality score** ranging from 0 (worst) to 10 (best). The dataset is often used for regression and classification tasks in data science.

- **Features**: Includes attributes like acidity, residual sugar, chlorides, alcohol content, etc.
- **Target**: A quality score representing the perceived quality of the wine.
- **Source**: UCI Machine Learning Repository.

---

## Workflow Overview

The project follows a well-structured ML pipeline:

### 1. **Data Ingestion**
   - Reads the raw dataset from source files.
   - Splits the data into training and testing sets.
   - Ensures proper storage for further processing.

### 2. **Data Validation**
   - Validates dataset schema (using `schema.yaml`).
   - Checks for missing or invalid values.
   - Ensures data integrity before moving forward.

### 3. **Data Transformation**
   - **Feature Engineerin & Data Preprocessing**: Handles missing values, encodes features, and normalizes numerical data for model training.

### 4. **Model Training**
   - Trains an **Elastic Net regression model** on the preprocessed training data.
   - Hyperparameter tuning using validation data.

### 5. **Model Evaluation**
   - Evaluates the trained model using metrics such as **RMSE**, **MAE**, and **R²**.
   - Logs metrics and artifacts with **MLflow**.
   - Uses **DagsHub** for version control and experiment tracking.

### 6. **Prediction Pipeline**
   - Provides a real-time prediction service using Flask.
   - Inputs physicochemical properties and returns the predicted wine quality.

---


## Tools and Libraries

- **Programming Language**: Python
- **Key Libraries**: Scikit-learn, Pandas, NumPy, MLflow, Flask
- **Experiment Tracking**: MLflow, DagsHub
- **Model**: Elastic Net Regression
- **Deployment**: Flask API with Docker support


---

## Results and Conclusion

- The Elastic Net regression model achieved competitive performance, demonstrating its effectiveness for this task.
- Experiment tracking and versioning with **MLflow** and **DagsHub** ensured reproducibility and insights into model performance.

