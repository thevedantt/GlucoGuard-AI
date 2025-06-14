# 🛡️ GlucoGuard AI

**Your AI-Powered Diabetes Risk Predictor & Health Advisor**

GlucoGuard AI is a smart health assistant that predicts diabetes risk using machine learning and provides personalized lifestyle recommendations via Google Gemini AI. It's your early warning system for better health and long-term prevention.
---

## 📌 Features

- Predicts diabetes risk based on user input.
- Trained on **Pima Indians Diabetes Dataset**.
- Uses **Random Forest Classifier** for high accuracy.
- Dynamically generates personalized recommendations via **Gemini AI API**.
- CLI-based interactive input system for real-time health assessments.
- Gender-sensitive handling (e.g., pregnancies input for females).

---

## 🛠️ Technologies Used

- Python 3.x
- pandas, numpy
- scikit-learn
- `requests` (for Gemini API calls)
- Google Gemini AI (`generativelanguage.googleapis.com`)

---
##🧠 How It Works
Model Training:

Loads data and splits it into training/test sets.

Trains a RandomForestClassifier.

User Input:

Asks user for health metrics like glucose, BMI, blood pressure, etc.

Gender-sensitive handling of Pregnancies field.

Prediction & Output:

Predicts the probability of having diabetes.

Shows Risk Level, Confidence, and Probability.

AI Recommendations:

Sends user profile to Gemini API.

Receives and displays a detailed lifestyle recommendation.
## 📂 Dataset

The system uses a dataset with the following columns:

```text
['Pregnancies', 'Glucose', 'BloodPressure', 'SkinThickness', 'Insulin',
 'BMI', 'DiabetesPedigreeFunction', 'Age', 'Outcome']

🚀 How to Run
Install required libraries:

bash
Copy
Edit
pip install pandas numpy scikit-learn requests
Upload your dataset (diabetes.csv) to the environment.

Update the path in the code if needed:

python
Copy
Edit
DiabetesPredictionSystem(csv_path="/content/diabetes.csv").run()
Run the Python script.

python
Copy
Edit
self.gemini_api_key = "YOUR_API_KEY_HERE"
Get the key from: https://makersuite.google.com/



