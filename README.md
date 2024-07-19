# Temporal Investment Forecast

## Table of Contents
1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Data Extraction](#data-extraction)
6. [Feature Engineering](#feature-engineering)
7. [Data Preprocessing](#data-preprocessing)
8. [Model](#model)
9. [Training and Evaluation](#training-and-evaluation)
10. [License](#license)

## Introduction
The Temporal Investment Forecast project aims to forecast Microsoft’s stock price using a variation of the Temporal Fusion Transformer model. The data is extracted from Nasdaq using the yfinance library, and various feature engineering and preprocessing techniques are applied to enhance the forecasting model.

## Project Structure
The project is organized as follows:
```sh
temporal-investment-forecast
┣ 📜 Temporal-investment.ipynb
┗ 📜 README.md
```
## Installation
To run this project, you need to have Google Colab or a local Jupyter Notebook setup. Follow the instructions below to get started:

1. **Open Google Colab**: Go to [Google Colab](https://colab.research.google.com/).

2. **Upload the Notebook**:
   - Click on `File` > `Upload notebook`.
   - Choose the `Temporal-investment.ipynb` file from your local machine.

3. **Set Up the Environment**:
   - Ensure you have a Google account to save and execute the notebook.

## Usage
  To use the temporal investment forecasting model, follow these steps:

1. **Execute the Notebook**:
  - Run each cell in the Temporal-investment.ipynb notebook sequentially.
  - The notebook includes the following steps:
    - Data extraction
    - Feature engineering
    - Data preprocessing
    - Model training
    - Model evaluation

## Data Extraction
  - Library: yfinance
  - Company: Microsoft
  - Ticker: MSFT
  - Data Source: Nasdaq The data is fetched using the yfinance library for Microsoft’s stock.

## Feature Engineering
Several new variables are created to improve model performance:

  - Closing Percentage Change: Measures the percentage change in closing prices.
  - Simple Moving Average (SMA): Calculates the average closing price over a specific period.
  - Moving Standard Deviation (MSD): Measures the standard deviation of closing prices over a specific period.
  - Volume Weighted Average Price (VWAP): Calculates the average price weighted by volume.
  - Relative Strength Index (RSI): Measures the speed and change of price movements.

## Data Preprocessing
The data is preprocessed using the following steps:

  - Normalization: Data is normalized using StandardScaler().
  - Splitting: Data is split into training, validation, and test sets.
  - Formatting: Data is formatted to be compatible with the model.

## Model
Temporal Fusion Transformer (TFT)
  - Description: The model is a variation of the Temporal Fusion Transformer, designed for forecasting time-series data.

## Training and Evaluation
The notebook includes sections for training and evaluating the TFT model:

  - Training: The model is trained on the preprocessed data.
  - Evaluation: The model’s performance is evaluated using appropriate metrics.

## License
This project is licensed under the MIT License. See the LICENSE file for more information.

---

Feel free to explore the notebook and experiment with different configurations to see how the model performs!

