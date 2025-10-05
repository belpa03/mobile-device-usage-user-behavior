# 📱 Mobile Device Usage & User Behavior — Deep Learning Analysis

A data science project exploring user behavior patterns from mobile usage data using **Artificial Neural Networks (ANN)**.  
This project combines **data cleaning, EDA, feature engineering, ANN modeling**, and **business-driven insights visualization** in one repository.

---

## 🔍 Dataset Overview
**Source:** [Kaggle - Mobile Device Usage & User Behavior Dataset](#)

| Variable | Description |
|-----------|--------------|
| User ID | Unique identifier for each user |
| Device Model | Smartphone model used |
| Operating System | iOS or Android |
| App Usage Time (min/day) | Daily app usage time |
| Screen On Time (hours/day) | Average screen active time |
| Battery Drain (mAh/day) | Daily battery consumption |
| Number of Apps Installed | Total apps per user |
| Data Usage (MB/day) | Daily mobile data usage |
| Age | User’s age |
| Gender | Male / Female |
| User Behavior Class | 1–5, from light to extreme usage |

---

## 🎯 Project Objectives
1. Clean and preprocess the dataset for modeling.  
2. Understand patterns and correlations in mobile usage.  
3. Build and train a **Deep Learning model (ANN)** to classify `User Behavior Class`.  
4. Evaluate model performance and interpret patterns.  
5. Visualize findings through an **infographic** for non-technical audiences.

---

## 🧠 Methodology
| Step | Description |
|------|--------------|
| **1. Data Cleaning & Filtering** | Handling missing values, type correction, and outlier removal. |
| **2. Exploratory Data Analysis (EDA)** | Understanding variable distribution, correlations, and relationships. |
| **3. Feature Engineering** | Creating new metrics such as `usage_per_app` and `battery_per_hour`. |
| **4. Deep Learning (ANN)** | Building and training a multi-layer perceptron (MLP) for classification. |
| **5. Evaluation & Visualization** | Comparing accuracy, loss trends, and generating visual reports. |
| **6. Business Insight Interpretation** | Translating technical findings into actionable takeaways. |

---

## 🧩 Model Architecture (ANN)
- **Input Layer:** normalized numeric features  
- **Hidden Layers:** 2–3 Dense layers (ReLU activation)  
- **Dropout:** to prevent overfitting  
- **Output Layer:** softmax activation (5 classes)  
- **Optimizer:** Adam  
- **Loss:** categorical crossentropy  
- **Metrics:** accuracy, F1-score  

Example summary (Keras):
```python
model = Sequential([
    Dense(64, activation='relu', input_dim=X_train.shape[1]),
    Dropout(0.3),
    Dense(32, activation='relu'),
    Dense(5, activation='softmax')
])
