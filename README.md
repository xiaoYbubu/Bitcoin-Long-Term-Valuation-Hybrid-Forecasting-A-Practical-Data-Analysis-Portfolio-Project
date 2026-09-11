# Bitcoin Long-Term Valuation & Hybrid Forecasting

A practical data analysis project that models Bitcoin’s long-term price trend using a power-law regression, evaluates current valuation with residual Z-scores, and tests a hybrid short-term adjustment model.

**Tools:** Python · pandas · statsmodels · matplotlib

---

## Quick Links

* 📄 **[Download Full PDF Report](./Bitcoin%20Long-Term%20Valuation%20%26%20Hybrid%20Forecast.pdf)**
* 💻 **[View Jupyter Notebook (.ipynb)](./Bitcoin_PowerLaw_Hybrid_Model.ipynb)**

---

## Project Overview

This project answers three practical questions:

1. Does Bitcoin exhibit a stable long-term price structure?
2. Where does the current price sit relative to that structure?
3. Can short-term market factors meaningfully improve near-term forecasts?

The analysis was developed in three stages:
- **Stage 1:** Long-term power-law trend model
- **Stage 2:** Valuation diagnostic using residual Z-score
- **Stage 3:** Hybrid model combining long-term trend with short-term factors

---

## Key Results

| Metric | Value |
|---|---|
| Power-law Model R-squared | **0.830** |
| Adjusted R-squared | 0.829 |
| Estimated Exponent (β) | 4.84 |
| Current Valuation Z-Score | **–0.66** |
| Hybrid Model R-squared | 0.005 |

**Interpretation (as of 5 Sep 2026):**  
Actual price ≈ $79,700 vs. model-implied trend ≈ $110,700.  
The market is moderately below the long-term trend but still within a normal valuation range.

The short-term hybrid model added almost no explanatory power, confirming that long-term structure is more reliable than short-term noise in this dataset.

---

## Visual Results

**Figure 1.** Long-term power-law trend and 95% prediction band  
![Figure 1](./figure1.png)

**Figure 2.** Long-term trend with residual Z-score valuation diagnostic  
![Figure 2](./figure2.png)

**Figure 3.** Hybrid short-term forecast vs. pure power-law baseline (Sep–Dec 2026)  
![Figure 3](./figure3.png)

---

## Full Report

The complete project report (methodology, results, interpretation, and limitations) is available here:

📄 **[Download Full Report (PDF)](./Bitcoin%20Long-Term%20Valuation%20%26%20Hybrid%20Forecast.pdf)**

---

## How to Run the Code

1. Clone this repository or download `.ipynb` file.
2. Install required packages:
```bash
pip install numpy pandas matplotlib statsmodels
