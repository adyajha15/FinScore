# FinScore

## Project Overview

FinScore is an AI-powered financial assessment tool designed to enhance credit risk evaluation, detect fraudulent activities, and predict ESG (Environmental, Social, and Governance) scores for loan applicants. By leveraging a weighted scorecard model, FinScore provides a comprehensive analysis of an applicant’s financial health, sustainability practices, and overall creditworthiness.

### Key Features
- **Credit Risk Assessment:** Predicts the likelihood of loan defaults using historical financial data and key performance indicators.
- **Fraud Detection:** Identifies fraudulent transactions and anomalies to enhance lending security.
- **ESG Score Prediction:** Evaluates an applicant’s sustainability practices based on environmental, social, and governance factors.
- **Loan Approval Prediction:** Combines risk assessment, fraud detection, and ESG scoring to provide a holistic loan approval recommendation.

## Installation

To set up FinScore, follow these steps:

```bash
# Clone the repository
git clone git clone https://github.com/adyajha15/FinScore.git

# Navigate to the project directory
cd FinScore

# Install the required dependencies
pip install -r requirements.txt

# Run the application
python main.py
```

## Usage

1. Upload financial and ESG-related data (currently using synthetic data, but supports expansion to real datasets).
2. The system analyzes credit risk, fraud likelihood, and ESG compliance.
3. View the final credit score and loan approval recommendations through the dashboard.

## Model Explanation

### 1. **Credit Risk Model**
- Uses **XGBoost** for classification.
- Considers historical financial indicators such as income, outstanding debts, payment history, and loan amounts.
- Predicts the probability of loan default using synthetic data (expandable to real data).

### 2. **Fraud Detection Model**
- Implements **anomaly detection techniques** such as Isolation Forest and Local Outlier Factor.
- Identifies suspicious transactions based on spending patterns and transaction history.

### 3. **ESG Score Prediction**
- Utilizes a weighted scoring model based on **World Bank Creditworthiness Methodology and PAS Creditworthiness Assessment Framework**.
- Scores applicants based on sustainability factors such as carbon footprint, ethical business practices, and governance compliance.

## 4. **Sentiment Analysis**
- Dual-model sentiment analysis approach: Gemini API for comprehensive theme analysis and lending risk factors, and TextBlob for numerical sentiment scoring
- Analyzes applicant-provided text data to determine sentiment polarity (positive, neutral, negative). Detects key themes and potential red flags that might indicate financial instability or fraudulent intent.

### 5. **Loan Approval Prediction**
- Integrates outputs from the credit risk model, fraud detection, ESG assessment and sentiment analysis.
- Applies a weighted decision mechanism to determine the final loan approval likelihood.

## Data Considerations
- Currently, **synthetic data** is used to train and test models.
- The system is designed for easy integration with **real financial datasets**.
- Supports **custom data ingestion** for scalability.

## Contributors
- **Adya Jha** 
- **Aditi Rao** 
- **Manavi Jhalani** 

## License
This project is licensed under the MIT License.

---

