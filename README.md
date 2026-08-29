# 🧠 Mental Health Score Prediction

<p align="center">
  🚀 Machine Learning | ⚡ FastAPI | 🌐 Web Application | 🤖 Predictive Model
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikit-learn">
  <img src="https://img.shields.io/badge/FastAPI-Backend-green?style=for-the-badge&logo=fastapi">
  <img src="https://img.shields.io/badge/HTML-CSS-JS-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge">
</p>

---

## 📌 About The Project

**Mental Health Score Prediction** is a Machine Learning powered web application that predicts a mental health score based on lifestyle, social media usage, and other relevant input factors.

The project combines a trained Machine Learning model with a **FastAPI backend** and a **HTML, CSS, and JavaScript frontend**.

Users can enter the required information through the web interface, and the application sends the data to the backend, where the trained model generates a prediction.

---

## 🎯 Project Objective

The main objective of this project is to build an end-to-end Machine Learning application that can:

* Analyze relevant mental health factors
* Process user input
* Predict a mental health score
* Provide predictions through a web interface
* Connect a Machine Learning model with a REST API
* Demonstrate the complete ML-to-Web workflow

---

## 🧠 Machine Learning

The Machine Learning workflow includes:

* Data Loading
* Data Understanding
* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Categorical Encoding
* Numerical Preprocessing
* Train-Test Split
* Model Training
* Model Evaluation
* Hyperparameter Tuning
* Model Saving

The trained model is saved as:

```text
model.pkl
```

---

## 🤖 Model

The application uses a trained Scikit-Learn Machine Learning model for predicting the mental health score.

The saved model is loaded by the FastAPI backend and used to generate predictions from user input.

```python
import joblib

model = joblib.load("model.pkl")
prediction = model.predict(data)
```

---

## ⚡ FastAPI Backend

**FastAPI** is used to create the backend API that connects the frontend with the Machine Learning model.

### API responsibilities

* Load the trained model
* Receive user input
* Validate input data
* Send data to the ML model
* Generate predictions
* Return prediction results to the frontend

Example API endpoint:

```text
POST /predict
```

A health-check endpoint can also be used:

```text
GET /health
```

---

## 🛡️ Data Validation

The API validates incoming data before sending it to the Machine Learning model.

This helps prevent invalid or unexpected values from reaching the prediction pipeline.

---

## 🌐 Frontend

The frontend is built using:

* HTML
* CSS
* JavaScript

Users can enter the required information through the web interface and receive the predicted mental health score.

### Frontend workflow

```text
User Input
    ↓
HTML Form
    ↓
JavaScript fetch()
    ↓
FastAPI /predict
    ↓
Machine Learning Model
    ↓
Prediction
    ↓
Frontend Result
```

---

## 🔄 Complete Project Architecture

```text
                    ┌─────────────────────┐
                    │      User           │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ HTML / CSS / JS     │
                    │     Frontend        │
                    └──────────┬──────────┘
                               │
                         HTTP Request
                               │
                               ▼
                    ┌─────────────────────┐
                    │      FastAPI        │
                    │      Backend        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Data Validation   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   ML Model (.pkl)   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Mental Health Score │
                    │     Prediction      │
                    └─────────────────────┘
```

---

## 📊 Model Evaluation

The Machine Learning model can be evaluated using regression metrics such as:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

These metrics help measure the prediction performance of the model.

---

## 🛠️ Technologies Used

### Machine Learning

* Python
* Pandas
* NumPy
* Scikit-Learn
* Joblib

### Data Visualization

* Matplotlib
* Seaborn

### Backend

* FastAPI
* Pydantic
* Uvicorn

### Frontend

* HTML5
* CSS3
* JavaScript

### Development

* Jupyter Notebook
* Git
* GitHub

---

## 📂 Project Structure

```text
Mental-Health-Score/
│
├── ML_Project.ipynb
├── Student Social Media And Mental Health Impact.csv
├── Mental_Health_Model.pkl
│
├── main.py
├── requirements.txt
│
├── index.html
├── style.css
├── script.js
│
├── ML Project.html
├── README.md
└── .gitignore
```

---

## 🚀 How To Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/haseebniazii/Mental-Health-Score.git
```

### 2. Open the project directory

```bash
cd Mental-Health-Score
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the environment

**Windows:**

```bash
venv\Scripts\activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Start FastAPI

```bash
uvicorn main:app --reload
```

### 7. Open the application

Open the local URL shown by Uvicorn in your browser.

---

## 📡 API Documentation

Once the FastAPI server is running, interactive API documentation is available through:

```text
/docs
```

FastAPI automatically provides interactive API documentation for testing the endpoints.

---

## ☁️ Deployment

The application can be deployed as a web service using platforms such as **Render**.

Deployment workflow:

```text
GitHub Repository
       ↓
    Render
       ↓
FastAPI Application
       ↓
Live Web Application
```

---

## 🔮 Future Improvements

* Improve model performance
* Add more advanced Machine Learning models
* Perform additional hyperparameter tuning
* Add authentication
* Improve frontend UI/UX
* Add prediction history
* Add model performance dashboard
* Deploy with a production-grade setup

---

## ⚠️ Disclaimer

This project is created for **educational and Machine Learning demonstration purposes**.

The predicted score should not be considered a medical diagnosis or professional mental-health assessment.

---

## 👨‍💻 Author

**Haseeb Khan**

GitHub:
https://github.com/haseebniazii

---

⭐ If you found this project useful, consider giving the repository a star!
