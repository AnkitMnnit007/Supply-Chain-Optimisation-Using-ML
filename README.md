# Supply Chain Optimisation Using Machine Learning
A machine learning project that predicts **weekly retail sales** using historical sales data, store characteristics, promotional activities, holidays, and seasonal factors. The project uses **Random Forest Regression** to identify key sales drivers and support data-driven inventory and supply chain decisions.

**Author:** Ankit Kumar

**College:** MNNIT Allahabad

---

## Project Overview

The goal of this project is to optimize supply chain operations by accurately predicting weekly sales for different retail stores.

A **RandomForestRegressor** model is trained on historical sales data along with store information, promotional activities, holidays, and other external factors. The project also includes exploratory data analysis, feature engineering, model evaluation, feature importance analysis, and interactive visualizations.

The insights generated can help businesses with:

* Inventory planning
* Demand forecasting
* Sales analysis
* Store performance evaluation
* Supply chain decision-making

---

## Objectives

The main objectives of this project are:

1. Predict **Weekly Sales** for retail stores using historical data.
2. Identify the key factors influencing store sales.
3. Analyze sales trends and seasonal patterns.
4. Evaluate the performance of the machine learning model.
5. Generate insights that can support inventory and supply chain planning.

---

## Dataset

The project uses four datasets:

### 1. Features.csv

Contains additional information related to stores, including:

* Promotional activities
* Holidays
* Temperature
* Fuel prices
* Consumer Price Index
* Unemployment

### 2. Stores.csv

Contains store-level information such as:

* Store Type
* Assortment Type

### 3. Train.csv

Contains historical sales data used for training the machine learning model, including:

* Store
* Date
* Weekly Sales
* Holiday information

### 4. Test.csv

Contains data used to evaluate the model's predictive performance.

---

## Project Workflow

### Step 1: Data Loading

The datasets were loaded using **Pandas** and combined to create a unified dataset containing store, sales, promotional, and external information.

### Step 2: Data Preprocessing

The following preprocessing steps were performed:

* Merged the `Features`, `Stores`, and `Train` datasets.
* Handled missing values using median imputation for numerical features and mode imputation for categorical features.
* Extracted date-based features such as:

  * Year
  * Month
  * Week
  * Day
  * Day of Week
* Encoded categorical variables using one-hot encoding.
* Prepared the processed dataset for machine learning.

### Step 3: Exploratory Data Analysis

Exploratory analysis was performed to understand:

* Sales trends over time
* Sales distribution across store types
* Seasonal patterns
* Relationships between store characteristics and sales
* Factors influencing weekly sales

### Step 4: Feature Engineering

Additional features were created from the existing data to improve model performance and provide better insights into sales patterns.

Key engineered features include:

* Year
* Month
* Week
* Day
* Day of Week
* Encoded categorical variables

### Step 5: Model Training

A **RandomForestRegressor** from Scikit-learn was used to predict `Weekly_Sales`.

The model learns relationships between historical sales, store characteristics, promotional activities, seasonal factors, and other features.

### Step 6: Model Evaluation

The model was evaluated using:

**Mean Squared Error (MSE)**
Measures the average squared difference between actual and predicted sales.

**R² Score**
Measures how much of the variation in weekly sales is explained by the model.

### Step 7: Feature Importance Analysis

Feature importance was analyzed using the trained Random Forest model to identify the variables that contributed most to sales predictions.

The analysis helps identify important sales drivers such as:

* Promotional activities
* Store type
* Seasonal factors
* Holiday effects
* External economic factors

### Step 8: Data Visualization

Visualizations were created using **Seaborn, Matplotlib, and Plotly**.

Key visualizations include:

* Weekly Sales Trend Over Time
* Sales Distribution by Store Type
* Feature Importance
* Seasonal Sales Patterns

---

## Technologies & Tools

### Programming Language

* Python

### Data Analysis & Preprocessing

* Pandas
* NumPy

### Machine Learning

* Scikit-learn
* Random Forest Regression

### Data Visualization

* Matplotlib
* Seaborn
* Plotly

---

## Project Structure

```text
Supply_Chain_Optimisation_using_ml/
│
├── Features.csv
├── Stores.csv
├── Train.csv
├── Test.csv
├── Supply_Chain_Opt.py
├── README.md
└── requirements.txt
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/KUN10SINGH/Supply_Chain_Optimisation_using_ml.git
```

### Navigate to the Project Directory

```bash
cd Supply_Chain_Optimisation_using_ml
```

### Install the Required Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly
```

---

## Usage

1. Clone the repository.
2. Place the required datasets in the appropriate directory.
3. Install the required Python libraries.
4. Run the Python script:

```bash
python Supply_Chain_Opt.py
```

The script performs:

* Data preprocessing
* Feature engineering
* Exploratory data analysis
* Model training
* Model evaluation
* Feature importance analysis
* Data visualization

---

## Results

The **Random Forest Regression** model was used to predict weekly retail sales.

The model performance was evaluated using:

* **Mean Squared Error (MSE)**
* **R² Score**

Feature importance analysis provided insights into the factors contributing to weekly sales predictions, including promotional activities, store characteristics, and seasonal patterns.

These insights can be used to support:

* Demand forecasting
* Inventory planning
* Store-level sales analysis
* Supply chain optimization

---

## Future Improvements

The project can be further improved through:

### Hyperparameter Tuning

Optimize Random Forest parameters such as:

* Number of trees
* Maximum tree depth
* Minimum samples per split
* Maximum features

### Advanced Machine Learning Models

Experiment with additional models such as:

* XGBoost
* Gradient Boosting
* LightGBM
* CatBoost

### Additional Features

Incorporate external factors such as:

* Economic indicators
* Regional events
* Weather information
* Competitor information
* Regional demand patterns

### Supply Chain Optimization

Use the predicted sales to develop optimization strategies for:

* Inventory allocation
* Demand planning
* Stock replenishment
* Store-level inventory management

---

## Author

**Ankit Kumar**
**MNNIT Allahabad**
Machine Learning & Data Analytics Enthusiast
