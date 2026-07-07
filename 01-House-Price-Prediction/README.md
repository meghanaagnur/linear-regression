# House Price Prediction using Linear Regression

A beginner Machine Learning project that predicts house prices based on the area of a house using **Simple Linear Regression** with **scikit-learn**.

This project was built while learning Machine Learning from the CodeBasics tutorial and demonstrates the complete workflow of training, visualizing, and using a regression model for prediction.

##  Project Overview

The model learns the relationship between a house's area (in square feet) and its selling price.

After training, the model can estimate the price of houses whose areas are not present in the original dataset.

## Dataset

### Training Data (`homeprices.csv`)

| Area (sq.ft) | Price (USD) |
| ------------ | ----------: |
| 2600         |      550000 |
| 3000         |      565000 |
| 3200         |      610000 |
| 3600         |      680000 |
| 4000         |      725000 |

### Prediction Data (`areas.csv`)

Contains house areas for which prices are predicted.

The predicted values are saved to:

```text
house_price_prediction.csv
```

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Machine Learning Workflow

* Load the dataset
* Visualize the data
* Train a Linear Regression model
* Predict house prices
* Export predictions to a CSV file

## Results

The trained model predicts house prices for unseen house areas using a fitted linear regression line.

Example prediction:

| Area | Predicted Price |
| ---: | --------------: |
| 3300 |      ≈ $628,715 |

## How to Run

Clone the repository:

```bash
git clone <your-repository-url>
cd <repository-name>
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook
```

Run all notebook cells to train the model and generate predictions.

## Learning Outcomes

Through this project I learned:

* Loading datasets with Pandas
* Data visualization using Matplotlib
* Training a Linear Regression model
* Making predictions with scikit-learn
* Exporting results to CSV
* Basic Git and GitHub workflow

