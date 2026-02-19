# 💰 Money Muling Detection Challenge

## 📌 Project Title
Money Muling Detection System – AI-Powered Financial Risk Assessment Platform

---

## 🌐 Live Demo URL
https://your-live-demo-link.com

---

## 🛠 Tech Stack

### Backend
- Python
- FastAPI
- Scikit-learn
- Pandas
- NumPy

### Frontend
- React.js
- Tailwind CSS

### Deployment
- Backend: Render
- Frontend: Vercel
- Version Control: GitHub

---

## 🏗 System Architecture

The system follows a client-server architecture:

1. User uploads transaction data (CSV/JSON) via frontend.
2. Frontend sends data to FastAPI backend.
3. Backend:
   - Cleans and preprocesses data
   - Extracts behavioral features
   - Applies ML model for classification
   - Calculates Suspicion Score
4. Backend returns structured JSON response.
5. Frontend displays:
   - Risk Level (Low/Medium/High)
   - Suspicion Score
   - Key behavioral indicators

Architecture Flow:

User → Frontend → API → Feature Engineering → ML Model → Suspicion Score → JSON Response → UI

---

## 🧠 Algorithm Approach

### 1️⃣ Data Preprocessing
- Remove missing values
- Normalize transaction amounts
- Encode categorical variables

Time Complexity: O(n)

---

### 2️⃣ Feature Engineering

Key Features:
- Transaction frequency
- Rapid fund movement detection
- Average transaction amount
- Geographical mismatch
- Account age
- Incoming vs outgoing ratio

Time Complexity: O(n)

---

### 3️⃣ Model Used

- Logistic Regression / Random Forest Classifier
- Supervised learning model trained on labeled mule / non-mule accounts

Training Complexity:
- Logistic Regression: O(n × d)
- Random Forest: O(n log n)

Where:
n = number of samples  
d = number of features  

Prediction Complexity:
O(d)

---

## 🚨 Suspicion Score Methodology

Suspicion Score ranges from 0 to 100.

Formula (Weighted Risk Model):

Suspicion Score =
(0.25 × Transaction Frequency Risk) +
(0.20 × Rapid Movement Risk) +
(0.20 × Amount Anomaly Risk) +
(0.15 × Geographic Risk) +
(0.20 × ML Model Probability × 100)

Risk Levels:

- 0 – 30 → Low Risk
- 31 – 70 → Medium Risk
- 71 – 100 → High Risk

This hybrid approach combines:
- Rule-based detection
- Machine Learning probability
- Behavioral risk scoring

---

## ⚙ Installation & Setup

### 1️⃣ Clone Repository
