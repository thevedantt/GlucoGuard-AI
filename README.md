# 🛡️ GlucoGuard AI

> **Your AI-Powered Diabetes Risk Predictor & Health Advisor**

**GlucoGuard AI** is an intelligent health assistant that predicts your risk of diabetes using machine learning and offers personalized lifestyle guidance via Google Gemini AI. It acts as your early warning system to promote better health and long-term prevention.

---

## 📌 Features

✅ Predicts diabetes risk based on user health metrics  
✅ Trained on **Pima Indians Diabetes Dataset**  
✅ Uses **Random Forest Classifier** for reliable accuracy  
✅ Real-time, **gender-aware interactive CLI input**  
✅ Integrates **Google Gemini AI** for custom lifestyle advice  
✅ Outputs: **Risk Level**, **Probability**, and **AI Recommendations**

---

## 🛠️ Technologies Used

- Python 3.x  
- `pandas`, `numpy`  
- `scikit-learn`  
- `requests` (for Gemini API communication)  
- **Google Gemini AI** (via `generativelanguage.googleapis.com`)

---

## 🧠 How It Works

### 🧪 Model Training
- Loads the dataset from CSV.
- Splits the data into training/testing sets.
- Trains a `RandomForestClassifier` model.

### 🧍 User Input
- Prompts user for medical input like glucose, blood pressure, BMI, etc.
- Smart gender-based handling (e.g., only females are asked about pregnancies).

### 🔮 Prediction & Output
- Predicts **risk of diabetes** based on model.
- Displays:
  - Risk Level (HIGH / LOW)
  - Confidence score
  - Diabetes probability

### 🤖 AI Lifestyle Recommendations
- Sends the patient profile to **Gemini API**
- Displays:
  - Immediate actions
  - Diet, exercise, and stress advice
  - Monitoring schedule & medical follow-up

---

## 📂 Dataset Columns

```text
['Pregnancies', 'Glucose', 'BloodPressure', 'SkinThickness', 'Insulin',
 'BMI', 'DiabetesPedigreeFunction', 'Age', 'Outcome']
