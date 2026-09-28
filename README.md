# Stock Market Price Modeling Using Geometric Brownian Motion GBM

## 📌 Project Overview

This project implements **Geometric Brownian Motion (GBM)** to model and simulate the behavior of the Nepal Stock Exchange (NEPSE) index. The study estimates model parameters from historical daily index data and generates simulated price paths to analyze future market scenarios under stochastic dynamics.

The project combines financial mathematics, stochastic calculus, and data analysis to evaluate how well GBM captures real market behavior.

---

## 🎯 Objectives

* Estimate drift (μ) and volatility (σ) from historical NEPSE log-returns
* Implement Geometric Brownian Motion using stochastic differential equations
* Simulate multiple future price paths
* Compare empirical and simulated return distributions
* Evaluate the suitability of GBM for NEPSE modeling

---

## 📚 Mathematical Model

The GBM model is defined by the stochastic differential equation:

[
dS_t = \mu S_t dt + \sigma S_t dW_t
]

where:

* ( S_t ) = Stock price at time ( t )
* ( \mu ) = Drift coefficient
* ( \sigma ) = Volatility coefficient
* ( W_t ) = Standard Brownian motion

The analytical solution is:

[
S_t = S_0 \exp\left((\mu - \tfrac{1}{2}\sigma^2)t + \sigma W_t\right)
]

---

## 🗂 Dataset

* Historical daily NEPSE index data (2020–2025)
* Source: Nepal Stock Exchange (NEPSE)
* Frequency: Daily closing prices

---

## ⚙️ Methodology

1. Collected daily closing index data
2. Computed logarithmic returns
3. Calculated mean and standard deviation of returns
4. Estimated drift (μ) and volatility (σ)
5. Simulated GBM paths using Monte Carlo simulation
6. Compared statistical properties of real vs simulated returns

---

## 📊 Results Summary

* Empirical returns exhibit heavier tails than simulated GBM returns
* GBM captures general trend but underestimates extreme volatility
* Model assumes normality and constant volatility

---

## 🛠 Technologies Used

* Python (NumPy, Pandas, Matplotlib)
* LaTeX (for research paper documentation)
* Stochastic Calculus & Financial Mathematics

---

## 📁 Project Structure

```
GBM-Modeling/
│── data/
│   └── nepse_data.csv
│── notebooks/
│   └── gbm_simulation.ipynb
│── src/
│   └── gbm_model.py
│── figures/
│   └── simulation_plot.png
│── paper/
│   └── research_paper.pdf
│── README.md
```

---



## 👤 Author

Aditya Kumar Sony
BSc Mathematics / Financial Modeling Research
Tribhuvan University

---

## 📄 License

This project is for academic and research purposes.
