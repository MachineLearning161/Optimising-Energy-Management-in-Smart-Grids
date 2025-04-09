
# ⚡ Electricity Demand Forecasting in England & Wales

This project leverages Machine Learning and Deep Learning techniques to forecast electricity demand using historical energy grid data. It includes models like **Random Forest**, **XGBoost**, **LSTM**, and **CNN** to evaluate and compare performance for time-series forecasting.

---

## 📌 Project Objective

To accurately predict short-term electricity demand in the England & Wales region based on time-stamped settlement data, embedded generation sources (solar, wind), and interconnector flows.

---

## 📂 Project Structure

```
electricity-demand-forecasting/
│
├── data/                      # Raw and processed datasets
├── notebooks/                 # Jupyter Notebooks for EDA, ML/DL Models
├── src/                       # Modular Python scripts for preprocessing and modeling
├── models/                    # Trained model files (.pkl, .h5, etc.)
├── reports/                   # Visualizations and final analysis
├── requirements.txt           # Python dependencies
├── README.md                  # This file
└── .gitignore                 # Ignore cache, virtual envs, checkpoints
```

---

## 📊 Models Implemented

| Model          | Type           | Technique         |
|----------------|----------------|-------------------|
| Random Forest  | Machine Learning | Ensemble Trees   |
| XGBoost        | Machine Learning | Gradient Boosting|
| LSTM           | Deep Learning    | Recurrent NN     |
| CNN            | Deep Learning    | 1D Conv Layers   |

---

## 🔍 Data Features

- `SETTLEMENT_DATE`, `SETTLEMENT_PERIOD`
- `ENGLAND_WALES_DEMAND`
- `EMBEDDED_WIND_GENERATION`, `EMBEDDED_SOLAR_GENERATION`
- Interconnector flows (`IFA_FLOW`, `NEMO_FLOW`, `NSL_FLOW`, etc.)
- `SCOTTISH_TRANSFER`, `PUMP_STORAGE_PUMPING`, etc.

---

## 📈 Key Visualizations

- Demand Trends Over Time
- Correlation Heatmaps
- Feature Importances
- Predicted vs Actual Demand (per model)

---

## 🛠️ How to Run

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/electricity-demand-forecasting.git
cd electricity-demand-forecasting
```

2. **Install dependencies:**

```bash
pip install -r requirements.txt
```

3. **Launch Jupyter Notebooks:**

```bash
jupyter notebook
```

4. **Run notebooks in sequence from `notebooks/` folder.**

---

## 📊 Model Performance 
Model	            MAE (kWh)	   RMSE (kWh)
Random Forest	     170.20	     219.65
XGBoost	           185.43	     245.11
LSTM	              0.07	     0.08
CNN	                0.06	     0.08

---

## 🧠 Tech Stack

- Python
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn, XGBoost
- TensorFlow / Keras
- Jupyter Notebook

---

## ✅ Future Improvements

- Add attention mechanism to LSTM
- Incorporate weather features (e.g., temperature, sunlight hours)
- Deploy with a Streamlit dashboard for real-time forecasting

---
