# Hybrid Time Series Forecasting Framework Using LSTM, FFT, ADMM

## 📌 Overview  
This project presents a **Hybrid Time Series Forecasting Framework** integrating **Long Short-Term Memory (LSTM) networks, Fast Fourier Transform (FFT), and Alternating Direction Method of Multipliers (ADMM)** to enhance predictive performance. The model is trained on historical stock price data to improve forecasting accuracy by leveraging both time-domain and frequency-domain features.

## 🚀 Features  
✅ **LSTM for sequential modeling** – Captures temporal dependencies  
✅ **FFT for feature extraction** – Identifies cyclic patterns in time series data  
✅ **ADMM for feature selection** – Ensures relevant features are retained  
✅ **Hybrid approach** – Combines time-domain and frequency-domain analysis for improved accuracy  
✅ **Comparative Analysis** – Evaluates models with and without hybrid techniques  

## 🏗️ System Architecture  
The system consists of:  
- **Preprocessing**: Outlier handling, normalization, and feature selection  
- **Feature Engineering**:  
  - FFT to extract dominant frequency components  
  - ADMM to select the most informative features  
- **LSTM Model**:  
  - Trained with and without FFT + ADMM features for comparison  
  - Evaluated using RMSE, MSE, and time-space complexity analysis  

## 📜 Project Structure  
```
/hybrid-time-series-forecasting
│── data/                          # Dataset (e.g., BAJAJ-AUTO.csv)
│── preprocessing/                  # Data cleaning, normalization, FFT, ADMM
│── model/                          # LSTM Model Training & Evaluation
│   ├── train.py                    # Train LSTM models with and without FFT + ADMM
│   ├── evaluate.py                  # Performance comparison & metrics calculation
│── utils/                          # Helper functions (feature extraction, plotting)
│── README.md                        # Project Documentation
│── requirements.txt                  # Dependencies
│── results/                         # Model results, graphs, and logs
```

## 🛠️ Installation & Setup  

### 1️⃣ Prerequisites  
- **Python 3.7+**  
- Required libraries (install via `requirements.txt`)  
```bash
pip install -r requirements.txt
```

### 2️⃣ Clone the Repository  
```bash
git clone https://github.com/your-repo/hybrid-time-series-forecasting.git
cd hybrid-time-series-forecasting
```

### 3️⃣ Run Preprocessing  
```bash
python preprocessing/data_preprocess.py
```

### 4️⃣ Train Models  
- **With FFT + ADMM Features:**  
```bash
python model/train.py --use_hybrid
```
- **Without FFT + ADMM Features:**  
```bash
python model/train.py
```

### 5️⃣ Evaluate Performance  
```bash
python model/evaluate.py
```

## 🔍 Key Algorithms Used  
### 📊 Fast Fourier Transform (FFT)  
- Extracts frequency components from time series data  
- Helps detect periodic patterns that improve forecasting accuracy  

### 🔍 Alternating Direction Method of Multipliers (ADMM)  
- Performs feature selection  
- Ensures optimal selection of relevant data, reducing model complexity  

### 🔮 Long Short-Term Memory (LSTM)  
- Captures long-term dependencies in sequential data  
- Improves prediction quality compared to traditional models  

## 📌 Results & Performance  
- **LSTM with FFT + ADMM** shows **lower RMSE & MSE** than LSTM alone  
- **Time Complexity Analysis**: Hybrid approach has **higher computational cost**  
- **Space Complexity Analysis**: ADMM reduces redundant features, optimizing storage  

## 📄 Future Enhancements  
🔹 **Real-time Forecasting** with live stock data  
🔹 **Parameter Optimization** for improved efficiency  
🔹 **Explainability** – Feature importance visualization  


This `README.md` provides clear **setup instructions, system architecture, feature details, and evaluation steps**. Let me know if you need any modifications! 🚀
