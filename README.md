# 📈 NIFTY AI Stock Prediction Dashboard

A comprehensive, fully offline-capable AI-powered stock prediction dashboard designed for NIFTY market analysis. This project provides intelligent forecasting, technical analysis, and visualization capabilities through both Streamlit and Flask-based interfaces while maintaining complete offline functionality.

---

## 🚀 Features

### 🔒 Fully Offline Architecture
- Uses local SQLite database (`nifty_history.db`)
- No dependency on external APIs
- No Yahoo Finance runtime calls
- Stable execution without internet connectivity

### 🎨 Dual Frontend Support

#### Streamlit Dashboard
- Interactive stock visualization
- AI prediction graphs
- Technical indicator charts
- Real-time recommendation summaries
- Complete analytics dashboard

#### Flask + Vanilla JavaScript Frontend
- Lightweight deployment option
- REST API backend
- Static HTML frontend
- Fast rendering
- Alternative hosting compatibility

---

## 🧠 AI / Machine Learning Models

The dashboard integrates multiple forecasting approaches:

| Model | Purpose |
|--------|----------|
| LSTM | Long-term sequential stock prediction |
| GRU | Efficient time-series forecasting |
| ARIMA Surrogate | Statistical trend smoothing |
| Prophet Surrogate | Pattern forecasting fallback |
| Scikit-Learn Models | Supplementary prediction logic |

Model pipelines support:

- Local model caching
- `.keras` model persistence
- `.pkl` serialized storage
- Automatic train-or-load workflow

---

## 📊 Technical Analysis Engine

The analytics module computes:

- RSI (Relative Strength Index)
- Price Volatility
- Momentum Indicators
- Trend Detection
- Signal Generation
- Algorithmic Buy/Sell Recommendation Summary

The system includes safeguards against:

- `NaN` propagation issues
- `fillna()` TypeErrors
- Runtime plotting failures
- Data consistency errors

---

## 🗂 Project Structure

```text
NIFTY-AI-STOCK-DASHBOARD/
│
├── app.py
├── api.py
├── data_fetch.py
├── analysis.py
├── model.py
├── nifty_history.db
├── script.js
├── index.html
└── README.md
```

### Module Description

### `app.py`
Streamlit dashboard frontend.

### `api.py`
Flask backend API engine.

### `data_fetch.py`
Handles offline database retrieval and fallback logic.

### `analysis.py`
Computes indicators and technical analytics.

### `model.py`
Model training, caching, loading, and prediction pipelines.

### `nifty_history.db`
Local SQLite historical stock database.

---

## ⚙ Installation

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/NIFTY-AI-STOCK-DASHBOARD.git

cd NIFTY-AI-STOCK-DASHBOARD
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate:

Windows:

```bash
venv\Scripts\activate
```

Linux / Mac:

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶ Running Application

## Streamlit Dashboard (Recommended)

Launch dashboard:

```bash
python -m streamlit run app.py
```

Features:

- Interactive graphs
- Model prediction visualization
- Technical analysis metrics
- Recommendation engine

---

## Flask API + Static Frontend

Start API:

```bash
python api.py
```

Open:

```text
index.html
```

The frontend automatically communicates with:

```text
http://localhost:5000
```

---

## 💾 Offline Data Engine

The project prioritizes reliability by using:

```text
SQLite Local Cache
```

Database:

```text
nifty_history.db
```

Advantages:

- Zero API dependency
- Faster loading
- Stable predictions
- Reproducible results

---

## 🛠 Technologies Used

### Backend
- Python
- Flask
- SQLite
- Pandas
- NumPy

### Machine Learning
- TensorFlow / Keras
- Scikit-Learn

### Frontend
- Streamlit
- HTML
- CSS
- Vanilla JavaScript

### Visualization
- Matplotlib
- Plotly

---

## 🔮 Future Improvements

- Portfolio optimization module
- Sentiment analysis integration
- Multi-stock comparison
- Advanced transformer-based forecasting
- Export prediction reports
- User authentication dashboard

---

## 🤝 Contribution

Contributions are welcome.

Steps:

1. Fork repository
2. Create feature branch

```bash
git checkout -b feature/NewFeature
```

3. Commit changes

```bash
git commit -m "Added New Feature"
```

4. Push branch

```bash
git push origin feature/NewFeature
```

5. Open Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## ⭐ Support

If this project helped you, consider giving it a ⭐ on GitHub.

---

Developed for intelligent offline NIFTY stock forecasting and technical market analytics.
