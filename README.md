# Predicting Flight Delays & Cancellations
*Capstone Project by Katia Lopes-Gilbert*

# Predicting Federally Qualified Health Center Program Funding Levels

## Project Overview
Flight delays have significant economic and logistical impacts, costing the aviation industry billions of dollars annually. Delays affect both airline operations and passenger satisfaction, often leading to cascading effects such as missed connections, rebookings, and logistical complications. This project aims to predict the likelihood of flight delays and cancellations based on historical flight performance data and weather conditions. Accurately forecasting delays will enable airlines, airports, and passengers to take proactive measures, minimizing disruptions and enhancing decision-making for all involved.

## High Level Overview of Results
For this binary, imbalanced classification problem focused on predicting flight cancellations, I evaluated several ensemble models, including Balanced Random Forest and Easy Ensemble, along with baseline models like Logistic Regression and Random Forest. Using 3-fold StratifiedKFold cross-validation and a custom grid search function, I optimized hyperparameters and tested diﬀerent class imbalance handling techniques such as undersampling with RandomUnderSampler and NearMiss. The Balanced Random Forest Classifier was selected as the best model, achieving a near-perfect recall (0.9997) and a strong AUPRC (0.380), crucial for minimizing false negatives in cancellation detection. Although precision was lower (0.104), the model's ability to capture true positives justified this trade-oﬀ. Key features influencing the model included prior cancellation counts and time-related and weather variables, aligning with trends identified during exploratory analysis.

## Reports
📝 [Technical Report](https://github.com/dezertdweller/flight-cancellations/blob/main/reports/Flight%20Cancellations%20Report.pdf)\
📊 [Executive Presentation](https://github.com/dezertdweller/flight-cancellations/blob/main/reports/Predicting%20Flight%20Cancellations%20Presentation.pdf)

## Repo Organization
```
├── LICENSE
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── raw            <- The original, immutable data dump.
│   ├── interim        <- Intermediate data that has been transformed, including hourly weather data.
│   ├── preprocessed   <- Intermediate data for preprocessing.
│   └── modeling       <- Final data for modeling.
│
├── assets             <- Exported images for reporting.
│
├── notebooks          <- Jupyter notebooks. 
│   ├── 01-importing-data.ipynb
│   ├── 02-historical-performance.ipynb
│   ├── 03-exploratory-data-analysis.ipynb
│   ├── 03-weather-data.ipynb
│   ├── 04-exploratory-data-analysis-top-20.ipynb
│   ├── 05-preprocessing.ipynb
│   └── 06-modeling.ipynb
|
├── model
│   ├── model.pkl
│   └── model-results
│
├── references          <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports
│   ├── Flight Cancellations Report.pdf
│   └── Predicting Flight Cancellations Presentation.pptx 
│                      
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
```
