# Multi-Label Text Classification Using Clinical BERT with Zero-Shot and Manual Labeling

This repository contains the implementation of a **multi-label text classification pipeline** using Clinical BERT. The project involves manually labeled benchmark data, which was split into training and testing datasets. The goal is to classify text into multiple predefined categories and evaluate the performance of the trained model.

---

## 📝 **Project Overview**

### **Objective**
- Build a robust multi-label classification model for text data using Clinical BERT.
- Use **manually labeled benchmark data** for training and testing.
- Evaluate the model's performance on key metrics.

### **Dataset**
1. **Benchmark Data**:  
   - Manually labeled dataset based on domain expertise.  
   - Split into training and testing datasets.  
   - Labels include:
     - Healthcare Provider
     - Patient
     - Payers and Insurers
     - Pharmaceutical Representative
     - Regulator

### **Key Features**
- **Clinical BERT-based multi-label classification.**
- Multi-metric evaluation: F1 Score (Micro), Hamming Loss, Classification Report.
- Experiment tracking and artifact logging using **DagsHub** and **MLflow**.

---

## ⚙️ **Workflow**

1. **Data Preprocessing**  
   - Convert stringified labels into Python lists.  
   - Encode multi-labels into a multi-hot format.  
   - Split the dataset into training and testing sets.

2. **Model Training**  
   - Fine-tune the Clinical BERT model on the training dataset.  
   - Handle class imbalance using weighted loss functions.

3. **Evaluation**  
   - Evaluate the model using metrics like F1 score, Hamming Loss, and Classification Report.  
   - Visualize confusion matrices for each class.

4. **Experiment Tracking**  
   - Log metrics, parameters, and artifacts using **MLflow** integrated with **DagsHub**.

---

## 📊 **Metrics and Evaluation**

The model performance is evaluated using:  
- **F1 Score (Micro)**: To measure overall precision and recall.  
- **Hamming Loss**: To assess misclassification of labels.  
- **Classification Report**: Precision, recall, and F1-score for each label.  
- **Confusion Matrices**: Visualized for each class.

---
