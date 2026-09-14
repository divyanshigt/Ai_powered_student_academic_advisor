# 🎓 AI-Powered Academic Advisor

An intelligent academic guidance system designed to analyze student academic performance, identify weak subjects, provide personalized recommendations, and generate customized study plans using Artificial Intelligence and Machine Learning.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Key Objectives](#-key-objectives)
- [System Architecture & Workflow](#-system-architecture--workflow)
- [Target User Personas](#-target-user-personas)
- [Functional & Non-Functional Requirements](#-functional--non-functional-requirements)
- [Requirement Traceability Matrix (RTM)](#-requirement-traceability-matrix-rtm)
- [Repository Structure](#-repository-structure)
- [Future Scope & Roadmap](#-future-scope--roadmap)
- [Project Team & Credits](#-project-team--credits)

---

## 📖 Overview

The **AI-Powered Academic Advisor** is an intelligent student-support system that analyzes academic information such as marks, grades, attendance, subject-wise performance, and learning progress.

The system uses **Artificial Intelligence and Machine Learning techniques** to understand a student's academic strengths and weaknesses and provide personalized academic guidance.

Based on the analyzed data, the system can:

- Identify weak and strong subjects
- Analyze overall academic performance
- Detect areas requiring improvement
- Recommend suitable learning resources
- Generate personalized study plans
- Track student progress
- Provide academic insights to faculty/advisors

The objective is to provide students with data-driven academic guidance rather than relying only on generic study recommendations.

---

## 🎯 Key Objectives

- **Academic Performance Analysis:** Analyze student marks, grades, attendance, and academic records.
- **Weak Subject Detection:** Identify subjects and topics where the student requires improvement.
- **Personalized Recommendations:** Generate recommendations based on individual student performance.
- **AI-Based Study Planning:** Create customized study plans according to academic requirements.
- **Learning Resource Recommendation:** Suggest relevant learning materials and resources.
- **Progress Tracking:** Monitor academic improvement over time.
- **Faculty Support:** Help faculty/advisors understand student performance and provide better guidance.
- **Data-Driven Decision Making:** Convert academic data into meaningful insights and actionable recommendations.

---

## 🔄 System Architecture & Workflow

```mermaid
flowchart TD

    A[👨‍🎓 Student] -->|Academic Data| B[Academic Data Management]

    B --> C[Data Preprocessing]

    C --> D[🤖 AI/ML Analysis Engine]

    D --> E{Academic Performance Analysis}

    E -->|Strong Areas| F[Strength Identification]
    E -->|Weak Areas| G[Weak Subject Detection]

    G --> H[Skill / Topic Gap Analysis]

    H --> I[Personalized Recommendation Engine]

    I --> J[📚 Learning Resource Recommendation]
    I --> K[📅 Personalized Study Plan]

    J --> L[Student Dashboard]
    K --> L

    L --> M[📈 Progress Tracking]

    M --> D

    N[👨‍🏫 Faculty / Advisor] -->|Review Performance| L
    O[⚙️ Administrator] -->|Manage Academic Data| B


    Academic Guidance Flow
Stage	System Action	Example
Data Collection	Collect academic information	Marks, grades, attendance
Preprocessing	Clean and prepare academic data	Missing-value handling, normalization
AI Analysis	Analyze student performance	Subject-wise performance
Weak Area Detection	Identify areas requiring improvement	Low performance in DBMS
Recommendation	Generate personalized suggestions	Practice SQL & normalization
Study Planning	Generate customized study plan	2 hours/day DBMS practice
Progress Tracking	Monitor improvement	Compare previous and current scores
👥 Target User Personas
Persona	Role	Key Needs & Goals
Student	Primary User	View performance, identify weak subjects, receive recommendations, follow study plans
Faculty / Advisor	Academic Mentor	Review student performance, monitor progress, provide academic guidance
Administrator	System Manager	Manage users, academic data, courses, subjects, and system information
📋 Functional & Non-Functional Requirements
Functional Requirements (FR)
FR1 — User Registration & Authentication: Allow students, faculty/advisors, and administrators to securely log in to the system.
FR2 — Profile Management: Allow students to create and update their academic profiles.
FR3 — Academic Data Management: Store and manage marks, grades, attendance, subjects, and academic records.
FR4 — Academic Performance Analysis: Analyze student academic performance using available academic data.
FR5 — Weak Subject Detection: Identify subjects or academic areas where the student is performing below the expected level.
FR6 — AI-Based Recommendation: Generate personalized academic recommendations based on student performance.
FR7 — Study Plan Generation: Generate customized study plans according to identified weak areas and student requirements.
FR8 — Learning Resource Recommendation: Recommend relevant learning resources for improvement.
FR9 — Progress Tracking: Track academic progress and compare performance over time.
FR10 — Dashboard & Reports: Display academic performance, recommendations, study plans, and progress through dashboards and reports.
FR11 — Faculty / Advisor Support: Allow faculty/advisors to review student performance and progress.
FR12 — Academic Data Administration: Allow administrators to manage users, courses, subjects, academic data, and system information.
Non-Functional Requirements (NFR)
NFR1 — Security: Student academic information must be protected using secure authentication and access control.
NFR2 — Performance: The system should provide academic analysis and recommendations within an acceptable response time.
NFR3 — Reliability: The system should provide consistent results and remain available during normal usage.
NFR4 — Scalability: The system should support an increasing number of students and academic records.
NFR5 — Usability: The interface should be simple, intuitive, and easy for students and faculty to use.
NFR6 — Accuracy: AI/ML recommendations should provide relevant and meaningful academic guidance.
NFR7 — Maintainability: The system should allow future modification of AI models, academic rules, and recommendation logic.
NFR8 — Privacy: Student academic data should only be accessible to authorized users.
NFR9 — Compatibility: The system should work effectively across commonly used web browsers and devices.
🤖 AI/ML Module

The AI/ML module is the core intelligent component of the AI-Powered Academic Advisor.

AI/ML Workflow
Student Academic Data
        ↓
Data Preprocessing
        ↓
Feature Extraction
        ↓
AI/ML Model
        ↓
Performance Analysis
        ↓
Weak Subject Detection
        ↓
Recommendation Generation
        ↓
Personalized Study Plan
AI/ML Responsibilities
Academic data preprocessing
Feature selection and engineering
Student performance analysis
Weak subject identification
Recommendation logic/model development
Model training and testing
Model evaluation
Personalized recommendation generation
AI module integration with the application
Possible ML Techniques

Depending on the final implementation, the project can use techniques such as:

Classification
Regression
Clustering
Recommendation systems
Performance prediction
🔗 Requirement Traceability Matrix (RTM)
ID	Requirement Description	Target Stakeholders	Priority	Source
FR1	User Registration & Authentication	Student, Faculty, Administrator	High	System Requirement
FR2	Student Profile Management	Student	High	User Requirement
FR3	Academic Data Management	Student, Faculty, Administrator	Critical	Core Specification
FR4	Academic Performance Analysis	Student, Faculty	Critical	Core Specification
FR5	Weak Subject Detection	Student, Faculty	Critical	AI Requirement
FR6	Personalized AI Recommendations	Student	Critical	AI Requirement
FR7	Personalized Study Plan	Student	High	User Requirement
FR8	Learning Resource Recommendation	Student	High	User Requirement
FR9	Progress Tracking	Student, Faculty	High	User Requirement
FR10	Dashboard & Reports	Student, Faculty, Administrator	Medium	System Requirement
FR11	Faculty / Advisor Support	Faculty	High	Stakeholder Requirement
FR12	Academic Data Administration	Administrator	Medium	Admin Requirement
📁 Repository Structure
ai-powered-academic-advisor/
│
├── README.md
│
├── frontend/
│   ├── index.html
│   ├── dashboard.html
│   ├── profile.html
│   ├── recommendations.html
│   └── study-plan.html
│
├── backend/
│   ├── server/
│   ├── routes/
│   ├── controllers/
│   └── models/
│
├── ml/
│   ├── datasets/
│   ├── preprocessing/
│   ├── models/
│   ├── training/
│   └── prediction/
│
├── database/
│   └── schema/
│
├── docs/
│   ├── SRS/
│   ├── UML/
│   └── DFD/
│
└── tests/
    ├── unit/
    └── integration/
🚀 Future Scope & Roadmap
 Train and deploy a dedicated ML model for academic performance prediction.
 Implement advanced personalized recommendation algorithms.
 Add an AI chatbot for student academic queries.
 Integrate real-time academic dashboards.
 Add semester-wise performance prediction.
 Provide topic-level weakness detection.
 Integrate external learning platforms and educational resources.
 Add faculty analytics and early-warning alerts for at-risk students.
 Implement explainable AI to show why a particular recommendation was generated.
 Deploy the complete system on a cloud platform.
👥 Project Team & Credits
Project Title: AI-Powered Academic Advisor
Project Type: Artificial Intelligence / Machine Learning & Academic Guidance System
Version: 1.0
Submission Date: September 2026

### 👨‍💻 Team Members

- **Arya Singh Vats** — AI/ML Developer
- **Shreya Singh** — System Analyst
- **Tanmay Shekhar** — Backend & Database Developer
- **Harshit Singh Bharti** — Frontend & UI/UX Developer
