# Interest Rate Modeling using Vasicek and Hull-White Models

## Project Objective

This project aims to estimate interest rates for non-standard tenors (3.5, 4.5, and 5.5 years) using short-rate models:
- **Vasicek Model**
- **Hull-White Model**

We calibrate both models using the Indian **MIBOR (Mumbai Interbank Offered Rate)** data from the past 2 years and evaluate their performance in estimating yield curves for the specified maturities.

---

## Data Source

- Indian MIBOR Overnight Rate from [FBIL](https://fbil.org.in)
- Time Period: Last 2 Years (e.g., May 2023 – May 2025)

---

## Methodology

### 1. **Data Cleaning & Preprocessing**
- Fill or remove missing values
- Calculate daily changes in MIBOR

### 2. **Model Calibration**
#### Vasicek:
\[ dr_t = a(b - r_t)dt + \sigma dW_t \]

#### Hull-White:
\[ dr_t = (\theta(t) - a r_t)dt + \sigma dW_t \]

- Estimate parameters `a`, `b`, and `σ` using regression

### 3. **Yield Curve Estimation**
- Use closed-form solutions for zero-coupon bond pricing
- Derive yields for 3.5, 4.5, and 5.5 years

### 4. **Comparison**
- Visualize yield curves
- Discuss which model is better and why

---

## Outputs

- Yield curve plots (Vasicek vs. Hull-White)
- Excel model for non-programming understanding
- Python notebook for full implementation
- Analytical comparison and conclusion

---

## Repository Structure


