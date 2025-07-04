
# 📈 NVIDIA Stock Price Forecasting (Time Series)

This project focuses on forecasting NVIDIA's stock prices using the ARIMA (AutoRegressive Integrated Moving Average) model on historical open price data. The project demonstrates time series analysis, forecasting, visualization, and evaluation with a focus on predicting trends in financial markets.

---

## 🚀 Project Overview

- **Project Title**: NVIDIA Stock Price Forecasting (Time Series)
- **Objective**: Forecast NVIDIA stock prices based on 365 days of historical open price data.
- **Model Used**: ARIMA (AutoRegressive Integrated Moving Average)
- **Key Result**: Achieved Root Mean Squared Error (RMSE) of approximately **4.8**.
- **Visualization**: Trends and predictions were visualized using **Matplotlib**.

---

## 📂 Dataset

- **Source**: NVIDIA Historical Stock Price Data (CSV file used)
- **Columns Used**: 
  - `Date` (Timestamp)
  - `Open` (Opening stock price)
- **Resampling**: Daily frequency with missing value handling.

---

## 🛠 Technologies Used

- **Python Libraries**:
  - `pandas` - Data manipulation
  - `numpy` - Numerical computations
  - `matplotlib` - Visualization
  - `statsmodels` - ARIMA modeling
  - `sklearn` - Evaluation metrics

---

## 📝 Methodology

1. **Data Preprocessing**
   - Loaded the dataset and converted `Date` to datetime format.
   - Set `Date` as index and selected the `Open` price column.
   - Resampled the data to daily frequency, forward-filling any missing values.

2. **Train-Test Split**
   - Split the data into:
     - **Training Set**: 80% of the data.
     - **Test Set**: 20% of the data.

3. **Model Building: ARIMA**
   - Chose ARIMA parameters `(p=5, d=2, q=0)` based on empirical performance.
   - Trained the model on the training data.

4. **Forecasting**
   - Generated predictions on the test set using the fitted ARIMA model.

5. **Evaluation**
   - Calculated **Root Mean Squared Error (RMSE)**: **4.8**

6. **Visualization**
   - Plotted:
     - Training data
     - Actual stock prices
     - Predicted stock prices

---

## 📊 Results

| Metric | Value  |
|--------|--------|
| RMSE   | 4.8    |

- The model demonstrated reasonable accuracy in forecasting NVIDIA stock prices over the test period.
- Visualization of actual vs. predicted values showed that the ARIMA model captured overall trends effectively.

---

## 💡 Key Learnings

- Time series forecasting requires careful data preparation, including resampling and stationarity checks.
- ARIMA models can effectively capture trends in financial time series but are sensitive to parameter tuning.
- Visualization is essential for assessing model performance beyond numerical metrics.

---

## 📌 How to Run the Project

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib statsmodels scikit-learn
   ```
3. Place the NVIDIA stock CSV file in the project directory.
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook NVIDIA.ipynb
   ```

---
