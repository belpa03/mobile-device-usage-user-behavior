# 📱 Mobile Device Usage & User Behavior — ANN Deep Learning Project
---

## 🔍 Dataset Overview
**Source:** [Kaggle - Mobile Device Usage & User Behavior Dataset](https://www.kaggle.com/code/momenayman9/mobile-device-usage-and-user-behavio/input)

| Variable | Description |
|----------|-------------|
| User ID | Unique identifier for each user |
| Device Model | Smartphone model used |
| Operating System | Device OS (iOS or Android) |
| App Usage Time (min/day) | Average daily app usage in minutes |
| Screen On Time (hours/day) | Average daily screen-on duration |
| Battery Drain (mAh/day) | Daily battery consumption |
| Number of Apps Installed | Total installed apps |
| Data Usage (MB/day) | Daily data usage in MB |
| Age | User age |
| Gender | Male / Female |
| User Behavior Class | Behavior classification (1–5, light to extreme) |

---

## 🔁 Project Workflow

### 1. Data Ingestion & Initial Check
- Load dataset and inspect schema.
- Check for missing values and inconsistent types.
- No missing values found → ready for preprocessing.

### 2. Exploratory Data Analysis (EDA)
- Analyze distributions of User Behavior Class, Age, Gender, OS.
- Visualize correlations between App Usage Time, Screen On Time, Battery Drain, Data Usage.
- Insights: heavy usage correlates with high battery consumption; Class 2 dominates.

### 3. Data Cleaning & Preprocessing
- Encode categorical variables.
- Standardize numeric variables for ANN modeling.
- Dataset split into 80% training / 20% testing.

### 4. Feature Engineering
- Create derived metrics (e.g., usage per app, battery per hour).
- Correlation analysis to select features for ANN.

### 5. ANN Model Training
- Train ANN with training set, validation split 0.33, 100 epochs.
- Monitor accuracy and loss to ensure proper convergence.

### 6. Model Evaluation
- Evaluate test accuracy and analyze confusion matrix.
- Class 1 shows highest correct-classification rate (73.8%).

### 7. Predictions
- Generate predicted classes for test set.
- Evaluate probability distributions across classes.

### 8. Model Visualization
- Infographic charts for training accuracy, loss, and confusion matrix.
- Heatmaps and scatterplots for feature correlations.

### 9. Reporting & Business Insights
- Infographic + one-page summary for stakeholders.
- Provides actionable insights for app retention, device optimization, and personalization strategies.

---

## 💡 Conclusions

- Device usage intensity directly impacts battery consumption and app interaction.  
- Behavior Class 2 dominates the population, while Class 1 is least represented.  
- ANN achieved **76.62% accuracy**, showing good predictive performance.  
- Confusion matrix shows Class 1 was most accurately predicted (73.8%).  
- Misclassifications mainly occur between adjacent classes (2 and 3), suggesting overlapping behavioral traits.  
- ANN effectively models nonlinear relationships, supporting segmentation and targeted interventions for different user behavior classes.  

---

## 🖼️ Infographic Notes (`User Behavior.png`)
![User Behavior](User%20Behavior.png)  
- Designed for stakeholders to quickly grasp key insights.
- Clean layout, 2–3 corporate colors, clear metrics.
- Panels include: class distribution, usage vs battery, device/OS insights, ANN accuracy, confusion matrix, business recommendations.  

