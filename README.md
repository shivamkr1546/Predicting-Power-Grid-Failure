# 🔌 Power Failure Severity Prediction using Random Forest

This project uses a machine learning model to predict power failure severity based on various system features. The goal is to assist in the early identification of critical system failures to improve reliability and maintenance in power grid infrastructures.

---

## 📁 Project Structure

- `dt.ipynb` – Main Jupyter Notebook containing the data preprocessing, model training, evaluation, and visualization.
- `confusion_matrix.png` – Confusion matrix heatmap showing the model's performance.

---

## 📊 Dataset Overview

The dataset contains historical power failure records with features such as:
- Resource type
- Severity type
- Location attributes
- Event type

The target variable is **`failure_severity`**, indicating whether a system experienced:
- No failure (`0`)
- Some failure (`1`)

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy (Data manipulation)
- Scikit-learn (Machine Learning)
- Matplotlib, Seaborn (Visualization)

---

## 🧠 Model Used

- **Random Forest Classifier**  
Chosen for its robustness, ability to handle imbalanced classes, and superior performance in classification tasks.

---

## ✅ Results

### Confusion Matrix Summary

|                    | Predicted: No Failure | Predicted: Failure |
|--------------------|-----------------------|--------------------|
| **Actual: No Failure** | 233                   | 0                  |
| **Actual: Failure**    | 2                     | 65                 |

- **Accuracy**: ~99.3%
- **Precision**: High (no false positives)
- **Recall**: High (only 2 false negatives)
- **Conclusion**: The model is highly reliable for detecting power failure severity with minimal misclassifications.

---

## 📌 Key Highlights

- Achieved near-perfect accuracy on the test dataset
- Extremely low false negative and zero false positive rate
- Provides a reliable method for predicting failures in power systems
- Could be integrated into real-time power grid monitoring systems

---

## 🚀 Future Work

- Integrate live data streams for real-time predictions
- Add more class labels for different failure types
- Deploy model as a web application for real-time monitoring

---

## 🙌 Acknowledgements

- Built using public power system datasets
- Inspired by real-world grid maintenance challenges

---

## 🧾 License

This project is for academic and educational use.
