Hotel ADR Analysis
Project overview

This project analyzes hotel reservation data to identify the main factors associated with Average Daily Rate (ADR) — the average daily price of a hotel room.

The project combines exploratory data analysis with machine learning to investigate which reservation characteristics have the strongest relationship with ADR.

Objective

The main objectives of the project are to:

- explore the factors associated with hotel room prices,
- identify the most important features related to ADR,
- build a regression model to predict ADR,
- evaluate the model's performance.

Dataset

The analysis is based on hotel reservation data covering bookings from two hotel types:
- City Hotel
- Resort Hotel

The dataset contains information about booking characteristics, stay details, customer information and other reservation-related features.

Analysis

The project includes:

- exploratory data analysis (EDA),
- data cleaning and preprocessing,
- feature engineering,
- categorical encoding,
- train-test split,
- Decision Tree Regressor,
- hyperparameter tuning,
- model evaluation,
- feature importance analysis.
- 
Model

The final model is a tuned Decision Tree Regressor.

Test set performance
Metric	Score
MAE	10.98
RMSE	18.71
R²	0.8323

The model achieved an R² of 0.8323, meaning that it explains approximately 83% of the variance in ADR on the test set.

Key findings

The analysis identified several factors that were particularly important for predicting ADR:

- Number of guests had the highest feature importance, indicating that the size of the reservation was strongly associated with the predicted ADR.
- Arrival month and week of the year were among the important features, supporting the presence of seasonality in hotel prices observed during the exploratory analysis.
- Lead time — the number of days between booking and arrival — also had a high importance, suggesting that the timing of a reservation is an important factor in ADR.
-Reserved room type was an important predictor, which is consistent with differences in pricing between different room categories and standards.
- The feature importance results were consistent with patterns observed during EDA, indicating that the model captured relationships already identified during the exploratory analysis.

Feature importance indicates which variables were most useful to the model for predicting ADR. It does not imply that these factors directly cause changes in hotel prices.

Project structure
hotel_adr_analysis.ipynb

The notebook contains the complete analysis, from data preprocessing and exploratory data analysis to model training, evaluation and interpretation.

Tools
- Python
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn
  
How to explore the project

The complete analysis is available in the Google Colab notebook:

hotel_adr_analysis.ipynb

The notebook contains the code, visualizations, model results and conclusions.
