# ⚡ Predicting Power Grid Failure Using Historical Outage Data

This project applies machine learning techniques to predict power grid failures using historical outage data. Early prediction of potential failures allows grid operators to take proactive steps in maintenance and risk mitigation, ultimately enhancing system reliability and reducing downtime.

---

## 📌 Project Objective

To build and evaluate a machine learning model capable of accurately classifying power outage events into "Failure" or "No Failure" using features derived from historical grid outage data.

---

## 📁 Project Structure

- `dt.ipynb` – Main Jupyter notebook containing:
  - Data preprocessing
  - Model training (Random Forest)
  - Evaluation metrics
  - Confusion matrix visualization

- `confusion_matrix.png` – Visual output of model prediction performance

---

## 📊 Dataset Description

The dataset contains entries of power outages along with features that may influence failure events, including:
- Resource type
- Event type
- Severity indicators
- Location-based attributes

### Target Variable
- `failure_severity`:
  - `0` → No Failure
  - `1` → Failure

---

## 🧠 Model Summary

### Algorithm Used:
- **Random Forest Classifier**

### Why Random Forest?
- Handles categorical and numerical data well
- Robust to overfitting
- Suitable for binary and multi-class classification
- Provides high accuracy and interpretability

---

## ✅ Evaluation Results

### Confusion Matrix

|                    | Predicted: No Failure | Predicted: Failure |
|--------------------|-----------------------|--------------------|
| **Actual: No Failure** | 233                   | 0                  |
| **Actual: Failure**    | 2                     | 65                 |

### Performance Metrics:
- **Accuracy**: ~99.3%
- **Precision**: 100%
- **Recall**: ~97%
- **F1-Score**: High (balanced precision and recall)

### 🔍 Interpretation:
- The model made **only 2 misclassifications** out of 300.
- No false positives were recorded, ensuring reliable failure predictions.
- Slight under-detection of failure cases, which can be improved with future tuning.

---

## 📈 Key Learnings

- Historical outage data provides valuable insight into grid behavior.
- Machine learning, especially ensemble models like Random Forest, is highly effective for predicting grid failures.
- Confusion matrix and performance metrics help validate the model’s reliability for real-world deployment.

---

## 🚀 Future Improvements

- Add real-time data pipeline for live failure prediction
- Explore other models (XGBoost, SVM) and compare performance
- Include feature importance analysis for explainability
- Deploy as a REST API or integrate into a grid monitoring dashboard

---

## 👨‍💻 Tools and Libraries

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib

---

## 🧾 License

This project is intended for educational and research purposes.

---

## ✍️ Author

- [Your Name Here]
