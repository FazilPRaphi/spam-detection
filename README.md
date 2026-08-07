#  Email Spam Detection using Machine Learning

A machine learning project that classifies emails as **Spam** or **Not Spam** using multiple supervised learning algorithms. The project compares various classification models, evaluates their performance, and selects the best-performing model based on accuracy and other evaluation metrics.

---

##  Project Overview

Email spam is one of the most common cybersecurity and communication problems. Spam emails often contain phishing attempts, advertisements, malware, or fraudulent content.

This project uses the **UCI Spambase Dataset** to build and evaluate multiple machine learning models capable of accurately identifying spam emails based on statistical features extracted from the email text.

---

##  Objectives

- Perform data exploration and preprocessing.
- Analyze the dataset for missing values and duplicates.
- Train multiple machine learning classification models.
- Compare model performance.
- Evaluate models using various performance metrics.
- Save the best-performing model for future predictions.

---

#  Technologies Used

| Category | Technology |
|----------|------------|
| Language | Python |
| Environment | Google Colab |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Model Saving | Joblib |

---

#  Dataset

Dataset Used:

**UCI Spambase Dataset**

- Total Samples: **4601**
- Features: **57**
- Target Variable: **1**

Target Labels:

| Value | Meaning |
|--------|----------|
| 0 | Not Spam |
| 1 | Spam |

Each feature represents the frequency of certain words or characters appearing within an email.

---

#  Exploratory Data Analysis

The following analysis was performed:

- Dataset inspection
- Shape analysis
- Data types
- Statistical summary
- Missing value detection
- Duplicate record detection
- Class distribution
- Correlation analysis
- Feature distribution visualization

---

#  Data Preprocessing

The preprocessing pipeline included:

- Checking missing values
- Removing duplicate records
- Separating features and target variable
- Train-Test Split
- Feature Scaling using StandardScaler

Train-Test Ratio:

```
80% Training
20% Testing
```

Random State:

```
42
```

---

#  Machine Learning Models

The following supervised learning algorithms were implemented:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

---

#  Model Evaluation

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

Performance comparison was carried out to determine the best-performing classifier.

---

#  Visualizations

The project includes several visualizations such as:

- Spam vs Non-Spam Distribution
- Pie Chart of Target Classes
- Correlation Heatmap
- Feature Distribution Graphs
- Model Accuracy Comparison
- Confusion Matrix

---

#  Best Model

The Random Forest Classifier achieved the highest overall performance on the Spambase dataset.

 accuracy:

```
94%
```

---

#  Model Persistence

The trained model and scaler are saved using Joblib.

Generated files:

```
spam_detector.pkl

scaler.pkl
```

These can later be loaded without retraining the model.

Example:

```python
import joblib

model = joblib.load("spam_detector.pkl")
scaler = joblib.load("scaler.pkl")
```

---

#  Project Structure

```
spam-detection/
│
├── Spam_Detection_ML.ipynb
├── spambase_csv.csv
├── spam_detector.pkl
├── scaler.pkl
├── README.md
└── requirements.txt
```

---

#  Installation

Clone the repository

```bash
git clone https://github.com/yourusername/spam-detection.git
```

Navigate to the project

```bash
cd spam-detection
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶ Running the Project

Open the notebook

```
Spam_Detection_ML.ipynb
```

Run all cells sequentially.

The notebook performs:

- Data Loading
- Data Cleaning
- Data Visualization
- Model Training
- Model Evaluation
- Model Comparison
- Model Saving

---

#  Requirements

```
numpy
pandas
matplotlib
seaborn
scikit-learn
joblib
```

Or install them using

```bash
pip install numpy pandas matplotlib seaborn scikit-learn joblib
```

---

#  Concepts Covered

- Data Cleaning
- Exploratory Data Analysis
- Feature Scaling
- Supervised Learning
- Classification
- Model Evaluation
- Confusion Matrix
- Precision
- Recall
- F1 Score
- Model Persistence

---

#  Future Improvements

Possible future enhancements include:

- Hyperparameter tuning using GridSearchCV
- Cross Validation
- ROC Curve Analysis
- Precision-Recall Curve
- Feature Importance Analysis
- SHAP Explainability
- Streamlit Web Application
- Flask REST API
- Email Classification Dashboard
- Real-time Spam Detection

---

#  Sample Output

The notebook generates:

- Dataset statistics
- Visualizations
- Model comparison table
- Confusion matrices
- Classification reports
- Saved machine learning model

---

#  Author

**Fazil P Raphi**

B.Tech Computer Science Engineering

Machine Learning • Cloud Computing • Full Stack Development

---

#  Acknowledgements

- UCI Machine Learning Repository
- Scikit-learn Documentation
- Google Colab
- Pandas Documentation
- Matplotlib
- Seaborn

---

#  License

This project is released under the MIT License.

```

