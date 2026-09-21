# 🎗️ BreastCare AI — Breast Cancer Early Detection System

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![React](https://img.shields.io/badge/React-Frontend-61DAFB)
![YOLOv8](https://img.shields.io/badge/YOLOv8-AI%20Model-red)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-336791)
![Accuracy](https://img.shields.io/badge/Accuracy-High-brightgreen)

> An AI-powered web platform for image-based breast cancer early detection using deep learning, designed to assist radiologists and healthcare professionals.

---

## 📌 Problem Statement

Breast cancer is one of the most common cancers affecting women worldwide and a leading cause of cancer-related deaths. Manual interpretation of mammograms is time-consuming and subject to human error. **BreastCare AI** addresses this by automating mammogram analysis using state-of-the-art deep learning.

---

## 🎯 Project Objectives

- Detect and classify breast abnormalities from mammogram images using AI
- Classify images as **Benign**, **Malignant**, or **Normal**
- Retrieve visually similar medical cases using embedding-based similarity search
- Provide a secure, multi-role web platform for hospitals, patients, and admins
- Generate automated AI medical reports for radiologists

---

## 🧠 AI & Tech Stack

| Layer | Technology |
|-------|-----------|
| AI Model | YOLOv8 (Object Detection & Classification) |
| Similarity Search | ResNet18 + Cosine Similarity |
| Backend | FastAPI (Python) |
| Frontend | React + TypeScript + shadcn/ui |
| Database | PostgreSQL |
| Auth | JWT Authentication |

---

## 🏗️ System Architecture

```
┌─────────────────┐     ┌──────────────────┐     ┌─────────────────┐
│   React Frontend │────▶│  FastAPI Backend  │────▶│   PostgreSQL DB  │
└─────────────────┘     └──────────────────┘     └─────────────────┘
                                  │
                    ┌─────────────┴──────────────┐
                    │         AI Services         │
                    │  ┌─────────┐ ┌──────────┐  │
                    │  │ YOLOv8  │ │ ResNet18 │  │
                    │  │Detection│ │Similarity│  │
                    │  └─────────┘ └──────────┘  │
                    └────────────────────────────┘
```

---

## 📁 Project Structure

```
Breast-Cancer-Graduation-Project/
├── AI/
│   ├── YoloModel.ipynb          # YOLO model training notebook
│   └── README.txt
├── Backend - Frontend/
│   ├── backend/
│   │   ├── app/
│   │   │   ├── models/          # Database models
│   │   │   ├── routes/          # API endpoints
│   │   │   ├── schemas/         # Pydantic schemas
│   │   │   └── services/        # AI & business logic
│   │   └── requirements.txt
│   ├── front end/
│   │   ├── src/
│   │   │   ├── app/components/  # React components
│   │   │   └── services/        # API services
│   │   └── package.json
│   └── databasepg.sql           # Database schema
├── DEMO.mp4                     # System demo video
├── Final graduation Presentation.pptx
├── graduation project thesis.pdf
├── IEEE 829 TEST PLAN.docx
└── Project summary.docx
```

---

## 👥 User Roles

| Role | Permissions |
|------|------------|
| 🏥 Hospital | Manage patients, radiologists, and mammogram uploads |
| 👤 Patient | View own medical reports and AI results |
| 🔧 Admin | Full system management and audit logs |

---

## 🔬 Datasets Used

- **BUSI** — Breast Ultrasound Images Dataset
- **CBIS-DDSM** — Curated Breast Imaging Subset of DDSM
- **Kaggle Breast Ultrasound Dataset**

---

## 👨‍💻 Team Members

| Name | Specialization |
|------|---------------|
| Omar Khaled Shaker | Computer Science (CS) |
| Seif Mohamed | Software Engineering (SE) |
| Omar Mahrous | Information Systems (IS) |
| Youssef Abdullah | Artificial Intelligence (AI) |
| Mohammed Karim | Artificial Intelligence (AI) |
| Moemen Ayman | Software Engineering (SE) |

---

## 🎓 Academic Info

- **Institution:** Arab Academy for Science, Technology and Maritime Transport
- **College:** College of Computing and Information Technology
- **Supervisor:** Dr. Hanan Ali
- **Year:** June 2026

---

## 📄 License

This project was developed as a B.Sc. Final Year Graduation Project. All rights reserved © 2026.
