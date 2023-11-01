# Ridge-Regression-and-LASSO-using-R

## Overview
This project involves analyzing a dataset of residential buildings to predict two key financial aspects: the "Actual Sales Price" and the "Actual Construction Cost". The analysis is conducted using Ridge Regression and LASSO (Least Absolute Shrinkage and Selection Operator), two popular regularization techniques in linear regression. The project is implemented in R, utilizing various libraries for data manipulation, modeling, and visualization.

## Data Description
The dataset, named "Residential Building Data Set", comprises various attributes of residential buildings constructed in different regions of Iran. The data includes numerous predictor variables, such as the total floor area, lot area, and preliminary estimated construction costs. These predictors are used to model and predict the "Actual Sales Price" and "Actual Construction Cost" of the buildings.

## File Structure
- `Residential-Building-Data-Set.xlsx`: The Excel file containing the dataset.
- `ridge_and_lasso.Rmd`: The R Markdown file containing all the code, descriptions, and visualizations.

## Libraries Used
- `readxl`: For reading Excel files.
- `caret`: For data splitting and cross-validation.
- `ggplot2`: For data visualization.
- `lattice`: For additional data visualization options.
- `glmnet`: For performing Ridge Regression and LASSO.

## Implementation Details

### Data Loading and Preprocessing
- The dataset is loaded from an Excel file using the `readxl` library.
- The `START QUARTER` column of the dataset is accessed, although its specific use is not detailed in the document.

### Predictor and Response Variables Description
- A brief description of some of the predictor variables is provided, helping to understand their role in the dataset.

### Data Splitting
- Two subsets of the data are created: `buildings.price` for predicting sales price and `buildings.cost` for predicting construction cost.
- Specific columns are removed from each subset to prepare them for modeling.

### Ridge Regression and LASSO for Sales Price
- Ridge Regression and LASSO are applied to predict the sales price of the buildings.
- 10-fold cross-validation is used to find the optimal regularization parameter (lambda).
- The models are fitted using the optimal lambda values, and the results are visualized.

### Ridge Regression and LASSO for Construction Cost
- Similar steps are followed for predicting the construction cost of the buildings.

### Visualization
- The results of the Ridge and LASSO models for both sales price and construction cost are visualized using various plots.

## Techniques Used
- **Ridge Regression**: A linear regression technique with L2 regularization.
- **LASSO**: A linear regression technique with L1 regularization, capable of performing variable selection.
- **Cross-Validation**: Used to find the optimal regularization parameter and assess the model's performance.
- **Data Visualization**: Used to visualize the results of the models and understand their performance.

## How to Run
1. Ensure that R and all the required libraries are installed.
2. Load the dataset onto your local machine and update the file path in the R Markdown file accordingly.
3. Open the R Markdown file in RStudio or any other R Markdown editor.
4. Run the chunks in the R Markdown file sequentially to perform the analysis and generate the visualizations.

## Conclusion
This project demonstrates the application of Ridge Regression and LASSO in predicting key financial aspects of residential buildings. Through cross-validation and visualization, the performance of the models is assessed, providing insights into the dataset and the modeling techniques used.
