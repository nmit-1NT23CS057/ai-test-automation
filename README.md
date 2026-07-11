# 🤖 AI-Powered Intelligent Software Testing Framework

An AI-driven software testing framework that automates requirement analysis, test case generation, prioritization, defect prediction, auto-triage, and API response prediction using Natural Language Processing (NLP) and Machine Learning (ML).

The framework reduces manual testing effort by converting software requirements into actionable test cases, prioritizing them based on risk, predicting defect categories from failure logs, automatically assigning defects to the appropriate teams, and estimating API response performance.

---

## 🚀 Features

### 📄 Requirement Analysis
- Reads Software Requirement Specification (SRS) documents
- Uses NLP (spaCy) to extract requirement statements
- Identifies functional requirements containing keywords such as:
  - should
  - must
  - shall

---

### ✅ Automatic Test Case Generation
- Converts extracted requirements into structured test cases
- Generates:
  - Test Case ID
  - Requirement
  - Description
  - Step-by-step execution procedure
- Exports generated test cases to CSV

---

### 🎯 AI-Based Test Case Prioritization
- Uses Machine Learning (Random Forest Classifier)
- Assigns risk scores to test cases based on:
  - Historical defects
  - Execution time
  - Failure probability
- Prioritizes high-risk test cases first

---

### 🐞 Defect Prediction & Root Cause Analysis
Predicts the type of software defect from execution logs.

Supported categories:

- Code Defect
- Environment Issue
- Flaky Test

Uses:

- TF-IDF Vectorization
- Logistic Regression
- Rule-based Hybrid Prediction

---

### ⚡ Test Failure Auto-Triage
Automatically assigns failed test cases to the responsible team.

Example:

| Defect Type | Assigned Team |
|-------------|---------------|
| Code Defect | Developer Team |
| Environment Issue | DevOps Team |
| Flaky Test | QA Team |

---

### 🌐 AI-Based API Testing
Predicts API response times using machine learning.

Features:

- Response time estimation
- Performance anomaly detection
- API latency prediction

---

## 🧠 Machine Learning Models

| Module | Algorithm |
|----------|------------------------------|
| Test Prioritization | Random Forest Classifier |
| Defect Prediction | Logistic Regression |
| Auto-Triage | Multinomial Naive Bayes |
| API Response Prediction | Random Forest Regressor |

---

## 🛠️ Technologies Used

### Programming Language

- Python 3.x

### NLP

- spaCy

### Machine Learning

- Scikit-Learn

### Data Processing

- Pandas
- NumPy

### Visualization

- Jupyter Notebook

---

## 📂 Project Structure

```
AI-Software-Testing/
│
├── data/
│   ├── sample_requirements.txt
│   ├── generated_test_cases.csv
│   ├── prioritized_test_cases.csv
│   ├── auto_triaged_failures.csv
│   └── api_response_predictions.csv
│
├── notebooks/
│   ├── requirement_analysis.ipynb
│   ├── prioritization.ipynb
│   ├── defect_prediction.ipynb
│   ├── auto_triage.ipynb
│   └── api_testing.ipynb
│
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI-Software-Testing.git

cd AI-Software-Testing
```

Install dependencies

```bash
pip install -r requirements.txt
```

Download spaCy model

```bash
python -m spacy download en_core_web_sm
```

---

## ▶️ Running the Project

### Requirement Analysis

```bash
python requirement_analysis.py
```

Generates:

```
generated_test_cases.csv
```

---

### Test Prioritization

```bash
python test_prioritization.py
```

Generates:

```
prioritized_test_cases.csv
```

---

### Defect Prediction

```bash
python defect_prediction.py
```

Predicts defect categories from failure logs.

---

### Auto-Triage

```bash
python auto_triage.py
```

Assigns defects to:

- QA Team
- Developer Team
- DevOps Team

---

### API Testing

```bash
python api_testing.py
```

Outputs:

```
Predicted Response Time
Performance Anomaly Detection
```

---

## 📊 Sample Outputs

### Generated Test Cases

| Test Case | Description |
|------------|-------------|
| TC_001 | Secure authentication |
| TC_002 | Login validation |
| TC_003 | Account lock after failed attempts |

---

### Prioritized Test Cases

| Test Case | Risk Score |
|------------|------------|
| TC_012 | 1.00 |
| TC_014 | 1.00 |
| TC_002 | 1.00 |

---

### Defect Prediction

Input Log

```
API timeout during request
```

Prediction

```
Environment Issue
```

---

### Auto-Triage

```
NullPointerException

↓

Developer Team
```

---

### API Prediction

```
GET /users?id=2

↓

Predicted Response Time:
132 ms
```

---

## 📈 Future Enhancements

- Large Language Model (LLM)-based requirement understanding
- Selenium integration for automated UI testing
- Jenkins CI/CD integration
- Real-time dashboard using Streamlit
- REST API support with FastAPI
- Test case recommendation system
- Deep learning-based defect prediction
- Support for Playwright and Cypress

---

## 🎯 Applications

- Software Quality Assurance
- Agile Testing
- Regression Testing
- Continuous Integration / Continuous Deployment (CI/CD)
- Intelligent Test Automation
- Software Reliability Engineering

---

## 📚 Libraries Used

- pandas
- numpy
- scikit-learn
- spacy
- matplotlib
- jupyter

---
