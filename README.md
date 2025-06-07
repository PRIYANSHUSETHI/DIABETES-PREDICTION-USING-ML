
# 🩺 Diabetes Prediction using Machine Learning

This project applies various machine learning models to predict whether a person is diabetic or not using medical diagnostic features. Built on the Pima Indians Diabetes Dataset, it compares multiple classifiers and identifies the best-performing model to deploy a predictive system.

## 📊 Dataset

- **Source**: [`diabetes.csv`](https://www.kaggle.com/datasets/mathchi/diabetes-data-set)
- **Features**: 8 medical indicators such as:
  - Pregnancies
  - Glucose
  - BloodPressure
  - SkinThickness
  - Insulin
  - BMI
  - DiabetesPedigreeFunction
  - Age
- **Target**: `Outcome` (0 = Non-Diabetic, 1 = Diabetic)

## 🚀 Features of This Project

- 🧼 Data preprocessing and standardization using `StandardScaler`
- 📈 Exploratory Data Analysis (EDA) using Seaborn and Matplotlib
- 🤖 Trained and evaluated 4 classifiers:
  - Support Vector Machine (SVM)
  - Logistic Regression
  - Random Forest
  - K-Nearest Neighbors (KNN)
- 🧪 Hyperparameter tuning for SVM using `GridSearchCV`
- 🔄 Cross-validation for robustness
- 📉 Evaluation using:
  - Accuracy
  - Confusion Matrix
  - Classification Report
  - ROC Curve & AUC Score
- 🧠 Final Prediction System using best model (Random Forest)
- ✅ Confidence score output with each prediction

## 🛠️ Installation

Clone the repo and install dependencies:
```bash
git clone https://github.com/yourusername/diabetes-prediction-ml.git
cd diabetes-prediction-ml
pip install -r requirements.txt
```

## 📦 Requirements

```txt
numpy
pandas
matplotlib
seaborn
scikit-learn
```

## 🧪 How to Use

Update the `input_data` tuple in the script with new patient values:
```python
input_data = (4, 110, 92, 0, 0, 37.6, 0.191, 30)
```

Run the script:
```bash
python diabetes_prediction_using_ML.py
```

You’ll get a result like:
```
The person is DIABETIC (Confidence: 0.87)
```

## 📊 Sample Output

- Model Accuracy Comparison Bar Chart
- Confusion Matrix
- ROC Curve with AUC
- Text-based prediction with confidence score

## 📌 Conclusion

Random Forest outperformed other classifiers in accuracy and robustness, making it the preferred model for deployment. This predictive system can help in early detection of diabetes using accessible health parameters.
