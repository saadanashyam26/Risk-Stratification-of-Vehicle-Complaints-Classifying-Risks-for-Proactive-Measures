# Risk Stratification of Vehicle Complaints 🚗💡

## 📌 Project Overview

The **Risk Stratification of Vehicle Complaints** project aims to enhance vehicle safety by leveraging **Machine Learning (ML) and Natural Language Processing (NLP)** to classify consumer complaints into risk categories. By analyzing **historical complaints, defect investigations, and recall datasets**, this project provides a data-driven approach to improve regulatory decision-making and predict future vehicle recalls.

This project was completed as part of **DSCI 5260** under the guidance of **Dr. Sameh Shamroukh** at the **G. Brint Ryan College of Business, UNT**.

---

## 🎯 Objectives

- **Develop an ML model** to classify vehicle complaints into **high, medium, and low risk**.
- **Analyze complaint trends** to identify early indicators of **safety defects**.
- **Assess the impact of new vehicle technologies** (ADAS, EVs, OTA updates) on recall patterns.
- **Improve regulatory decision-making** by automating complaint prioritization.
- **Enhance vehicle safety tracking** by integrating **structured recall and investigation data**.

---

## 🔍 Research Questions

1. **Predictive Analytics for Vehicle Recalls**  
   - What key factors in historical complaint data help identify **high-risk** complaints?  

2. **Impact of Technological Advancements**  
   - How have recalls evolved before and after major advancements (ADAS, EVs, self-driving)?  
   - Have software-related defects increased due to OTA updates and automation?  

---

## 📊 Data Sources & Preparation

### 📂 **Datasets Used**
We used **three primary datasets** from the **National Highway Traffic Safety Administration (NHTSA)**:

1. **Consumer Complaints Dataset** (1.2M+ records)  
   - Details **safety-related defect complaints** filed since 1995.  
   - Includes **crash, fire, injury, and fatality reports**.  

2. **Defect Investigations Dataset** (306K+ records)  
   - Contains NHTSA **safety defect investigations** since 1972.  
   - Links investigations to **specific vehicle makes/models**.  

3. **Recall Dataset** (583K+ records)  
   - Covers all **safety recalls** since 1967.  
   - Includes **manufacturer details, defect descriptions, and corrective actions**.  

📌 **Data Source:** [NHTSA Open Data](https://www.nhtsa.gov/nhtsa-datasets-and-apis)  

### 🔄 **Data Processing & Transformation**
- **Handling Missing Values**  
  - Removed columns with **90%+ missing data**.  
  - Imputed missing mileage and occurrences using **age-based means and medians**.  

- **Feature Engineering**  
  - Created **new attributes** like **vehicle age, time-to-report, regional classification, and complaint trends**.  
  - Used **NLP-based text analysis** for defect classification.  

- **Data Aggregation**  
  - Standardized records at the **complaint level** for better analysis.  
  - Merged complaints, investigations, and recall data for **predictive modeling**.  

---

## 🤖 Machine Learning Models

### 🏗 **Modeling Approach**
- **Complaint Risk Classification**  
  - ML models trained to categorize complaints as **High, Medium, or Low risk**.  
- **NLP-based Text Analysis**  
  - Used **BERT-based NLP models** to classify complaints based on recall likelihood.  
- **Predictive Recall Modeling**  
  - Implemented **XGBoost, Random Forest, and Logistic Regression** to predict **recall probabilities**.  

### 📊 **Model Architecture**
- **Feature Selection:** Extracted **key safety-related features**.
- **Supervised Learning:** Trained ML models using **labeled recall/investigation outcomes**.
- **Text Processing:** Applied **TF-IDF and BERT embeddings** for complaint descriptions.
- **Evaluation Metrics:** Used **Precision, Recall, F1-score, and ROC-AUC**.

---![image](https://github.com/user-attachments/assets/cd0c499a-4148-477a-9fc0-d925ae09b55e)


## 🛠️ Technology Stack

- **Programming Languages**: Python (Pandas, NumPy, Scikit-Learn, TensorFlow, NLP libraries)  
- **Cloud Services**: Google Cloud Storage for **dataset management**  
- **Data Visualization**: Matplotlib, Seaborn for **EDA and trends analysis**  
- **Machine Learning**: XGBoost, Random Forest, Logistic Regression, BERT NLP  
- **Big Data Processing**: PySpark for **handling large datasets efficiently**  

---

## 📈 Key Findings

- **ML models successfully classified** complaints with an **accuracy of ~85%**.
- **BERT-based NLP improved recall prediction** by capturing **textual complaint context**.
- **Software-related recalls increased by ~40%** post-ADAS and EV adoption.
- **Early complaint indicators** (fire, braking issues, unintended acceleration) were strong **predictors of recalls**.
- **Faster response times** for **high-risk** complaints could reduce **safety defects** significantly.

---


