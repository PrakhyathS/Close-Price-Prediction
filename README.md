# Nasdaq Closing Price Prediction

## Description

This project involves developing a predictive model for forecasting closing price movements of Nasdaq-listed stocks during the critical final ten minutes of each trading day. By leveraging data from the order book and closing auction, the model aims to provide insights into supply and demand dynamics, thereby identifying potential trading opportunities.

## Objective

Create a model that accurately predicts closing price movements for a diverse range of Nasdaq-listed stocks using historical data from the order book and closing auction.

## Dataset

The dataset comprises historical data including:
- **Order Book Dynamics**: Real-time order book data.
- **Auction Data**: Information from the closing auction.
- **Closing Price Movements**: Historical closing prices.

## Evaluation Criteria

Models are evaluated based on the **Mean Absolute Error (MAE)** between the predicted return and the observed target.

**Formula for MAE**:

$$
\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} \left| \text{Actual output value}_i - \text{Predicted output value}_i \right|
$$



## Methods

### 1. Baseline Model

Initially, we established a baseline by feeding the training data into LightGBM. The public score at this stage was **5.3888**.

### 2. Parameter Optimization

We utilized Optuna for hyperparameter tuning, which led to a slight improvement in the public score to **5.3866**.

### 3. Feature Engineering

Incorporated features related to imbalance between bid-size and ask-size, resulting in an improved public score of **5.3852**.

### 4. Additional Features

Further improvements were made by adding features such as the bid/ask ratio in size and price. This refinement aimed to enhance model performance.

## Results

The model's public score improved incrementally with each enhancement, demonstrating the effectiveness of our approaches in refining the predictions.

## Challenges and Considerations

- **Combining Order Book and Auction Data**: Effective integration of data from both sources was crucial for accurate predictions.
- **Supply and Demand Dynamics**: Understanding these dynamics was key to predicting closing price movements accurately.
- **Trading Opportunities**: The model was designed to identify potential trading opportunities in the final minutes of trading.

**Contact**: For inquiries or further information, contact [prakhyathshivappa@gmail.com](mailto:prakhyathshivappa@gmail.com)

