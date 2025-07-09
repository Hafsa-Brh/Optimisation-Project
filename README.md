# Optimisation-Project

This repository contains a time series forecasting project using an LSTM model. The focus of the project is on **meta-optimization**: tuning the hyperparameters of different optimizers (**SGD**, **Adam**, **RMSprop**) using **Bayesian Optimization**.

## 🔍 Project Objective

To evaluate and compare the performance of several optimization algorithms on a forecasting task, by systematically optimizing their hyperparameters and analyzing:

- Prediction accuracy (measured by RMSE)
- Training time
- Memory usage
- Convergence stability

## 🧪 Tools & Technologies

- Python
- Jupyter Notebook
- TensorFlow / Keras
- Optuna (for Bayesian optimization)
- Pandas, NumPy, Seaborn, Matplotlib

## 📁 Files Included

- `Optimisation_Project.ipynb`: Jupyter notebook containing all code for data preprocessing, model building, optimization, and evaluation.
- `your_dataset.csv`: The time series dataset used for training and evaluation.
- Result tables (PDFs and images) and logs (if available)

## ⚙️ Hyperparameters Tuned

The following parameters were explored through Bayesian Optimization:

- `learning_rate`
- `momentum` / `beta1`, `beta2`
- `dropout`
- `batch_size`
- `units`
- `lstm_layers`

## 📊 Results Summary

- **SGD** achieved the best overall RMSE (≈ 0.119) when carefully tuned.
- **Adam** provided faster convergence but less stability.
- **RMSprop** offered consistent but slightly lower performance.

## 📌 Key Takeaways

- Bayesian Optimization is an effective method for exploring hyperparameter spaces.
- Optimizer selection has a significant impact on both accuracy and efficiency.
- Hyperparameter sensitivity varies greatly between optimizers.

## 🚀 Getting Started

To run this notebook:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Optimisation-Project.git
   cd Optimisation-Project
