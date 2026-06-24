# Food Delivery Time Prediction

## Project Overview

This project predicts food delivery times using Machine Learning. The objective is to analyze factors affecting delivery delays and build a model capable of estimating the expected delivery time of an order.

## Dataset

Dataset Source: Kaggle Food Delivery Dataset

The dataset contains information about:

* Delivery person details
* Traffic conditions
* Weather conditions
* Vehicle type and condition
* Restaurant and delivery locations
* Delivery time

Total Records: 45,593

## Project Workflow

### Data Cleaning

* Converted numerical columns stored as text into numeric format.
* Handled missing values using appropriate techniques.
* Cleaned categorical variables.
* Removed inconsistent entries.

### Exploratory Data Analysis (EDA)

* Analyzed delivery time distribution.
* Studied the impact of traffic density on delivery time.
* Examined weather conditions and delivery performance.
* Investigated the effect of multiple deliveries.

### Feature Engineering

Created a new feature:

* Distance between restaurant and delivery location.

### Machine Learning Model

Model Used:

* Random Forest Regressor

## Results

| Metric   | Value |
| -------- | ----- |
| MAE      | 3.23  |
| RMSE     | 4.08  |
| R² Score | 0.81  |

The model explains approximately 81% of the variation in delivery times.

## Important Features

Top factors influencing delivery time:

1. Delivery Person Ratings
2. Multiple Deliveries
3. Road Traffic Density
4. Delivery Person Age
5. Distance

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
DeliveryDelayPrediction/
│
├── DATA/
│   └── train.csv
│
├── notebooks/
│   └── delivery_delay_prediction.ipynb
│
├── README.md
│
└── requirements.txt
```

## How to Run

1. Clone the repository.
2. Open the Jupyter Notebook.
3. Run all cells in sequence.

## Conclusion

The Random Forest model successfully predicts food delivery times with good accuracy. Traffic conditions, delivery distance, rider ratings, and multiple deliveries were identified as major factors affecting delivery performance.
