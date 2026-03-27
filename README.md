# Marketing Campaign Response Prediction

This project uses the UCI Bank Marketing dataset to predict whether a customer will respond positively to a marketing campaign.

## Project goal
The goal of this project is to build a machine learning model that predicts whether a customer will say yes or no to a marketing campaign offer.

## Dataset
The dataset used in this project is the UCI Bank Marketing dataset. It contains customer information and campaign-related variables.

## Data preparation
- Converted the target variable from yes/no to 1/0
- Checked missing values
- Removed the `poutcome` column because of a high percentage of missing values
- Split the data into training and testing sets

## Model
A logistic regression model was used as the baseline model.  
Numerical variables were scaled, categorical variables were one-hot encoded, and missing values were handled using a preprocessing pipeline.

## Results
- Accuracy: about 82%
- ROC-AUC: about 0.89
- Threshold tuning was tested at 0.5, 0.7, and 0.8
- A threshold of 0.7 provided a more balanced trade-off between precision and recall

## Conclusion
This project shows how machine learning can be used to predict customer campaign responses.  
It also shows the trade-off between precision and recall when changing the decision threshold.
