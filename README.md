# 🏥 Medical Appointment No-Show Prediction

This project aims to predict whether a patient will show up for a medical appointment using classification machine learning models. It uses the "Medical Appointment No Show" dataset and performs end-to-end analysis including data cleaning, EDA, feature engineering, model building, and evaluation.

---

## 📂 Dataset

- **Source**: Kaggle – [Medical Appointment No Shows](https://www.kaggle.com/joniarroba/noshowappointments)
- **Description**: The dataset contains 110k+ medical appointments in Brazil and whether the patient showed up or not.
- **Target Variable**: `No-show` (Yes/No)

---

## 🧹 Data Preprocessing

- Removed unnecessary columns: `PatientId`, `AppointmentID`
- Converted `ScheduledDay` and `AppointmentDay` to datetime
- Encoded categorical features using **Label Encoding**
- Handled class imbalance using **SMOTE**
- Final features only in numeric format (SMOTE requirement)

---

## 📊 Exploratory Data Analysis (EDA)

- Checked for nulls and duplicates
- Visualized:
  - No-show distribution
  - Age and waiting time
  - Day of the week of appointment
  - Neighbourhood trends (if applicable)

---

## 🤖 Models Used

| Model               | F1 Score (Class 1) | Accuracy |
|--------------------|--------------------|----------|
| Decision Tree       | ~0.40              | ~0.68    |
| Random Forest       | ~0.42              | ~0.69    |
| Gradient Boosting   | ~0.42              | ~0.62    |

> Note: SMOTE was used to handle the imbalanced target variable.

---

## 🔧 Model Tuning

- Used **RandomizedSearchCV** for hyperparameter tuning
- Focused on maximizing **F1-score for Class 1** (No-show = Yes)

---

## 🧪 Evaluation Metrics

- **Accuracy**
- **Precision, Recall, F1-score**
- **Classification Report**
- **Confusion Matrix**

---

## 📁 Project Structure
