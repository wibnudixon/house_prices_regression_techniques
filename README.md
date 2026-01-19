# House Prices Regression Techniques

A Kaggle competition project to predict house prices using advanced regression techniques.

## Project Overview

Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling or the proximity to an east-west railroad. But this playground competition's dataset proves that much more influences price negotiations than the number of bedrooms or a white-picket fence.

With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home.

## Dataset

The dataset includes:
- `train.csv` - Training set with 1460 observations
- `test.csv` - Test set for predictions
- `data_description.txt` - Full description of each column
- `sample_submission.csv` - Submission format example

## Evaluation

### Goal
Predict the sales price for each house. For each Id in the test set, predict the value of the SalePrice variable.

### Metric
Submissions are evaluated on Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the logarithm of the observed sales price. Taking logs means that errors in predicting expensive houses and cheap houses will affect the result equally.

### Submission File Format
The file should contain a header and have the following format:

```
Id,SalePrice
1461,169000.1
1462,187724.1233
1463,175221
etc.
```

## Project Structure

```
├── Data/
│   ├── train.csv
│   ├── test.csv
│   ├── data_description.txt
│   └── sample_submission.csv
├── house_prices_analysis.ipynb
├── Pipfile
└── README.md
```

## Getting Started

1. Install dependencies:
   ```bash
   pipenv install
   ```

2. Open the Jupyter notebook:
   ```bash
   jupyter notebook house_prices_analysis.ipynb
   ```

3. Follow the analysis workflow in the notebook

## Methodology

1. **Exploratory Data Analysis (EDA)**
   - Data loading and inspection
   - Statistical summary
   - Missing values analysis
   - Feature distributions

2. **Data Preprocessing**
   - Handling missing values
   - Feature engineering
   - Encoding categorical variables
   - Feature scaling

3. **Model Development**
   - Baseline models
   - Advanced regression techniques
   - Model evaluation and comparison

4. **Prediction & Submission**
   - Generate predictions
   - Create submission file