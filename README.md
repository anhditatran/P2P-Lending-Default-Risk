# **P2P Lending Default Risk Prediction**

Predicting borrower default using **611k LendingClub loans (2015–2018)**.
Project identifies **key risk factors**, evaluates **predictive models**, and optimizes **investment thresholds** for better returns.

📂 **Dataset:**
[https://drive.google.com/file/d/13OwJaMuMkLtJlXcMkNqbMC2vSbIofcWb/view?usp=sharing](https://drive.google.com/file/d/13OwJaMuMkLtJlXcMkNqbMC2vSbIofcWb/view?usp=sharing)

---

## **Key Insights**

### **1. Financial Stability Predicts Default**

* Higher **DTI**, lower **income**, and renter status → significantly higher default risk.
* Mortgage holders and high-income borrowers are the safest.

### **2. Loan Grade & Purpose Strongly Segment Risk**

* Default rate rises from **6% (Grade A)** → **54% (Grade G)**.
* Highest-risk purposes: **Small Business, Renewable Energy**
* Lowest-risk: **Credit Card, Auto, Education**

### **3. FICO Score Tracks Both Default & Interest Rates**

* Very Good FICO → lowest default rates and interest costs.
* Strong predictor of borrower reliability.

### **4. Verified Borrowers Often Show Higher Risk**

Platforms verify **riskier applicants**, making verification a **risk indicator**, not a guarantee.

### **5. All Models Perform Consistently (~79% Accuracy)**

| Model        | Best Use                                         |
| ------------ | ------------------------------------------------ |
| **Logistic** | Clear risk probabilities                         |
| **Lasso**    | Most interpretable; selects strongest predictors |
| **Ridge**    | Best for correlated features                     |
| **OLS**      | Most detailed explanation of risk drivers        |

### **6. Best Investment Threshold (τ*)**

* **Threshold:** 0.68
* **Profit:** $80.6M
* **ROI:** 19.96%
  Smart investing = **balancing** risk, not avoiding it.

---

## ** Methods**

* Python (pandas, numpy, sklearn, statsmodels)
* Data cleaning & feature engineering
* Logistic, Ridge, Lasso, OLS
* Profit optimization using expected value
* Visual analysis: EDA, distributions, risk patterns

---

## ** Practical Takeaways**

* Prefer **high-grade, low-DTI, verified** borrowers.
* Avoid loans for **small business** or **renewable energy** unless priced well.
* Use predicted probabilities + thresholds to maximize ROI.
* Verification = **screening flag** for high-risk borrowers.

---

## ** Future Work**

* Add ML models (RF, XGBoost)
* Build interactive dashboard
* Include macroeconomic indicators
