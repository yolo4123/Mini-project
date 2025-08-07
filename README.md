# Mini-project
Mini Project: Agricultural Price Prediction

This project applies various machine learning models to predict modal prices of agricultural commodities using market data. The workflow includes data preprocessing, exploratory analysis, and regression modeling with multiple algorithms.

Dataset

The dataset contains agricultural market information with features such as:

State Name
District Name
Market Name
Variety
Group
Arrival Tonnes
Minimum Price (Rs/Quintal)
Maximum Price (Rs/Quintal)
Modal Price (Rs/Quintal)
Reported Date
Commodity Name
Data is loaded from agridata_202207142054.xlsx.

Workflow

Import Libraries
Uses pandas, numpy, and machine learning modules from scikit-learn.

Data Loading & Inspection
Loads the dataset and inspects first few rows.

Missing Value Handling

Checks for missing values.
Drops or fills missing values appropriately.
Feature Engineering & Preprocessing

Converts reported_date to datetime.
Extracts Year and Month features.
Encodes categorical variables.
Scales numerical features.
Train/Test/Validation Split

Splits data into training, validation, and test sets using an 80/20 split and further 75/25 for validation.
Modeling
Models implemented:

Linear Regression
Random Forest Regressor
Decision Tree Regressor
K-Nearest Neighbors (KNN) Regressor
Ridge Regression
Each model is evaluated using:

Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Mean Absolute Error (MAE)
R² Score
Results

The notebook prints metrics for training, validation, and test sets for each model.
Random Forest and Decision Tree models typically achieve the best performance.
Ridge Regression is tested for regularization effects.
How to Run

Clone the repository.
Ensure you have the required packages:
bash
pip install pandas scikit-learn numpy
Place the dataset (agridata_202207142054.xlsx) in the working directory.
Open Mini_Project.ipynb in Jupyter Notebook or Google Colab.
Run the notebook cells sequentially.
File Structure

Code
Mini-project/
├── Mini_Project.ipynb
├── agridata_202207142054.xlsx
└── README.md
Credits

Developed by yolo4123.

Feel free to modify this README as you see fit! If you want to add usage examples, model comparison plots, or more details, let me know.
