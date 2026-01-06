# 💳 Credit Card Approval Prediction 


> A production‑ready ML system that predicts credit card approval probability *without* triggering a hard credit enquiry. Built for real users and real risk.


## 🔑 Key Insight 
Applicants with **higher income levels** and **stable relationships (having a partner)** show a significantly higher probability of credit card approval.

---

## 📌 Why This Project Matters 
Every hard credit enquiry hurts a user’s credit score.

This application predicts **credit card approval probability** *before* a formal application — allowing users to make informed decisions **without damaging their credit profile**, and enabling financial institutions to:
- Reduce default risk
- Improve applicant filtering
- Align approval strategy with market conditions

This is not just ML — it’s **risk‑aware decision engineering**.

---

## 📊 Data Source
- Kaggle: [Credit Card Approval Prediction Dataset](https://www.kaggle.com/rikdifos/credit-card-approval-prediction)

---

## 🧠 Methodology 
- Exploratory Data Analysis (EDA)
- Bivariate & multivariate analysis
- Feature correlation analysis
- Model benchmarking

---

## ⚙️ Tech Stack
- **Python** — core language
- **Scikit‑Learn** — modeling & evaluation
- **Matplotlib / Seaborn** — visualization

---

### Model Comparison

| Model | Recall |
|------|-------|
| Support Vector Machine | 88% |
| **Gradient Boosting** | **90%** |
| AdaBoost | 79% |

✅ **Final Model Selected:** Gradient Boosting Classifier

---

## 🎯 Metric Strategy — Precision vs Recall (Real‑World Logic)
Choosing the right metric depends on **economic context**:

### 📈 Bull Market
- Low default risk
- Higher tolerance for false positives
- **Recall is preferred** (approve more potential good customers)

### 📉 Bear Market
- High default risk
- Conservative lending
- **Precision is preferred** (avoid risky approvals)

🧠 **Conclusion:**
Given current market assumptions, **Recall** is the most business‑aligned metric for this problem.

---

## 🧪 Key Learnings
- Education level & relationship status are strong predictors
- Capital gain, age & working hours add predictive power
- Occupation & work class contribute the least

### 📌 Recommendation
Prioritize **financial stability indicators** over job titles when assessing applicants.

---

## ⚠️ Limitations & Improvements

- **Dataset Vintage**: Data from 1990s, inflation not adjusted  
  → Solution: Retrain with recent financial datasets

- **Hyperparameter Tuning**: Used RandomSearchCV  
  → Solution: GridSearchCV for marginal gains

---

## 🚀 Run Locally

```bash
git clone https://github.com/Sumit-9826/credit_card_approval_prediction.git
cd Credit-card-approval-prediction-classification
conda env create --prefix <env_name> --file assets/environment.yml
conda activate <env_name>
```

---

## 🗂️ Repository Structure

```
├── datasets/
├── assets/
├── notebooks/
├── requirements.txt
├── README.md
```

---

## 🤝 Contribution
Pull requests are welcome. For major changes, please open an issue to discuss improvements.


---

🔥 **Final Note**
This project demonstrates how **ML + business intuition + clean deployment** can come together to solve a real financial problem — the kind recruiters, fintech teams, and data leaders actually care about.
