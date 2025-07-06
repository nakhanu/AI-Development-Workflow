# 🧠 Week 5 Assignment – AI Development Workflow

This repository contains all deliverables for the Week 5 AI assignment, which covers theoretical, practical, and reflective components of designing and deploying an AI system. It includes structured sections covering short answer questions, a healthcare case study, ethical analysis, and a visual workflow diagram.

---

## 📘 Part 1: Short Answer Questions (30 points)

### 1. Problem Definition (6 pts)

**Hypothetical AI Problem:** Predicting student dropout rates.

**Objectives:**
- Identify at-risk students early.
- Recommend targeted interventions.
- Improve overall student retention.

**Stakeholders:**
- School Administrators  
- Academic Advisors

**Key Performance Indicator (KPI):**
- Dropout prediction accuracy.

---

### 2. Data Collection & Preprocessing (8 pts)

**Data Sources:**
- Learning Management System (LMS) activity logs  
- Student Information System (SIS) records

**Potential Bias:**
- Overrepresentation of urban students may introduce bias against rural populations.

**Preprocessing Steps:**
1. Handle missing data (e.g., incomplete attendance).
2. Normalize test scores and grades.
3. Encode categorical variables like gender and school type.

---

### 3. Model Development (8 pts)

**Chosen Model:** Random Forest

**Justification:**  
Robust to overfitting and works well with mixed data types.

**Data Split:**
- Training: 70%
- Validation: 15%
- Testing: 15%

**Hyperparameters to Tune:**
- `n_estimators`: Controls number of trees in the forest.
- `max_depth`: Prevents overly complex models.

---

### 4. Evaluation & Deployment (8 pts)

**Evaluation Metrics:**
- Accuracy: Measures overall prediction correctness.
- F1-Score: Balances precision and recall, ideal for imbalanced datasets.

**Concept Drift:**  
Changes in data distribution over time that reduce model performance.

**Monitoring Strategy:**  
Regular re-evaluation using real-time data and performance dashboards.

**Technical Challenge:**  
Scaling the model for nationwide deployment across multiple school systems.

---

## 🏥 Part 2: Case Study – Hospital Readmission Prediction (40 points)

### Problem Scope (5 pts)

**Problem:** Predicting hospital readmission risk within 30 days of discharge.

**Objectives:**
- Minimize readmission rates.
- Optimize patient recovery plans.
- Reduce healthcare costs.

**Stakeholders:**
- Hospital Management
- Clinicians and Care Teams

---

### Data Strategy (10 pts)

**Proposed Data Sources:**
- Electronic Health Records (EHRs)  
- Patient demographics & discharge summaries

**Ethical Concerns:**
- Patient privacy and HIPAA compliance  
- Algorithmic bias (e.g., against underrepresented groups)

**Preprocessing Pipeline:**
1. Handle missing clinical values.
2. Feature engineering (e.g., comorbidity score, length of stay).
3. Encode categorical variables like diagnosis codes.

---

### Model Development (10 pts)

**Chosen Model:** Logistic Regression  
**Reasoning:** High interpretability for clinical use.

**Confusion Matrix (Hypothetical):**

|            | Predicted No | Predicted Yes |
|------------|--------------|---------------|
| Actual No  |      50      |      10       |
| Actual Yes |      5       |      35       |

**Precision:** 35 / (35 + 10) = 0.78  
**Recall:** 35 / (35 + 5) = 0.875

---

### Deployment Strategy (10 pts)

**Integration Steps:**
- Build a REST API for real-time integration with the EHR system.
- Trigger alerts in the clinician dashboard when risk is high.

**Compliance Measures:**
- Ensure data encryption in transit and at rest.
- Role-based access control and audit logs.

**Optimization Strategy:**  
Use dropout regularization and cross-validation to combat overfitting.

---

## 💡 Part 3: Critical Thinking (20 points)

### Ethics & Bias (10 pts)

**Effect of Bias:**  
Biased training data can lead to misdiagnosis, delayed care, or inappropriate treatment for minority groups.

**Mitigation Strategy:**  
Use diverse and representative datasets. Apply fairness-aware algorithms and monitor model fairness metrics.

---

### Trade-offs (10 pts)

**Interpretability vs. Accuracy:**  
In healthcare, highly interpretable models (e.g., logistic regression) are often preferred over complex models (e.g., neural networks) for trust and accountability, even at the cost of a slight dip in accuracy.

**Impact of Limited Resources:**  
Resource constraints may necessitate simpler, less computationally expensive models like Decision Trees or Logistic Regression over deep learning models.

---

## ✍️ Part 4: Reflection & Workflow Diagram (10 points)

### Reflection (5 pts)

**Challenge:**  
The hardest part was designing a fair and ethical preprocessing pipeline with limited healthcare data examples.

**Improvement:**  
With more time, I would explore federated learning to increase data diversity without compromising privacy.

---

### Workflow Diagram (5 pts)
[Problem Definition]
↓
[Data Collection]
↓
[Preprocessing & Feature Engineering]
↓
[Model Selection & Training]
↓
[Evaluation & Validation]
↓
[Deployment]
↓
[Monitoring & Optimization]

---

## 📦 Submission Checklist

- ✅ PDF Report (5–10 pages): Includes all sections except the diagram
- ✅ GitHub Repository: Includes this README and any relevant code or outputs
- ✅ PLP Academy Post: PDF article shared as required

---

## 🔗 References

- Scikit-learn Documentation: https://scikit-learn.org  
- World Health Organization – AI Ethics in Health  
- HIPAA Privacy Rule Overview: https://www.hhs.gov/hipaa/

---

