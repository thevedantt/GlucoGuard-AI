# 🛡️ GlucoGuard AI
**Your AI-Powered Diabetes Risk Predictor & Health Advisor**

GlucoGuard AI is a smart health assistant that predicts diabetes risk using machine learning and provides personalized lifestyle recommendations via Google Gemini AI. It's your early warning system for better health and long-term prevention.

---

## 📌 Features

- 🔍 Predicts diabetes risk based on user input
- 📊 Trained on Pima Indians Diabetes Dataset
- 🌲 Uses Random Forest Classifier for high accuracy
- 🤖 Dynamically generates personalized recommendations via Gemini AI API
- 🖥️ CLI-based interactive input system for real-time health assessments
- 👩 Gender-sensitive handling (e.g., pregnancies input for females)

---

## 🛠️ Technologies Used

- Python 3.x
- pandas, numpy
- scikit-learn
- requests (for Gemini API calls)
- Google Gemini AI (generativelanguage.googleapis.com)

---

## 🧠 How It Works

### 🧪 Model Training:
- Loads data and splits it into training/test sets
- Trains a `RandomForestClassifier`

### 🧍 User Input:
- Asks user for health metrics like glucose, BMI, blood pressure, etc.
- Gender-sensitive handling of Pregnancies field

### 🧾 Prediction & Output:
- Predicts the probability of having diabetes
- Shows Risk Level, Confidence, and Probability

### 🤖 AI Recommendations:
- Sends user profile to Gemini API
- Receives and displays a detailed lifestyle recommendation

---

## 📂 Dataset

The system uses a dataset with the following columns:

```
['Pregnancies', 'Glucose', 'BloodPressure', 'SkinThickness', 'Insulin',
 'BMI', 'DiabetesPedigreeFunction', 'Age', 'Outcome']
```

---

## 🚀 How to Run

### 1. Install Required Libraries

```bash
pip install pandas numpy scikit-learn requests
```

### 2. Upload Dataset

Make sure your `diabetes.csv` file is placed in your environment, e.g.:

```python
diabetes = pd.read_csv('/content/diabetes.csv')
```

### 3. Update API Key

Open the main script and replace:

```python
self.gemini_api_key = "YOUR_API_KEY_HERE"
```

🔑 Get your free API key at: [https://makersuite.google.com/](https://makersuite.google.com/)

### 4. Run the Application

```python
DiabetesPredictionSystem(csv_path="/content/diabetes.csv").run()
```

---

## 💬 Example Output

```text
Diabetes Risk: HIGH RISK
Confidence: 92.3%
Diabetes Probability: 0.879

🤖 AI LIFESTYLE RECOMMENDATIONS
1. IMMEDIATE ACTIONS: Cut sugary intake, walk 30 min daily...
2. DIET: Add oats, broccoli, avoid white rice...
3. EXERCISE PLAN: 4x/week, 45 mins, moderate intensity...
...
```

---

## 📢 Disclaimer

This tool is **not a medical diagnosis**. It is an educational aid.  
Always consult certified healthcare professionals for actual medical decisions.

---

## 🧑‍💻 Author

**Vedantt Talekar**  
Open to feedback & collaborations!

Let me know if you want a logo, deployment guide (Streamlit/Gradio), or want to host it online!
