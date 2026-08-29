# 🧠 Mental Health Score Prediction

<p align="center">
  🚀 Machine Learning | ⚡ FastAPI | 🌐 Web Application | 🤖 Predictive Model
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikit-learn">
  <img src="https://img.shields.io/badge/FastAPI-Backend-green?style=for-the-badge&logo=fastapi">
  <img src="https://img.shields.io/badge/GitHub%20Pages-Frontend-black?style=for-the-badge&logo=github">
</p>

---

## 📌 About The Project

**Mental Health Score Prediction** is a Machine Learning web application that predicts a mental health score based on lifestyle habits, academic activities, screen time, social media usage, sleep, physical activity, and perceived stress.

The project combines:

* 🤖 Machine Learning
* ⚡ FastAPI backend
* 🌐 HTML, CSS & JavaScript frontend
* 🐙 GitHub Pages deployment

Users enter their information through the web interface, and the data is sent to the FastAPI backend. The trained Machine Learning model processes the input and returns a predicted mental health score.

> ⚠️ This project is for educational and demonstration purposes only. It is not a medical or clinical assessment.

---

## 🌐 Live Demo

### Frontend

🔗 **Live Website:**

https://haseebniazii.github.io/Mental-Health-Score/

The frontend is hosted using **GitHub Pages**.

### Backend

The FastAPI backend is designed to receive prediction requests from the frontend and run the trained Machine Learning model.

---

## 🎯 Project Objective

The main objective of this project is to demonstrate a complete **Machine Learning → API → Web Application** workflow.

The application can:

* Analyze lifestyle and digital habits
* Process user input
* Predict a mental health score
* Provide predictions through a web interface
* Connect a Machine Learning model with a REST API
* Demonstrate an end-to-end ML deployment workflow

---

## 🧠 Machine Learning Workflow

The Machine Learning workflow includes:

1. Data Loading
2. Data Understanding
3. Data Cleaning
4. Exploratory Data Analysis
5. Feature Engineering
6. Categorical Encoding
7. Numerical Preprocessing
8. Train-Test Split
9. Model Training
10. Model Evaluation
11. Hyperparameter Tuning
12. Model Saving

The trained model is saved as:

```text
Mental_Health_Model.pkl
```

---

## 🤖 Machine Learning Model

The application uses a trained **Scikit-Learn regression model** to predict a mental health score.

The saved model is loaded by the FastAPI backend.

Example:

```python
import joblib

model = joblib.load("Mental_Health_Model.pkl")

prediction = model.predict(data)
```

---

## ⚡ FastAPI Backend

**FastAPI** is used to create the REST API that connects the frontend with the Machine Learning model.

### API Responsibilities

* Receive user input
* Validate input data
* Load the trained model
* Process prediction data
* Generate the mental health score
* Return the prediction to the frontend

### Prediction Endpoint

```text
POST /predict
```

### Health Check

```text
GET /health
```

### API Documentation

When running locally, FastAPI provides interactive documentation at:

```text
/docs
```

---

## 🌐 Frontend

The frontend is built using:

* HTML5
* CSS3
* JavaScript

The interface allows users to enter:

* Age
* Gender
* Country
* Academic level
* Most-used social media platform
* Primary purpose of social media
* Average daily screen time
* Daily phone unlocks
* Study hours
* Physical activity
* Sleep hours
* Perceived stress level

The frontend then sends the data to the FastAPI `/predict` endpoint.

---

## 🔄 Application Workflow

```text
                    👤 User
                       │
                       ▼
              ┌─────────────────┐
              │  HTML/CSS/JS    │
              │    Frontend     │
              └────────┬────────┘
                       │
                       │ POST /predict
                       ▼
              ┌─────────────────┐
              │     FastAPI     │
              │     Backend     │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Data Validation │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │  ML Model .pkl  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Mental Health   │
              │ Score Prediction│
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Frontend Result │
              └─────────────────┘
```

---

## 📊 Model Evaluation

The regression model can be evaluated using:

* MAE — Mean Absolute Error
* MSE — Mean Squared Error
* RMSE — Root Mean Squared Error
* R² Score

These metrics help evaluate how accurately the model predicts the target score.

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

### Deployment

* GitHub
* GitHub Pages
* Render

### Development

* Jupyter Notebook
* Git
* GitHub

---

## 📂 Project Structure

```text
Mental-Health-Score/
│
├── Mental Health Score/
│   ├── Student Mental Health Score.ipynb
│   ├── Mental Health.csv
│   ├── Mental_Health_Model.pkl
│   │
│   ├── main.py
│   ├── requirements.txt
│   │
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   │
│   └── ML Project.html
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🚀 Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/haseebniazii/Mental-Health-Score.git
```

### 2. Open the project

```bash
cd Mental-Health-Score
```

### 3. Enter the project folder

```bash
cd "Mental Health Score"
```

### 4. Create virtual environment

```bash
python -m venv venv
```

### 5. Activate virtual environment

**Windows:**

```bash
venv\Scripts\activate
```

### 6. Install dependencies

```bash
pip install -r requirements.txt
```

### 7. Start FastAPI

```bash
uvicorn main:app --reload
```

### 8. Open the application

Open:

```text
http://127.0.0.1:8000
```

API documentation:

```text
http://127.0.0.1:8000/docs
```

---

## ☁️ Deployment Architecture

The frontend and backend can be deployed separately.

```text
                 GitHub
                   │
          ┌────────┴────────┐
          │                 │
          ▼                 ▼
   GitHub Pages          Render
          │                 │
          ▼                 ▼
     HTML/CSS/JS         FastAPI
          │                 │
          └────────┬────────┘
                   │
                   ▼
              ML Model
              (.pkl)
                   │
                   ▼
          Mental Health Score
```

### Frontend

The static frontend is hosted on GitHub Pages:

https://haseebniazii.github.io/Mental-Health-Score/

### Backend

The FastAPI backend can be deployed separately as a web service on Render.

---

## 🔮 Future Improvements

* Improve model performance
* Compare multiple ML algorithms
* Perform additional hyperparameter tuning
* Add prediction history
* Add model performance dashboard
* Improve frontend UI/UX
* Add authentication
* Add database integration
* Deploy the complete backend
* Add more useful wellness insights

---

## ⚠️ Disclaimer

This project is created for **educational and Machine Learning demonstration purposes**.

The predicted score should **not** be considered a medical diagnosis, clinical assessment, or professional mental-health evaluation.

If you are experiencing serious mental-health difficulties, consider speaking with a qualified healthcare professional or someone you trust.

---

## 👨‍💻 Author

### Haseeb Khan

GitHub:

https://github.com/haseebniazii

---

## ⭐ Support

If you found this project useful, please consider giving the repository a ⭐ star.

**Thank you for checking out the project!**
