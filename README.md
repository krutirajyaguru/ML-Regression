# ML-Regression

# Capital Bike Share Demand Prediction

## Overview
This project focuses on building and training a **regression model** using the **Capital Bike Share** dataset from Kaggle to predict hourly bicycle rental demand based on **time and weather conditions**. The model helps answer questions like:

> *"Given the forecasted weather conditions, how many bicycles can we expect to be rented out (city-wide) this Saturday at 2 PM?"*

The project involves data exploration, feature engineering, model training, optimization, and evaluation using **Root Mean Squared Logarithmic Error (RMSLE)**.

---

## Objectives
- **Load and explore** the Capital Bike Share dataset.
- **Split** data into training and validation sets.
- **Engineer time-based features** to improve predictions.
- **Conduct exploratory data analysis (EDA)** to understand patterns.
- **Train a regression model** to predict bike demand.
- **Optimize the model iteratively** by adjusting feature selection.
- **Apply regularization** to prevent overfitting.
- **Evaluate model performance** using **RMSLE**.

---

## Tech Stack
- **Python** - Core programming language
- **Pandas & NumPy** - Data manipulation and feature engineering
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-learn** - Model training and evaluation

---

## Dataset
The **Capital Bike Share Kaggle dataset** includes:
- **datetime**: Timestamp of rental records
- **season**: Season indicator (1 = winter, 2 = spring, etc.)
- **holiday**: Whether the day is a public holiday
- **workingday**: Whether the day is a working day
- **weather**: Weather conditions (1 = Clear, 2 = Mist, etc.)
- **temp, atemp**: Temperature-related features
- **humidity**: Humidity level
- **windspeed**: Wind speed
- **count**: Total number of bike rentals (target variable)

---

## Project Workflow
### 1. **Exploratory Data Analysis (EDA)**
- Check for missing values and data types.
- Visualize rental demand trends across different features.
- Identify correlations between features and target variable.

### 2. **Feature Engineering**
- Extract **hour, day, month, and year** from the `datetime` column.
- Convert categorical variables like **season and weather** using **one-hot encoding**.
- Create new features such as **weekday/weekend indicators**.

### 3. **Data Splitting**
- Split the dataset into **training** (80%) and **validation** (20%) sets.
- Ensure time-based splitting to avoid data leakage.

### 4. **Train a Regression Model**
- Train an initial **Linear Regression** model.
- Evaluate performance using **RMSLE**.

### 5. **Model Optimization**
- Experiment with additional features (e.g., lag features, interaction terms).
- Tune hyperparameters and select the best feature subset.

### 6. **Regularization & Overfitting Prevention**
- Train models with **Ridge and Lasso regression** to prevent overfitting.
- Compare performance of different models.

### 7. **Model Evaluation**
- Calculate **RMSLE** for both training and validation sets.
- Analyze model residuals to check prediction errors.

---

## Results & Learnings
- Discovered key factors influencing bike rentals.
- Learned **feature engineering** techniques for time-series data.
- Compared performance of **Linear Regression, Ridge, and Lasso models**.
- Understood how **regularization** improves model generalization.

---

## License
This project is licensed under the MIT License.
