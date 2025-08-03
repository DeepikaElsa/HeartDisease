# ❤️ Heart Disease Prediction System (with GUI)

This project is a **machine learning-based application** that predicts the likelihood of heart disease using patient health metrics. It includes both command-line and GUI interfaces, powered by various supervised ML models and deployed with a Tkinter-based user interface.

---

## 🔍 Project Highlights

- Trained on a real-world dataset (`heart.csv`)
- Multiple ML models: Logistic Regression, SVM, KNN, Decision Tree, Random Forest, Gradient Boosting
- Data preprocessing: handling duplicates, encoding categorical features, scaling
- GUI built using **Tkinter** for easy usability
- Model saved using **Joblib** for deployment

---

## 🧠 Models & Accuracy

| Model               | Accuracy (%) |
|--------------------|--------------|
| Logistic Regression| 78.69        |
| SVM                | 80.33        |
| K-Nearest Neighbors| 73.77        |
| Decision Tree      | 73.77        |
| Random Forest      | **81.97**    |
| Gradient Boosting  | 80.33        |

> Final model used for prediction in GUI: **Random Forest**

---

## 🗂️ Dataset Features

- `age`, `sex`, `cp`, `trestbps`, `chol`, `fbs`, `restecg`
- `thalach`, `exang`, `oldpeak`, `slope`, `ca`, `thal`
- `target`: 1 indicates the presence of heart disease, 0 indicates no disease

---

## 📦 Requirements

```bash
pip install pandas numpy scikit-learn matplotlib seaborn joblib
```
## To use the GUI
```bash
pip install tk
```
## ⚙️ How to Run
▶️ 1. Model Training and Evaluation
Run the full notebook or script that includes:
- Data preprocessing
- Model training & evaluation
- Saving the final model

💾 2. Save the Trained Model
```bash
import joblib
joblib.dump(rf, 'model_joblib_heart')
```
🖼️ 3. GUI Prediction App
Save and run the GUI Python file:
```bash
python gui_heart_predictor.py
```
You will be prompted to enter:
- Age
- Gender (1 for male, 0 for female)
- Chest Pain type (cp)
- Blood pressure, cholesterol, etc.

Press the Predict button to get the result:
- "No Heart Disease"
- "Possibility of Heart Disease"

## 📁 File Structure
├── heart.csv
├── model_training.ipynb / model_training.py
├── model_joblib_heart (Saved Model)
├── gui_heart_predictor.py
└── README.md
