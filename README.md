# 🧠 Probit Regression on Heart Disease Risk – Fisher Scoring & MCMC

This project implements and compares two approaches to binary Probit regression: a frequentist **Fisher Scoring algorithm** and a **Bayesian Gibbs Sampling method** using Markov Chain Monte Carlo (MCMC). The models are applied to the **SAheart dataset** to analyze the relationship between cholesterol levels and the risk of coronary heart disease (CHD).

## 📁 Files

- `FINALprojectFisher_&_MCMC.ipynb` – Jupyter notebook with full implementation
- `Stats_Final_Project.pdf` – Detailed project report and model derivations
- `SAheart.txt` - dataset

## 📊 Summary

### 1. Fisher Scoring (Frequentist Approach)
- Implemented a custom Probit regression algorithm using Fisher Scoring
- Estimated parameters via iteratively reweighted least squares (IRLS)
- Used Monte Carlo simulation to approximate the standard normal CDF

### 2. Bayesian Probit Regression (Gibbs Sampling)
- Augmented the model using latent variables (Albert & Chib, 1993)
- Used Gibbs sampling to draw from the posterior of parameters
- Diagnosed convergence via trace plots and autocorrelation

### 3. Key Finding
- Higher LDL cholesterol is positively associated with CHD risk  
  → Average marginal effect ≈ **+3%** per unit increase in cholesterol  
  → Having family history adds ~**+15.5%** probability of CHD

## 🔧 Tools & Libraries
- Python (NumPy, SciPy, matplotlib, pandas, statsmodels)
- Custom implementation of truncated normal sampling
- No external ML libraries used for model fitting

## 📌 Notes
- This analysis is **correlational**, not causal.
- The implementation builds both from scratch and validated with `statsmodels`.

## 📚 References
- Albert, J. H., & Chib, S. (1993). *Bayesian Analysis of Binary and Polychotomous Response Data*
- SAheart dataset (Statistical Learning with Sparsity, 2015)

---

📈 *This project was completed as part of a university course in Statistics and Probability course.*
