# 📌 Bitcoin Price Prediction Using LSTM  

## 🚀 Project Overview  
This project uses **Long Short-Term Memory (LSTM) neural networks** to predict **Bitcoin prices** based on historical data fetched from the **Twelve Data API**. It applies **time-series forecasting techniques**, including data preprocessing, normalization, and deep learning models, to make short-term Bitcoin price predictions.  

---

## 🛠 Features  
✅ **Fetches real-time Bitcoin price data** using the Twelve Data API  
✅ **Preprocesses time-series data** (scaling, reshaping)  
✅ **Builds a deep learning LSTM model** to analyze trends  
✅ **Predicts future Bitcoin prices** based on historical patterns  
✅ **Visualizes actual vs. predicted prices** using Matplotlib  

---

## 📂 File Structure  
```bash
📂 bitcoin-price-prediction  
 ├── 📜 bitcoin_price_prediction.py   # Main script for data processing & prediction  
 ├── 📜 README.md                     # Project documentation  
 ├── 📜 requirements.txt              # List of dependencies  
```

---

## 🛠 Installation  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/yourusername/bitcoin-price-prediction.git
cd bitcoin-price-prediction
```

### 2️⃣ Install Dependencies  
Ensure you have **Python 3.x** installed, then install the required libraries:  
```bash
pip install pandas numpy matplotlib requests keras tensorflow scikit-learn
```

---

## 📊 How It Works  

### 📌 Step 1: Fetch Bitcoin Data  
- Retrieves historical **Bitcoin price** data using the **Twelve Data API**  
- Extracts the **closing price** for each 5-minute interval  
- Converts data into a **pandas DataFrame**  

### 📌 Step 2: Preprocess Data  
- **Normalizes** price values using **MinMaxScaler**  
- Creates **training sequences** using a **24-time step window**  
- Splits data into **training and testing sets**  

### 📌 Step 3: Build & Train LSTM Model  
- Constructs a **stacked LSTM network** with dropout layers  
- Uses **ReLU activation** for LSTM layers  
- Compiles with **MSE loss function** and **Adam optimizer**  
- Trains the model for **10 epochs**  

### 📌 Step 4: Make Predictions  
- Fetches **new Bitcoin price data** for testing  
- Applies the trained **LSTM model** to make predictions  
- Inversely transforms scaled predictions back to real price values  

### 📌 Step 5: Visualize Results  
- **Plots actual vs. predicted Bitcoin prices** using Matplotlib  
- Compares **trends in real price movements**  

---

## 🔥 Results  
📊 **Actual vs. Predicted Bitcoin Prices**  
- **LSTM captures Bitcoin trends well**, but improvements can be made.  

---

## 💡 Future Improvements  
🚀 Implement **Bidirectional LSTMs** for better trend detection  
🚀 Optimize model with **hyperparameter tuning**  
🚀 Deploy model as a **Flask or FastAPI web service**  
🚀 Extend dataset to **train on larger time frames**  

---

## 📜 License  
This project is **open-source** and free to use. Contributions are welcome! 🚀  
