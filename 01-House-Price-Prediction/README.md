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

## Model Evaluation

The model was evaluated using an **80:20 train-test split**.

| Metric                             |              Value |
| ---------------------------------- | -----------------: |
| **R² Score**                       |         **0.9233** |
| **Mean Absolute Error (MAE)**      |  **16,184.21 USD** |
| **Mean Squared Error (MSE)**       | **490,893,351.80** |
| **Root Mean Squared Error (RMSE)** |  **22,156.11 USD** |

The model achieved an **R² Score of 0.9233**, indicating a strong linear relationship between house area and price on the test data. Since this project uses a very small dataset for learning purposes, these evaluation metrics should be interpreted as a demonstration of the model evaluation process rather than a definitive measure of real-world performance.

## Learning Outcomes

Through this project I learned:

* Loading datasets with Pandas
* Data visualization using Matplotlib
* Training a Linear Regression model
* Making predictions with scikit-learn
* Exporting results to CSV
* Basic Git and GitHub workflow

## Future Improvements

* Train the model on a larger and more diverse real-world housing dataset to improve prediction accuracy and generalization.
* Include additional features such as the number of bedrooms, bathrooms, location, parking spaces, and property age to build a more comprehensive pricing model.
* Use Cross Validation and Hyperparameter Tuning for more robust model evaluation.
* Build an interactive web application using **Streamlit** or **Flask** that allows users to estimate house prices by entering property details.
* Deploy the trained model on a cloud platform such as Render, Hugging Face Spaces, or Streamlit Community Cloud for public access.
