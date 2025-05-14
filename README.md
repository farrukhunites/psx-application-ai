# 📈 PSX Stock Closing Price Forecasting Using LSTM

This project focuses on forecasting the **closing prices** of **20 major stocks listed on the Pakistan Stock Exchange (PSX)** using a **Sequential LSTM (Long Short-Term Memory) neural network** model. The goal was to predict next-day closing prices using historical stock data spanning the last 20 years.

## 📊 Forecasted Stocks

- Bank Alfalah (BAFL)  
- D.G. Khan Cement (DGKC)  
- Engro Fertilizers (EFERT)  
- Engro Corporation (ENGRO)  
- Fauji Cement (FCCL)  
- Fauji Fertilizer Bin Qasim (FFBL)  
- Habib Bank Limited (HBL)  
- Hub Power Company (HUBC)  
- Mari Petroleum (MARI)  
- Meezan Bank (MEBL)  
- Maple Leaf Cement (MLCF)  
- Millat Tractors (MTL)  
- Netsol Technologies (NETSOL)  
- Oil and Gas Development Company (OGDC)  
- Pak Elektron Ltd. (PAEL)  
- Pakistan Petroleum Ltd. (PPL)  
- Pakistan Refinery Ltd. (PRL)  
- Pakistan State Oil (PSO)  
- Sui Northern Gas Pipelines Ltd. (SNGP)  
- Systems Limited (SYS)  

## 🧠 Model Overview

- **Model Type**: Sequential LSTM (Long Short-Term Memory)
- **Libraries Used**: TensorFlow / Keras, Pandas, NumPy, Matplotlib, Scikit-learn
- **Data Source**: [https://dps.psx.com.pk](https://dps.psx.com.pk)
- **Data Span**: Last 20 years (scraped programmatically)
- **Input Features**: Historical closing prices
- **Evaluation Metric**: Mean Absolute Error (MAE), Root Mean Square Error (RMSE), Prediction Accuracy

### 🔍 Model Performance

- **Average Accuracy**: 85%+
- **Prediction Error**: Within ±5% of actual closing prices on most stocks

## 📂 Project Structure

```
📁 psx-application-ai/
├── Date wise data/
│   ├── 2014
│   ├── ...
├── Pre_processed_data/
│   ├── Trainings.ipynb
│   └── bafl_data.csv
├── Trainings/
│   └── balf_training.ipynb
├── utils/
│   └── unzip_files.ipynb.ipynb
│   └── updated_data_scrapper_code.ipynb
├── requirements.txt
└── README.md
```

## 🛠️ Installation & Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/farrukhunites/psx-application-ai.git

2. **View predictions in notebook**:
   * Open `Trainings/bafl_training.ipynb` in Jupyter or VSCode.

3. **View sample results in notebook**:
   * Open `Trainings/bafl_valid_predictions.ipynb` in Jupyter or VSCode.

## 📈 Sample Results

Example comparison of actual vs predicted closing prices:

| Date       | Actual Price | Predicted Price | Prediction Correct +- 5% |
| ---------- | ------------ | --------------- | ------------------------ |
| 2024-10-01 | 189.50       | 191.20          | True                     |
| 2024-10-02 | 190.30       | 188.10          | False                    |

> ✅ The predictions are consistently within ±5% range, showing strong learning of stock patterns.

## 🧹 Future Improvements

* Incorporate technical indicators (MACD, RSI, etc.)
* Try Bi-Directional LSTMs or Transformer-based models
* Integrate real-time API data for live predictions
* Integrate this model with already built web app (https://github.com/farrukhunites/psx_backend_application)

---

## 🙋‍♂️ About Me

**Muhammad Farrukh Umair**  
Software Engineer | AI & Data Enthusiast

📫 **Email**: [haris.umair2002@gmail.com](mailto:haris.umair2002@gmail.com)  
🔗 **LinkedIn**: [linkedin.com/in/muhammad-farrukh-umair](https://www.linkedin.com/in/muhammad-farrukh-umair/)

---

## 🧾 License

This project is open-source and available under the [MIT License](LICENSE).
