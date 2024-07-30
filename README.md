# Ames Housing Price Prediction
This project involves analysing and predicting house sale prices in Ames, Iowa using a multiple linear regression model. 
The dataset used in this project was collected by the Ames City Assessor’s Office and describes 2930 property sales in Ames, Iowa between 2006 and 2010. 
The dataset, compiled and published by De Cock in 2011, contains 81 variables. 
For this project, we focused on a subset of these variables.

## Dataset Description
The dataset includes the following variables:

- **Year_Built**: The year that the house was originally constructed
- **Year_Remod_Add**: The year that the house was last remodelled
- **Total_Bsmt_SF**: Total size of basement area in square feet
- **First_Flr_SF**: Size of the first floor in square feet
- **Second_Flr_SF**: Size of the second floor in square feet
- **Gr_Liv_Area**: Size of above grade, ground living area in square feet
- **Full_Bath**: Number of full-above-grade bathrooms in the house
- **Half_Bath**: Number of half-above-grade bathrooms in the house
- **Bedroom_AbvGr**: Number of above-grade bedrooms (does not include basement bedrooms)
- **Kitchen_AbvGr**: Number of above-grade kitchens
- **TotRms_AbvGrd**: Total number of above-grade rooms (does not include bathrooms)
- **Fireplaces**: Number of fireplaces in the house
- **Garage_Area**: Size of garage in square feet
- **Sale_Price**: The sale price of the house in dollars

## Project Goal
The goal of this project was to analyse the relationship between these variables and build a multiple linear regression model to predict the sales prices based on the `Gr_Liv_Area` and `Garage_Area` variables.

## Approach
- Loading the Dataset:
The dataset was loaded into a pandas DataFrame for analysis.

- Brief Look at the Data:
The first few rows of the dataset were examined to understand its structure and the types of values it contains.

- Handling Missing Data:
Missing data in each column was identified and cleaned to ensure the dataset's integrity.

- Data Transformation and Scaling:
The underlying distribution of each column was examined to decide on the appropriate transformations and scaling methods.

- Feature Correlation Analysis:
Correlation between the features was explored using the `Seaborn pairplot` and `Seaborn heatmap` to understand the relationships between different variables.

- Feature Selection:
The most correlated features with the target variable (`Sale_Price`) were identified.

- Feature Extraction:
Dependent (`Sale_Price`) and independent features were extracted for the analysis.

- Linear Relationship Exploration:
The relationship between the dependent and each independent feature was explored to determine if it fits a linear relation.

- Outlier Removal:
Outliers from the chosen independent variables were removed to improve model performance.

- Data Splitting:
The data was split into training and test sets to evaluate the model's performance.

- Feature Scaling:
Features were scaled to ensure they were on the same scale for the regression model.

- Model Training:
A multiple linear regression model was fitted to the training data.

- Model Evaluation:
The model's performance was evaluated on the test data using the R² score.

## Results
The multiple linear regression model was successfully trained and evaluated. The performance of the model was assessed using the R² score, which measures the proportion of variance in the dependent variable that is predictable from the independent variables.

## Installation
To run the project locally, follow these steps:

- Clone the repository:
```sh
git clone https://github.com/dorsasam/ames-housing-price-prediction.git
cd ames-housing-price-prediction
```

- Create a virtual environment and activate it:
```sh
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

- Install the required dependencies:
```sh
pip install -r requirements.txt
```

- Run the Jupyter notebooks or scripts as needed.



