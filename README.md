# 🫀 Heart Disease Prediction Using Machine Learning

This project applies supervised machine learning to predict the presence of heart disease using structured clinical data. The goal is to provide an early warning system for potential heart issues based on measurable health indicators.



## 📊 Dataset Features

The dataset includes the following attributes for each patient:

| Feature         | Description                                        |
|----------------|----------------------------------------------------|
| `age`           | Age of the patient                                 |
| `gender`        | Gender of the patient                              |
| `impluse`       | Heart rate or pulse                                |
| `pressurehight` | Systolic blood pressure                            |
| `pressurelow`   | Diastolic blood pressure                           |
| `glucose`       | Blood glucose level                                |
| `kcm`           | Potassium or related health marker                 |
| `troponin`      | Troponin level (indicator of heart muscle damage)  |
| `class`         | Target variable (1 = Heart Disease, 0 = No Disease)|

---

## 🧠 Models Used & Results

Three machine learning models were trained and tested:

| Model                    | Accuracy |
|--------------------------|----------|
| Logistic Regression      | **90%**  |
| Decision Tree Classifier | **97%**  |
| Random Forest Classifier | **98%**  |

🏆 **Best Model**: Random Forest Classifier (98% accuracy)

---

## 📈 Evaluation Metrics

Each model was evaluated with the following metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Curve

Visual tools such as confusion matrices and ROC curves were used to assess classification performance.

---

## ⚙️ Preprocessing Steps

- Cleaned the data (duplicates, missing values).
- Encoded categorical features like `gender`.
- Normalized features using `StandardScaler`.
- Split dataset into training and test sets (e.g., 80/20).

---

## 🚧 Challenges Faced

- **Data Scaling**: Essential for Logistic Regression and helped improve accuracy.
- **Overfitting Risk**: Managed using proper validation, especially for Decision Trees.
- **Model Interpretability**: Logistic Regression offered clearer insights, but tree-based models outperformed in accuracy.

---

## ✅ Achievements

- Developed an accurate ML pipeline to predict heart disease.
- Validated and compared multiple models with strong metrics.
- Identified significant features (like `troponin` and `pressurehight`) contributing to predictions.

---

## 🛠 Tools & Technologies

- **Language**: Python
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- **Environment**: Jupyter Notebook

---

## 🧪 How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/heart-disease-prediction.git
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch the notebook**:
   ```bash
   jupyter notebook heart_disease.ipynb
   ```

---

## 🚀 Future Enhancements

- Perform hyperparameter tuning (e.g., GridSearchCV).
- Deploy the model using Streamlit or Flask for user interaction.
- Add interpretability features like SHAP or LIME.
- Gather more diverse datasets to enhance model generalizability.
