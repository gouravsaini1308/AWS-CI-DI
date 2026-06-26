# 🚀 Student Performance Prediction | AWS CI/CD Deployment

A complete End-to-End Machine Learning project that predicts a student's **Math Score** based on demographic and academic features. The project demonstrates the complete ML lifecycle, from model training to deployment using **Docker**, **AWS EC2**, **GitHub Actions**, and **AWS ECR**.

---

## 📌 Project Overview

This project predicts the **Math Score** of a student using the following features:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

The trained machine learning model is deployed as a Flask web application and automated using a CI/CD pipeline.

---

## ✨ Features

- End-to-End Machine Learning Pipeline
- Data Ingestion
- Data Validation
- Data Transformation
- Model Training
- Prediction Pipeline
- Flask Web Application
- Docker Containerization
- AWS EC2 Deployment
- AWS Elastic Container Registry (ECR)
- GitHub Actions CI/CD Pipeline

---

## 🛠️ Tech Stack

### Programming Language
- Python 3.11

### Libraries
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- CatBoost
- XGBoost
- Flask
- Dill

### DevOps & Cloud
- Docker
- AWS EC2
- AWS ECR
- GitHub Actions
- Git
- GitHub

---

# 📂 Project Structure

```
AWS-CI-CD-Projects/
│
├── artifacts/
│   ├── model.pkl
│   ├── preprocessor.pkl
│   ├── train.csv
│   ├── test.csv
│   └── raw.csv
│
├── notebook/
│   ├── EDA STUDENT PERFORMANCE.ipynb
│   ├── MODEL TRAINING.ipynb
│   └── data/
│
├── src/
│   ├── components/
│   ├── pipeline/
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── templates/
│   ├── home.html
│   └── index.html
│
├── .github/
│   └── workflows/
│
├── app.py
├── Dockerfile
├── requirements.txt
└── setup.py
```

---

# ⚙️ Installation

## Clone the Repository

```bash
git clone https://github.com/gouravsaini1308/AWS-CI-CD-Projects.git
```

```bash
cd AWS-CI-CD-Projects
```

---

## Create Virtual Environment

Windows

```bash
python -m venv venv
venv\Scripts\activate
```

Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Application

```bash
python app.py
```

Open your browser and visit

```
http://localhost:5000
```

---

# 🐳 Docker

## Build Docker Image

```bash
docker build -t student-performance .
```

## Run Docker Container

```bash
docker run -d -p 5000:5000 student-performance
```

---

# ☁️ AWS Deployment

The application is deployed using the following AWS services:

- Amazon EC2
- Amazon ECR
- GitHub Actions

Deployment Workflow

```
GitHub
    │
    ▼
GitHub Actions
    │
    ▼
Build Docker Image
    │
    ▼
Push Image to AWS ECR
    │
    ▼
EC2 Pulls Latest Image
    │
    ▼
Docker Container Starts Automatically
```

---

# 🔄 CI/CD Pipeline

The project uses **GitHub Actions** for Continuous Integration and Continuous Deployment.

Pipeline Steps

- Checkout Repository
- Install Dependencies
- Build Docker Image
- Authenticate with AWS
- Push Docker Image to AWS ECR
- Pull Latest Image on EC2
- Stop Previous Container
- Run Updated Container

---

# 📊 Machine Learning Workflow

```
Data Collection
        │
        ▼
Data Ingestion
        │
        ▼
Data Transformation
        │
        ▼
Feature Engineering
        │
        ▼
Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Model Serialization
        │
        ▼
Prediction Pipeline
        │
        ▼
Flask Web Application
        │
        ▼
Docker Deployment
        │
        ▼
AWS EC2
```

---

# 📸 Application

The web application allows users to enter student details and predict the expected Math Score.

Input Features

- Gender
- Race/Ethnicity
- Parent Education
- Lunch
- Test Preparation Course
- Reading Score
- Writing Score

Output

- Predicted Math Score

---

# 📦 Requirements

```
Python >= 3.11
Flask
scikit-learn
Pandas
NumPy
CatBoost
XGBoost
Docker
AWS CLI
```

---

# 👨‍💻 Author

**Gourav Saini**

GitHub: https://github.com/gouravsaini1308

LinkedIn: https://www.linkedin.com/in/gouravsaini1308/

---

# ⭐ If you found this project useful, consider giving it a Star!
