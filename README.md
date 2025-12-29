# 🥇 Gold Price Prediction Using GRU & LSTM

## 📌 Overview
Forecasting gold prices is a challenging task due to the complex, non-linear, and highly dynamic nature of financial markets. Gold prices are influenced by multiple interacting factors such as market trends, economic conditions, and investor sentiment.

This project applies **deep learning–based time-series forecasting** using **Gated Recurrent Units (GRU)** and **Long Short-Term Memory (LSTM)** networks to predict future gold prices. Both **single-feature** and **multi-feature** models are developed and compared to demonstrate the impact of richer feature representations on prediction accuracy.

---

## 🎯 Objectives
- Build deep learning models for gold price forecasting  
- Compare **single-feature** vs **multi-feature** approaches  
- Demonstrate the effectiveness of **GRU–LSTM hybrid architectures**  
- Evaluate model performance using **Mean Absolute Error (MAE)**  
- Provide a clean, reproducible, and well-documented pipeline  

---

## 🧠 Why GRU & LSTM?
Financial time-series data exhibits:
- long-term dependencies  
- short-term volatility  
- non-linear patterns  
- noisy fluctuations  

GRU and LSTM networks are specifically designed to handle such challenges by:
- maintaining memory over long sequences  
- selectively retaining or forgetting information  
- modeling complex temporal relationships  

These properties make them highly suitable for gold price prediction.

---

## 📂 Project Structure

├── data/
│ └── Gold Price.csv
├── notebook/
│ └── Gold_Price_Prediction.ipynb
├── README.md

---

## 🔧 Methodology

### 1️⃣ Data Preprocessing
- Load historical gold price data  
- Remove non-essential columns  
- Normalize features using `MinMaxScaler`  
- Generate time-series sequences using a sliding window  

---

### 2️⃣ Modeling Approaches

#### 🔹 Single-Feature Model
- Uses only historical gold prices  
- Captures pure temporal price dynamics  
- Serves as a baseline model  

#### 🔹 Multi-Feature Model
- Uses multiple market-related numerical features  
- Learns interactions between correlated variables  
- Provides richer contextual information  

Both models use deep **GRU and LSTM stacks** with dropout regularization.

---

### 3️⃣ Model Architecture Highlights
- Stacked GRU layers for efficient temporal encoding  
- Stacked LSTM layers for long-term dependency learning  
- Dropout for overfitting prevention  
- Linear output layer for regression  

---

### 4️⃣ Training & Evaluation
- Optimizer: **Adam**  
- Loss Function: **Mean Squared Error (MSE)**  
- Evaluation Metric: **Mean Absolute Error (MAE)**  
- Train–test split: 80% / 20%  

---

## 📊 Results

| Model            | MAE ↓ |
|------------------|-------|
| **Multi-Feature** | **154.20** |
| Single-Feature   | 343.59 |

### 🔍 Key Findings
- The **multi-feature GRU–LSTM model** reduces error by more than **50%**
- Additional market features significantly improve prediction accuracy
- Deep recurrent architectures are effective for complex financial forecasting tasks

---

## 🚀 How to Run the Project

### 🔹 Requirements
```bash
pip install numpy, pandas, matplotlib, scikit-learn, tensorflow, and keras
```
### 🔹 Run the Notebook
```bash
Gold-Price-LSTM.ipynb
```

## 👤 Author

[AmirHossein]
Deep Learning Specialist
📧 Email: amirhosseinheydarinejad69@gmail.com
🔗 GitHub: https://github.com/Amirhossein4860
