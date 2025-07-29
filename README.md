# Capstone-Project
# AAVAIL Demand Forecasting and Recommender System

This project is a capstone solution that demonstrates how to forecast demand and recommend content for a video streaming company (AAVAIL) using machine learning. The solution includes a Flask-based API, performance monitoring, unit testing, and containerization with Docker.

## 📌 Project Goals

- Forecast future demand (views, purchases, revenue) for different countries and dates
- Enable content recommendation based on user behavior
- Deploy a prediction API using Flask
- Monitor performance and detect anomalies or data drift
- Containerize the solution for easy deployment and reproducibility

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **Flask** – RESTful API
- **scikit-learn** – Machine Learning models
- **pandas / numpy** – Data preprocessing
- **matplotlib / seaborn / plotly** – Visualizations
- **pytest** – Unit testing
- **Docker** – Containerization
- **Git** – Version control

---

## 📁 Repository Structure

```bash
.
├── app/
│   ├── api.py                # Flask API with prediction endpoints
│   ├── model.py              # ML model loading and prediction logic
│   ├── utils.py              # Helper functions for processing
│   ├── logger.py             # Logging configuration
│   └── config.py             # Configuration file
│
├── tests/
│   ├── test_api.py           # Unit tests for API
│   ├── test_model.py         # Unit tests for model
│   └── test_logging.py       # Unit tests for logging
│
├── data/
│   ├── raw/                  # Raw data files (JSON, CSV, etc.)
│   └── processed/            # Cleaned and transformed data
│
├── notebooks/
│   ├── eda.ipynb             # Exploratory Data Analysis
│   └── model_comparison.ipynb  # Model training and evaluation
│
├── Dockerfile                # For building the Docker image
├── requirements.txt          # Python dependencies
├── ingest_data.py            # Data ingestion script
├── run.py                    # Entry point to start the Flask app
├── README.md                 # This file
└── .gitignore
