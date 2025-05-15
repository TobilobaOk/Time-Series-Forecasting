# Inflation Rate Prediction in Nigeria using Deep Learning (LSTM & GRU)

This project leverages advanced deep learning techniques (LSTM and GRU) to predict Nigeria's inflation rate based on time series and macroeconomic indicators like crude oil price, production, and various CPI components.

##Project Overview

Inflation prediction is crucial for economic planning and policy decisions. This project explores two Recurrent Neural Network (RNN) architectures 

— **Long Short-Term Memory (LSTM)**and **Gated Recurrent Unit (GRU)** 

— to forecast Nigeria's inflation rate using historical data.

## Models Used

- **LSTM (Long Short-Term Memory)**
- **GRU (Gated Recurrent Unit)**

Both models were trained and evaluated using the same dataset and configuration
---

## Dataset

- **Source:** Data set was gotten from Online Repository.
- **Features:**
  - Crude Oil Price
  - Crude Oil Production
  - Crude Oil Export
  - CPI Components (e.g., food, housing, health, education)

- **Target:**
  - Inflation Rate (monthly)

  ---
 
  Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib & Seaborn (for visualization)

  ---

 ## Model Performance Summary

### 🔹 GRU Model

- **Initial val_loss:** 0.0335
- **Best val_loss:** 0.0335 (Epoch 1)
- **Final val_loss:** 0.1424

**Pros:**
- Stable but limited learning
- Low risk of overfitting

**Cons:**
- Underfitting after Epoch 1
- No performance improvement with more training

---

LSTM Model

- **Initial val_loss:** 0.0080
- **Best val_loss:** 0.0019 (Epoch 18)
- **Final val_loss:** 0.2288

**Pros:**
- Excellent early generalization
- Best overall predictive performance

**Cons:**
- Overfitting observed after Epoch 25
- Validation loss increased in later epochs

  Conclusion

While both models were able to learn from the dataset, **LSTM outperformed GRU** in terms of predictive accuracy. GRU showed signs of underfitting, while LSTM offered superior results but required regularization and early stopping to prevent overfitting.

**Recommendation:**
> Use **LSTM** with early stopping and dropout layers for optimal inflation forecasting.

---

Future Work

- Incorporate more economic indicators (e.g., exchange rates, interest rates)
- Apply hyperparameter tuning (e.g., learning rate, optimizer)
- Use ensemble models (e.g., LSTM + GRU hybrid)
- Deploy model as a web app for real-time forecasting

---

For questions or collaboration:
Oluwatobi Adebamiro 
– https://www.linkedin.com/in/oluwatobi-adebamiro-7a9468184 
– tobilobaadebamiro@gmail.com
