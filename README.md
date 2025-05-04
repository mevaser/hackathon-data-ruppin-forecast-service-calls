# 📈 Hackathon Data Ruppin – Forecasting Municipal Service Calls

This project was developed as part of the **Hackathon Data Challenge 2025** at Ruppin Academic Center.

🏆 We proudly achieved **3rd place** in the competition!

It aims to improve municipal service quality in Emek Hefer by predicting:

- ✉️ **The volume of incoming service calls** per topic and date.
- ⏳ **The estimated handling time** for a given request.

We built a smart system to assist the municipality in **planning resources** and **updating citizens** with estimated response times.

---

## 🧠 What We Did

### ✍️ Data Preparation

- Merged service request data with external **weather data**.
- Created new features: holidays, moving averages, one-hot encoding for categorical features (topics, dates).
- Built two labeled datasets:
  1. For predicting **call volumes**.
  2. For predicting **handling duration**.

### ⚖️ Models Trained

#### ⚡ Call Volume Forecasting:

- Random Forest
- Gradient Boosting
- XGBoost
- MLP (Neural Network)
- LSTM (RNN)

#### ⏳ Handling Time Prediction:

- LSTM Neural Network

Each model was evaluated using MAE, RMSE, and R^2.

✅ The addition of **momentum features (moving averages)** significantly improved model performance: boosting **R² from 0.45 to 0.7**.

---

## 💪 Notable Features

- **Momentum-based features**: moving averages of recent days.
- **Weather-based features**: rainfall indicators.
- **Temporal features**: year, month, weekday (in Hebrew).
- **Topic-specific predictions**: per service type (e.g., garbage, pests, public lighting).
- **XAI**: explainability using LIME and counterfactuals.

---

## 📄 Project Structure

```
├── data/                # Cleaned datasets ready for modeling
├── images/              # Visualizations and plots
├── notebooks/           # Model training, evaluation, prediction
├── presentation/        # Final slides for demo day
├── .gitignore
└── README.md
```

---

## 🗕️ How the Municipality Benefits

- ⏰ Forecast load spikes (e.g., holidays, seasonal topics)
- 🧠 Allocate teams based on predicted need
- 🥵 Improve response time estimates sent to citizens

---

## 👥 Contributors

- [@mevaser](https://github.com/mevaser) – modeling, preprocessing, and LSTM evaluation
- [@galazulay3](https://github.com/galazulay3) – modeling, creative feature engineering, and joint data preparation

---

## 💼 License

This project is open for educational use and collaboration. Credit is appreciated.
