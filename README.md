# NYC Airbnb 2021 — Price Analysis & Prediction

## Overview
Exploratory data analysis and price prediction on the New York City Airbnb dataset (December 2021), containing **38,277 listings** across all five NYC boroughs.

## Dataset
- **Source:** [Kaggle — Airbnb New York (Dec 2021)](https://www.kaggle.com/datasets/sirapatsam/airbnb-new-york-4dec2021)
- **Features:** 18 columns including location, room type, availability, and reviews
- **Target:** Listing price (per night)

## Project Structure
```
├── New_York_Airbnb_4_dec_2021_2.csv   # Raw dataset
├── airbnb_nyc_2021_analysis.ipynb     # Main analysis notebook
└── README.md
```

## Key Findings
- **Manhattan** has the highest median listing prices (~$175/night)
- **Entire home/apt** listings are ~2× more expensive than private rooms
- Geographic coordinates and room type are the strongest price predictors
- **Random Forest** outperforms all linear regression models (Ridge, Lasso, ElasticNet)

## Methods Used
| Step | Approach |
|------|----------|
| EDA | Boxplots, pie charts, geographic scatter map, top neighbourhood analysis |
| Preprocessing | Outlier removal (price > $1000), median imputation, log transformation |
| Encoding | LabelEncoder for categorical variables |
| Modelling | Linear Regression, Ridge, Lasso, ElasticNet, Random Forest |
| Evaluation | MAE, RMSE, R² (on 20% test set) |

## How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy
jupyter notebook airbnb_nyc_2021_analysis.ipynb
```

## Requirements
- Python 3.8+
- pandas, numpy, matplotlib, seaborn
- scikit-learn, scipy
