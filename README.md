# 📈 Enhanced Stock Market Forecasting Using Hybrid BiLSTM-GRU Model

This project implements an advanced deep learning-based forecasting system using a hybrid **BiLSTM-GRU** model to predict stock prices based on historical **S&P 500** data. The architecture captures both forward and backward temporal dependencies, resulting in highly accurate predictions.

---

## 🔍 Overview

Stock price prediction is vital for informed financial decisions. In this project, we benchmarked multiple models, including both classic machine learning and deep learning approaches:

- Traditional Models: `Random Forest`, `GARCH`
- Deep Learning Models: `CNN`, `LSTM`, `GRU`, `BiLSTM`, `Transformer (Attention)`
- Hybrid Architectures:
  - `LSTM + CNN + RF`
  - `GARCH + LSTM`
  - `LSTM + GRU`
  - **`BiLSTM + GRU`** *(Best Performing)*

After comprehensive experimentation, the **BiLSTM + GRU** model achieved the best performance across all evaluation metrics.

---

## 📊 Dataset

- **Source:** S&P 500 Historical Data
- **Records:** 2,538 trading days
- **Features Used:** `Date`, `Open`, `High`, `Low`, `Close`, `Change%`

> 📌 *You can include a data summary table or EDA visualizations here.*

---

## ⚙️ Model Architecture

The hybrid **BiLSTM-GRU** model is structured as follows:

Input → BiLSTM(50) → Dropout(0.2) → GRU(50) → Dropout(0.2) → Dense → Output

> 🖼️ *Figure 1: Block Diagram of the Model*

---

## 🧪 Evaluation Metrics

| Metric  | Score     |
|---------|-----------|
| RMSE    | 0.0125    |
| MAE     | 0.0101    |
| MAPE    | 0.83%     |
| R²      | 0.9901    |

> 🖼️ *Figure 2: Validation vs Predicted*  
> 🖼️ *Figure 3: Regression Plot*  
> 🖼️ *Figure 4: Training Loss Convergence*

Compared to other models, **BiLSTM+GRU** consistently produced the lowest error and highest R² score, showing excellent generalization and training stability (F-test confirmed).

---

## 🧠 Key Features

- ✅ Historical time-series preprocessing with scaling & windowing
- ✅ Hybrid model combining BiLSTM & GRU layers
- ✅ Evaluation using RMSE, MAE, MAPE, and R²
- ✅ Visualization of model predictions vs actual prices
- ✅ Modular, reproducible codebase

---

## 💡 Applications

- 📈 Real-time stock forecasting for financial platforms  
- 🧠 Decision support for investors and analysts  
- 🧮 Portfolio risk mitigation via predictive insights  
- 📊 Integration with financial dashboards

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/kscoder27/Hybrid-Stock-Market-Model.git



<img width="989" height="590" alt="ConvergenceGraph" src="https://github.com/user-attachments/assets/ea7fb2d5-7c03-41e3-917d-e1f3921af902" />
<img width="989" height="790" alt="RegressionGraph" src="https://github.com/user-attachments/assets/5ec5bb85-aa8a-4c01-a13a-4b28e8e60dd5" />

<img width="1280" height="594" alt="ValidationandTestPredicitions" src="https://github.com/user-attachments/assets/66624cf4-af90-4a4b-9b55-409311e2e787" />


