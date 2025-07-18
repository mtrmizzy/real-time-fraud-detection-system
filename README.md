# 🛡️ **Real-Time Multi-Modal Fraud Detection System**

## 📈 **Project Overview**
This project simulates a **real-time fraud detection system** that processes both **structured transaction data** and **unstructured check images** to classify fraudulent activities.
The system combines **traditional machine learning** with a **computer vision model (CNN)** to detect fraud across multiple data modalities.

---

## 🧰 **Tech Stack**
| **Component**                    | **Tool**                         |
| -------------------------------- | -------------------------------- |
| **Data Streaming**               | Kafka                            |
| **Batch & Streaming Processing** | PySpark                          |
| **Workflow Orchestration**       | Apache Airflow                   |
| **Data Storage**                 | BigQuery / Redshift / PostgreSQL |
| **Model Serving**                | Flask API + Docker + AWS Lambda  |
| **CNN Model (Check Fraud)**      | PyTorch                          |
| **Image Storage**                | AWS S3 / MinIO                   |
| **Cloud Deployment**             | AWS Lambda / Docker Containers   |

---

## 💡 **Key Features**
- **Real-Time Transaction Streaming**
    Stream simulated bank transactions with Kafka.

- **Structured Fraud Detection**
    Train and deploy a traditional ML model (e.g., XGBoost or Random Forest) for transaction anomaly detection.

- **Check Image Fraud Detection**
    Generate synthetic check images and train a CNN model to classify valid vs fraudulent checks.

- **OCR & Image Metadata Pipeline (Bonus)**
    Use OCR (e.g., Tesseract) to extract text from checks and stream metadata into Kafka alongside images.

- **Data Storage & Analytics**
    Store structured and unstructured fraud analysis results in BigQuery, Redshift, or PostgreSQL for querying and reporting.

- **Model Deployment**
    Containerize and deploy models via Flask API, served with Docker and optionally deployed to AWS Lambda.

- **Orchestration & Automation**
    Automate ETL jobs, model retraining, and monitoring with Apache Airflow.

---

## 🚀 **How It Works**
1. **Data Simulation**:
   - Generate fake transactions & check images.
   - Inject fraud cases for model training.
2. **Streaming Pipeline**:
   - Use Kafka to stream transaction data and check metadata (OCR text + S3 path).
3. **Processing & ML Models**:
   - PySpark processes transaction data.
   - CNN processes check images separately.
4. **Unified Prediction API**:
   - Serve both models via Flask API / AWS Lambda.
   - Combine outputs for final fraud decision.
5. **Storage & Reporting**:
   - Store results in BigQuery/Redshift for querying.
   - Visualize insights with optional dashboard tools (Streamlit, Tableau, etc.).

---

## 📈 **Future Enhancements**
- Add **concept drift detection** for model performance monitoring.
- Integrate **model monitoring dashboards** for real-time alerts.
- Deploy end-to-end pipeline to AWS/GCP for full cloud architecture.

---

## 📬 **Contact**
If you'd like to collaborate, discuss this project, or provide feedback, feel free to reach out!

LinkedIn: https://www.linkedin.com/in/marcus-moody-153a83253/

GitHub: [mtrmizzy](https://github.com/mtrmizzy)
