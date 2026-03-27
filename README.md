# Boston House Price Prediction

This project is a Machine Learning regression project developed as part of the **ShadowFox AI/ML Internship**.  
The goal of this project is to predict **Boston house prices** using different regression models and compare their performance to select the best one.

---

## Project Objective

The main objective of this project is to:

- analyze the Boston Housing dataset
- handle missing values properly
- train multiple regression models
- compare their performance using evaluation metrics
- select the most suitable model for house price prediction

---

## Dataset Used

The dataset used in this project is:

- **HousingData.csv**

It contains housing-related features such as:

- CRIM
- ZN
- INDUS
- CHAS
- NOX
- RM
- AGE
- DIS
- RAD
- TAX
- PTRATIO
- B
- LSTAT

Target variable:

- **MEDV** → Median value of owner-occupied homes

---

## Technologies and Libraries Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

The complete workflow of this project is as follows:

### 1. Data Loading
The dataset was uploaded and loaded into Google Colab using Pandas.

### 2. Data Exploration
Basic dataset inspection was performed using:
- `head()`
- `shape`
- `columns`
- `info()`
- `isnull().sum()`
- `describe()`

### 3. Data Preprocessing
- Input features (`X`) and target (`y`) were separated
- Train-test split was performed
- Missing values were handled using **SimpleImputer**
- Median strategy was used for data imputation

### 4. Model Training
The following regression models were trained:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### 5. Model Evaluation
The models were evaluated using:

- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)
- R² Score

### 6. Best Model Selection
The model with the best performance was selected based on:

- highest R² score
- lowest error values

### 7. Visualization
Two plots were used for better understanding of model performance:

- Actual vs Predicted Prices
- Residual Plot

---

## Models Compared

| Model | MAE | MSE | RMSE | R² Score |
|------|------:|------:|------:|------:|
| Linear Regression | 3.147843 | 24.983445 | 4.998344 | 0.659319 |
| Decision Tree | 3.152941 | 26.134706 | 5.112211 | 0.643620 |
| Random Forest | 2.047843 | 8.131793 | 2.851630 | 0.889113 |

---

## Final Best Model

**Random Forest Regressor** was selected as the final best model because:

- it achieved the **highest R² score**
- it gave the **lowest MAE**
- it gave the **lowest MSE**
- it gave the **lowest RMSE**

So, Random Forest performed better than Linear Regression and Decision Tree for this dataset.

---

## Output Visualizations

The notebook includes the following visual outputs:

- **Actual vs Predicted Prices Scatter Plot**
- **Residual Plot**

These visualizations help in understanding:

- how close the predictions are to actual values
- how errors are distributed

---

## Project File

Main notebook file:

- `Boston_House_Pricing.ipynb`

Dataset file:

- `HousingData.csv`

---

## Conclusion

This project helped in understanding the complete Machine Learning workflow for a regression problem, including:

- data preprocessing
- missing value handling
- model training
- model comparison
- model evaluation
- model selection

Among all the tested models, **Random Forest Regressor** gave the best performance for Boston House Price Prediction.

---

## Future Improvements

This project can be improved further by:

- performing feature selection
- tuning hyperparameters
- applying cross-validation
- deploying the model as a web app
- testing additional regression algorithms

---

## Author

**Anuja Bagalkot**  
ShadowFox AI/ML Internship Project
