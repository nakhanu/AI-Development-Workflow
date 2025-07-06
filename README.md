# AI Development Workflow – Week 5 Assignment

This repository contains the deliverables for the Week 5 AI assignment focused on applying AI concepts across the lifecycle of problem-solving, from definition to deployment, using a healthcare-based case study.

---

## 📁 Contents

- `Critical Thinking.pdf`: PDF with detailed responses for the assignment's Part 3.
- All code (if any) related to model design or preprocessing.
- This `README.md` file summarizing the full scope of work.

---

## 🧠 Part 1: Short Answer Questions (30 points)

### 1. Problem Definition

**Problem:** Predicting student dropout rates.  
**Objectives:**
- Identify students at risk of dropping out.
- Improve student retention.
- Provide early intervention strategies.

**Stakeholders:**  
- School Administrators  
- Academic Advisors  

**KPI:**  
- Dropout prediction accuracy.

---

### 2. Data Collection & Preprocessing

**Data Sources:**
- Student Information Systems (SIS)
- Learning Management Systems (LMS)

**Potential Bias:**  
- Overrepresentation of students from urban schools may skew results.

**Preprocessing Steps:**
1. Handle missing attendance/grades.
2. Normalize numerical features.
3. Encode categorical variables (e.g., gender, school type).

---

### 3. Model Development

**Model Chosen:** Random Forest  
**Justification:** Robust to overfitting and handles both categorical and numerical data.

**Data Split:**  
- Training: 70%  
- Validation: 15%  
- Test: 15%  

**Hyperparameters Tuned:**
- `max_depth`: Controls model complexity.
- `n_estimators`: Number of trees for ensemble strength.

---

### 4. Evaluation & Deployment

**Evaluation Metrics:**
- Accuracy: Measures overall correctness.
- F1-Score: Balances precision and recall for imbalanced datasets.

**Concept Drift:**  
Occurs when data patterns change over time.  
**Monitoring:** Use dashboards and periodic retraining.

**Deployment Challenge:**  
Ensuring scalability for large student datasets.

---

## 🏥 Part 2: Case Study – Hospital Readmission Prediction (40 points)

### Problem Scope

**Problem:** Predict patient readmission within 30 days post-discharge.  
**Objectives:**
- Reduce readmissions
- Improve care quality

**Stakeholders:**  
- Hospital Management  
- Clinicians

---

### Data Strategy

**Data Sources:**
- Electronic Health Records (EHRs)  
- Patient Demographics

**Ethical Concerns:**
- Data privacy (HIPAA compliance)  
- Algorithmic bias against underserved groups

**Preprocessing Pipeline:**
- Handle missing vitals/labs  
- Feature engineering (e.g., comorbidity count)  
- One-hot encoding for categorical values

---

### Model Development

**Model Chosen:** Logistic Regression  
**Reason:** Interpretable for clinical use

**Confusion Matrix Example:**
