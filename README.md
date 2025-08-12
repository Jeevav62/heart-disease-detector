# ❤️ Heart Disease Risk Predictor

A machine learning-powered web app that predicts the likelihood of heart disease based on user health metrics. Built with XGBoost and Streamlit, this tool offers interpretable predictions and confidence scores using the UCI Heart Disease dataset.

---

## 🚀 Features

- ✅ Predicts heart disease risk using XGBoost classifier
- 📊 Interactive Streamlit interface for real-time input
- 🎯 Confidence score for each prediction
- 🧠 Encodes categorical features with LabelEncoder
- 📁 Locally hosted model (`model.pkl`) for fast inference

---

## 🧪 Dataset

- Source: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease)
- Location: `data/heart_disease_uci.csv`
- Includes patient attributes like age, sex, chest pain type, cholesterol, ECG results, and more

---

## 🧠 Model Details

- Algorithm: `XGBClassifier`
- Parameters:
  - `n_estimators=300`
  - `max_depth=5`
  - `learning_rate=0.05`
  - `subsample=0.8`
  - `colsample_bytree=0.8`
  - `random_state=42`
- Target: Binary classification (`num > 0` → heart disease)

---

## 🖥️ How to Run Locally

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/heart-disease-detector.git
cd heart-disease-detector
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the App
```bash
streamlit run heart_disease.py
```

---

## 📦 Project Structure

```
heart-disease-detector/
├── data/
│   └── heart_disease_uci.csv
├── heart_disease_model.ipynb
├── heart_disease.py
├── model.pkl
├── requirements.txt
└── README.md
```

---

## 📊 Sample Prediction Output

- Input: Age = 57, Sex = Male, Chest Pain = Asymptomatic, Cholesterol = 270  
- Output: ⚠️ Likely to have heart disease  
  Confidence: 87.65%

---

## 🧑‍💻 Author

**Jeevarathinam V**  
Bachelor of Technology in AI & Data Science  
Anand Institute of Higher Technology, Chennai  
Focused on building socially impactful AI tools for misinformation detection, bias analysis, and media literacy.

---

# ❤️ Heart Disease Risk Predictor

## 🧾 Input Form

![User Input Form](assets/input_form.png)

## 📊 Prediction Result

![Prediction Output](assets/prediction_result.png)
