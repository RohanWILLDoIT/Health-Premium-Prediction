# Health-Premium-
# 🏥 Health Insurance Premium Prediction

A machine learning-based web application that predicts **health insurance premiums** based on personal, medical, financial, and lifestyle information.

The application is built using **Python, Streamlit, Scikit-learn, XGBoost, Pandas, NumPy, and Joblib** and provides an easy-to-use interface for obtaining an estimated insurance premium.

## 🚀 Live Demo

👉 **[Try the Health Insurance Premium Predictor](https://willdoit-health-premium-prediction.streamlit.app)**

---

## 📌 Project Overview

Health insurance premiums depend on several factors such as:

* Age
* Number of dependants
* Income
* Gender
* Marital status
* BMI
* Smoking habits
* Employment status
* Region
* Medical history
* Genetic risk
* Insurance plan

This project uses machine learning models to analyze these factors and predict an estimated health insurance premium.

The application provides a simple web interface where users can enter their information and receive a predicted premium instantly.

---

## ✨ Features

* 🧑 Personal information-based prediction
* 🏥 Medical history consideration
* 🚬 Smoking status analysis
* 💰 Income-based prediction
* 🧬 Genetic risk consideration
* 📍 Regional information
* 📊 BMI category consideration
* 🛡️ Insurance plan selection
* 🤖 Machine learning-based prediction
* ⚡ Instant prediction through Streamlit
* 🌐 Online deployment using Streamlit Community Cloud

---

## 🧠 Machine Learning Approach

The application uses different models depending on the user's age group.

### Young Users

For users aged **25 or below**, the application uses:

* `model_young.joblib`
* `scaler_young.joblib`

### Other Users

For users aged **above 25**, the application uses:

* `model_rest.joblib`
* `scaler_rest.joblib`

This allows the prediction system to use models specifically prepared for different age groups.

---

## 🔄 Prediction Workflow

```text
User Input
    ↓
Data Preprocessing
    ↓
Categorical Encoding
    ↓
Medical Risk Calculation
    ↓
Feature Scaling
    ↓
Age-Based Model Selection
    ↓
Machine Learning Prediction
    ↓
Predicted Insurance Premium
```

---

## 🏗️ Project Structure

```text
Health-Premium-Prediction/
│
├── artifacts/
│   ├── model_rest.joblib
│   ├── model_young.joblib
│   ├── scaler_rest.joblib
│   └── scaler_young.joblib
│
├── main.py
├── prediction_helper.py
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🛠️ Technologies Used

| Technology                | Purpose                            |
| ------------------------- | ---------------------------------- |
| Python                    | Programming language               |
| Streamlit                 | Web application                    |
| Pandas                    | Data processing                    |
| NumPy                     | Numerical operations               |
| Scikit-learn              | Machine learning and preprocessing |
| XGBoost                   | Machine learning model             |
| Joblib                    | Model serialization                |
| GitHub                    | Version control                    |
| Streamlit Community Cloud | Deployment                         |

---

## 📋 Input Parameters

The application accepts the following information:

### Personal Information

* Age
* Gender
* Marital Status
* Number of Dependants

### Financial Information

* Income in Lakhs
* Insurance Plan

### Medical Information

* Medical History
* Genetic Risk
* BMI Category

### Lifestyle Information

* Smoking Status
* Employment Status

### Location

* Region

---

## ⚙️ How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/rohann1-0/health-premium-prediction.git
```

### 2. Navigate to the project

```bash
cd health-premium-prediction
```

### 3. Create a virtual environment

```bash
python3 -m venv venv
```

### 4. Activate the virtual environment

On macOS/Linux:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the application

```bash
streamlit run main.py
```

The application will open in your browser.

---

## 📦 Requirements

The application uses the following main dependencies:

```text
streamlit
numpy==1.24.3
pandas==2.0.2
scikit-learn==1.3.0
joblib==1.3.2
xgboost
```

The version constraints help maintain compatibility with the serialized machine learning models.

---

## 🔮 How Prediction Works

When the user clicks **Predict**, the application:

1. Collects all user inputs.
2. Converts categorical values into numerical features.
3. Calculates a normalized medical risk score.
4. Selects the appropriate scaler.
5. Scales the required numerical features.
6. Selects a machine learning model based on age.
7. Generates the predicted insurance premium.
8. Displays the result to the user.

---

## 🎯 Objective

The main objective of this project is to demonstrate how machine learning can be integrated into a real-world application to estimate health insurance premiums from multiple user-related factors.

It also demonstrates the complete machine learning deployment workflow:

```text
Data
 ↓
Preprocessing
 ↓
Model Training
 ↓
Model Serialization
 ↓
Streamlit Application
 ↓
Cloud Deployment
```

---

## 🌐 Deployment

The application is deployed using **Streamlit Community Cloud**.

### Live Application

👉 **https://willdoit-health-premium-prediction.streamlit.app**

---

## ⚠️ Disclaimer

This application provides an **estimated insurance premium based on a machine learning model**.

The prediction is for **educational and demonstration purposes only** and should not be considered an actual insurance quotation or financial/medical advice.

---

## 👨‍💻 Author

**Rohan**

B.Tech Student | Machine Learning & Data Science Enthusiast

---

## ⭐ If You Like This Project

If you found this project useful, consider giving the repository a ⭐ on GitHub!
