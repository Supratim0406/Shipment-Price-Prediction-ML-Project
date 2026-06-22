# 🚚 Shipment Price Prediction - End-to-End Machine Learning Project

## 📌 Project Overview

Shipment pricing plays a critical role in logistics and supply chain management. Accurately predicting shipment costs helps businesses optimize transportation expenses, improve budgeting, and enhance operational efficiency.

This project builds an end-to-end Machine Learning pipeline to predict shipment prices based on shipment characteristics such as origin, destination, weight, transportation mode, customer information, and other logistics-related features.

The project follows a production-grade architecture with modular components for data ingestion, validation, transformation, model training, and evaluation.

---

## 🎯 Business Problem

Logistics companies often struggle to estimate shipment costs accurately due to multiple influencing factors.

The objective of this project is to:

* Predict shipment prices with high accuracy.
* Automate the machine learning workflow.
* Detect data quality issues before model training.
* Enable scalable deployment and future MLOps integration.

---

## 🛠️ Tech Stack

### Programming Language

* Python 3.11

### Libraries

* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* CatBoost
* LightGBM
* Evidently AI
* PyMongo
* PyYAML

### Database

* MongoDB Atlas

### MLOps Tools

* MLflow
* DVC
* GitHub Actions

### Cloud (Future Scope)

* AWS S3
* AWS EC2
* AWS ECS/Fargate

---

## 📂 Project Structure

```bash
Shipment-Price-Prediction-ML-Project/
│
├── artifacts/
├── config/
├── notebook/
├── shipment/
│   ├── components/
│   ├── configuration/
│   ├── constants/
│   ├── entity/
│   ├── exception/
│   ├── logger/
│   ├── pipeline/
│   └── utils/
│
├── requirements.txt
├── demo.py
├── main.py
└── README.md
```

## ⚙️ ML Pipeline Workflow

### 1️⃣ Data Ingestion

* Connects to MongoDB Atlas
* Reads shipment dataset
* Splits data into train and test datasets
* Stores artifacts locally

### 2️⃣ Data Validation

* Validates schema consistency
* Checks missing values
* Detects data drift using Evidently AI
* Generates validation reports

### 3️⃣ Data Transformation

* Feature engineering
* Missing value handling
* Encoding categorical variables
* Feature scaling
* Creation of preprocessing pipeline

### 4️⃣ Model Training

Models evaluated:

* Random Forest Regressor
* XGBoost Regressor
* CatBoost Regressor
* LightGBM Regressor
* Gradient Boosting Regressor

Best-performing model is automatically selected.

### 5️⃣ Model Evaluation

Evaluation Metrics:

* R² Score
* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* RMSE (Root Mean Squared Error)

### 6️⃣ Model Persistence

* Saves trained model
* Saves preprocessing pipeline
* Stores artifacts for deployment

---

## 🗄️ MongoDB Setup

Create a `.env` file:

```env
MONGO_DB_URL=your_mongodb_connection_string
```

Upload the shipment dataset to your MongoDB Atlas cluster.

---

## 🚀 Installation

### Clone Repository

```bash
git clone <your-repository-url>
cd Shipment-Price-Prediction-ML-Project
```

### Create Environment

```bash
conda create -n shipment python=3.11 -y
conda activate shipment
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run Training Pipeline

```bash
python demo.py
```

or

```bash
python main.py
```

---

## 📈 Future Improvements

* MLflow Experiment Tracking
* DVC Data Versioning
* Docker Containerization
* CI/CD with GitHub Actions
* AWS Deployment (ECS/Fargate)
* Real-Time Prediction API using FastAPI
* Monitoring with Evidently AI

---

## 📊 Key Features

✅ End-to-End ML Pipeline

✅ MongoDB Atlas Integration

✅ Automated Data Validation

✅ Data Drift Detection

✅ Modular Production-Ready Code

✅ Artifact-Based Pipeline Design

✅ MLOps Ready Architecture

---

## 👨‍💻 Author

**Supratim Saha**

Aspiring Data Scientist | Machine Learning Engineer | MLOps Enthusiast

GitHub: https://github.com/Supratim0406

LinkedIn: Add Your LinkedIn Profile

---

⭐ If you found this project useful, consider giving it a star on GitHub.
