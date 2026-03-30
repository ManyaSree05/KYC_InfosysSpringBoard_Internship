# KYC_InfosysSpringBoard_Internship

## 📖 Overview

This project is an AI-powered KYC (Know Your Customer) verification system that automatically verifies identity documents.

Supported documents:

* Aadhaar Card
* PAN Card
* Passport
* Invalid / Non-KYC Documents (Rejected)

The system performs:

* Document Type Detection using Machine Learning
* OCR Text Extraction
* Data Parsing and Structuring
* Fraud Detection using Graph Neural Networks (GNN)
* Final Decision (Approved / Suspicious / Rejected)

---

## 🏗️ System Architecture

User → Frontend (React) → Backend (Node.js) → ML Service (Flask) → Database (MongoDB) → Response → UI

---

## ⚙️ Tech Stack

### Frontend

* React (Vite)
* Axios
* Tailwind CSS

### Backend

* Node.js (Express)
* MongoDB Atlas
* JWT Authentication

### ML Service

* Python (Flask)
* EasyOCR
* TensorFlow / PyTorch
* Graph Neural Networks (GNN)

### Deployment

* AWS EC2 (Backend + ML Service)
* AWS S3 (Frontend Hosting)
* PM2 (Process Manager)

---

## 🔥 Key Features

* Multi-document classification (Aadhaar, PAN, Passport)
* OCR-based data extraction
* GNN-based fraud detection
* Real-time verification dashboard
* Manual review system (Approve / Reject / Suspicious)
* Scalable backend architecture
* Cloud deployment support

---

## 🧠 ML Pipeline

1. Image Upload
2. Document Classification
3. OCR Extraction
4. Data Preprocessing
5. Feature Vector Creation
6. Graph Construction
7. GNN Anomaly Detection
8. Final Decision

---

## 📊 Sample Output

Document Type: PAN Card
Extracted Fields: Name, DOB, PAN Number
Anomaly Score: 2.08
Status: Suspicious

---

## 🚀 Setup Instructions

### 1. Clone Repository

git clone <your-repo-link>
cd KYC_InfosysSpringBoard_Internship

### 2. Backend Setup

cd backend
npm install
npm start

### 3. ML Service Setup

cd ml-service
python -m venv venv
venv\Scripts\activate   (Windows)
pip install -r requirements.txt
python app.py

### 4. Frontend Setup

cd frontend
npm install
npm run dev

---

## ☁️ Deployment

Frontend → AWS S3
Backend → AWS EC2
ML Service → AWS EC2
Database → MongoDB Atlas

---

## 📌 API Endpoints

### Backend

POST /api/auth/login
POST /api/kyc/verify
GET /api/kyc/verifications
GET /api/kyc/verifications/stats

### ML Service

POST /api/ml/classify

---

## 🛡️ Fraud Detection Logic

* Graph-based similarity between documents
* Node = Document
* Edge = Feature similarity
* High anomaly score → Suspicious

---

## 📈 Future Improvements

* Face Matching Integration
* Real-time KYC APIs
* More document types
* Improved OCR accuracy

---

## 🧾 License

This project is for academic and demonstration purposes only.

---

## 🙌 Acknowledgements

* EasyOCR
* MongoDB Atlas
* AWS

---

