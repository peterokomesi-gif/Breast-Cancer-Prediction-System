# Breast-Cancer-Prediction-System
Breast Cancer Prediction System is a machine learning and Streamlit-based application that classifies tumors as Benign or Malignant using the Wisconsin Breast Cancer Dataset. The project includes data preprocessing, model training, evaluation, and deployment, providing fast and accurate predictions through an interactive web interface.
# Breast Cancer Prediction System

A Machine Learning and Streamlit-based web application that predicts whether a breast tumor is **Benign** or **Malignant** using the Wisconsin Breast Cancer Diagnostic Dataset. The project demonstrates the complete machine learning workflow, including data preprocessing, model training, evaluation, model deployment, and user interaction through a simple web interface.

---

##  Project Overview

Breast cancer is one of the most common cancers worldwide. Early detection can significantly improve treatment outcomes and survival rates.

This project uses machine learning algorithms to classify tumors as:

* **Benign (Non-Cancerous)**
* **Malignant (Cancerous)**

The final model is deployed using **Streamlit**, allowing users to enter tumor measurements and receive instant predictions.

---

##  Objectives

* Load and explore the Breast Cancer Wisconsin Dataset.
* Perform data preprocessing and feature scaling.
* Train multiple machine learning classification models.
* Evaluate model performance using various metrics.
* Select and save the best-performing model.
* Build an interactive Streamlit web application.
* Predict breast cancer diagnosis from user-provided inputs.

---

##  Dataset Information

**Dataset:** Breast Cancer Wisconsin (Diagnostic)

**Source:** Scikit-learn Built-in Dataset

### Dataset Statistics

* Total Samples: 569
* Features: 30 Numerical Features
* Classes:

  * 0 → Malignant
  * 1 → Benign

### Example Features

* Mean Radius
* Mean Texture
* Mean Smoothness
* Mean Concavity
* Mean Symmetry
* Fractal Dimension
* Perimeter
* Area
* Compactness

---

##  Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Streamlit
* Joblib

---

##  Project Structure

```text
Breast_Cancer_Prediction/
│
├── notebook/
│   └── breast_cancer_prediction.ipynb
│
├── models/
│   ├── breast_cancer_model.pkl
│   └── scaler.pkl
│
├── app.py
├── requirements.txt
├── README.md
└── report.pdf
```

---

##  Exploratory Data Analysis

The project includes:

* Dataset shape analysis
* Feature distribution analysis
* Class distribution visualization
* Correlation heatmap
* Summary statistics
* Missing value detection
* Duplicate record checking

---

##  Data Preprocessing

The following preprocessing steps were performed:

### 1. Missing Value Handling

* Checked dataset for null values.
* Replaced missing values when necessary.

### 2. Duplicate Removal

* Identified and removed duplicate records.

### 3. Feature Scaling

* StandardScaler used to normalize features.

### 4. Train-Test Split

* 80% Training Data
* 20% Testing Data

---

##  Machine Learning Models

Three classification models were trained and compared:

### Logistic Regression

A simple and interpretable linear classification model.

### Random Forest Classifier

An ensemble learning method using multiple decision trees.

### Support Vector Machine (SVM)

A powerful classifier capable of handling complex decision boundaries.

---

##  Model Evaluation Metrics

Each model was evaluated using:

* Accuracy Score
* Precision Score
* Recall Score
* F1 Score
* Confusion Matrix

Example:

```python
from sklearn.metrics import accuracy_score
```

---

## Best Model Selection

The model with the highest overall performance was selected based on:

* Accuracy
* Precision
* Recall
* F1 Score

The final model was saved using Joblib for deployment.

```python
import joblib

joblib.dump(model, "breast_cancer_model.pkl")
```

---

##  Streamlit Application

The web application allows users to:

* Enter tumor feature values.
* Click the Predict button.
* Receive instant prediction results.

### Prediction Outputs

 Benign — Low Risk

 Malignant — High Risk

### Additional Features

* Dataset Information Sidebar
* Model Accuracy Display
* User Guide Section
* Clean and Interactive Interface

---

##  Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/Breast-Cancer-Prediction-System.git
```

### Navigate to Project Directory

```bash
cd Breast-Cancer-Prediction-System
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

##  Run Application

```bash
streamlit run app.py
```

Open your browser and visit:

```text
http://localhost:8501
```

---

##  Application Screenshots

### Home Page

Add screenshot here.

### Prediction Page

Add screenshot here.

---

##  Results

The trained model achieved high classification accuracy on unseen test data, demonstrating the effectiveness of machine learning in healthcare diagnosis support systems.

Key outcomes include:

* Accurate tumor classification
* Fast prediction response
* User-friendly deployment interface
* End-to-end machine learning workflow implementation

---

##  Learning Outcomes

Through this project, the following concepts were learned:

* Data preprocessing techniques
* Exploratory Data Analysis (EDA)
* Feature scaling
* Classification algorithms
* Model evaluation
* Model deployment with Streamlit
* Healthcare AI applications

---

##  Future Improvements

* Hyperparameter tuning using GridSearchCV
* SHAP explainability integration
* Cloud deployment
* Database integration
* User authentication
* Prediction history tracking

---

##  Author

Developed as part of a Machine Learning Internship Project focusing on healthcare prediction systems and deployment of machine learning models using Streamlit.

---

##  License

This project is intended for educational and learning purposes.
