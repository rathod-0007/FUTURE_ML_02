# 📈 Stock Price Prediction using LSTM and Hyperparameter Tuning

This project focuses on predicting future stock prices using historical stock data and LSTM neural networks. It involves data preprocessing, sequence generation, model building, hyperparameter tuning with Keras Tuner, and evaluation using RMSE, MAE, and R² score.

---

## 🔧 Features

- Preprocessing historical stock data
- Time series modeling using LSTM
- Hyperparameter tuning with Keras Tuner
- Evaluation using standard regression metrics
- Visualization of predicted vs actual prices

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Keras Tuner
- Matplotlib

---

## 📁 Dataset

The dataset includes historical stock prices with the following columns:

```
['Date', 'Close/Last', 'Volume', 'Open', 'High', 'Low']
```

Ensure:
- Columns are stripped of whitespace
- Prices are cleaned (e.g., remove `$` sign and convert to float)

Example source: [Yahoo Finance](https://finance.yahoo.com/)

---

## 🚀 Getting Started

1. **Clone this repository:**
   ```bash
    git clone https://github.com/rathod-0007/FUTURE_ML_02.git
   cd FUTURE_ML_02
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run in Jupyter or Google Colab:**
   - Upload your `.csv` dataset
   - Execute all notebook cells

---

## 📊 Evaluation Metrics

The model is evaluated using the following metrics:

- **RMSE** – Root Mean Squared Error
- **MAE** – Mean Absolute Error
- **R² Score** – Coefficient of Determination

---

---

## 🔄 Project Workflow

1. **Data Collection**: Load historical stock data (e.g., from Yahoo Finance).
2. **Data Cleaning & Preprocessing**: Remove special characters, format date columns, normalize price values.
3. **Sequence Generation**: Convert time series into supervised format using sliding window.
4. **Model Building**: Create and train an LSTM model to learn temporal patterns.
5. **Hyperparameter Tuning**: Use Keras Tuner to optimize model performance.
6. **Evaluation**: Calculate RMSE, MAE, and R² on test predictions.
7. **Visualization**: Plot predicted vs actual stock prices for visual analysis.

---

---

## 📊 Results & Evaluation

| Model              | MAE    | RMSE   |
|-------------------|--------|--------|
| LSTM            | 1.56   | 1.91   | 



| Model              | Units | Droupout Rate  |
|-------------------|--------|----------------|
| 1st LSTM layer    | 200   | 0.5  |
| 2nd LSTM layer   | 200   | 0.1   |

Best learning rate: 0.006098158336710077


| Model              | Learning Rate    |
|-------------------|--------|
| LSTM            |  0.006098158336710077  |

---


## 📈 Visual Output Example


![Stock Closing Price History](https://github.com/rathod-0007/FUTURE_ML_02/blob/main/Stock%20Closing%20Price%20History.png?raw=true)  
*Stock Closing Price History*

![Actual vs Predicted Stock Prices](https://github.com/rathod-0007/FUTURE_ML_02/blob/main/Actual%20vs%20Predicted.png?raw=true)  
*Actual vs Predicted Stock Prices using LSTM*

![7 Day Forecasted Stock Price](https://github.com/rathod-0007/FUTURE_ML_02/blob/main/Predict%20Next%20n_days%20Ahead.png?raw=true)  
*7 Day Forecasted Stock Price*

---

## 📈 Results

- Improved accuracy through hyperparameter tuning
- Visual comparison of predicted vs actual prices

---

## 📬 Contact

For queries or collaborations:

- Name: Pavan Kumar Naik Rathod
- Email: [rathodpavan2292@gmail.com]  
- LinkedIn: [https://www.linkedin.com/in/rathod-pavan-kumar/](https://www.linkedin.com/in/rathod-pavan-kumar/)

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).

## 🙌 Acknowledgments

- [TensorFlow](https://www.tensorflow.org/)
- [Keras Tuner](https://keras.io/keras_tuner/)
- [Yahoo Finance](https://finance.yahoo.com/)
