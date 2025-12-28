Diabetes Prediction using Support Vector Machine (SVM)
This project implements a machine learning model to predict whether a patient has diabetes based on specific diagnostic measurements. The system utilizes a Support Vector Machine (SVM) classifier to achieve high accuracy in classification.

📌 Project Overview
The goal of this project is to build a predictive system that can assist medical professionals in identifying diabetic patients. The workflow includes data preprocessing, standardization, model training, and a predictive system for new data instances.

🛠️ Technical Stack
Language: Python

Libraries: \* Pandas & NumPy (Data Manipulation)

Scikit-learn (Machine Learning & Preprocessing)

StandardScaler (Feature Scaling)

📊 Dataset Description
The model is trained on a dataset containing 768 records with 8 medical features:

Pregnancies: Number of times pregnant

Glucose: Plasma glucose concentration

BloodPressure: Diastolic blood pressure (mm Hg)

SkinThickness: Triceps skin fold thickness (mm)

Insulin: 2-Hour serum insulin (mu U/ml)

BMI: Body mass index (weight in kg/(height in m)^2)

DiabetesPedigreeFunction: Genetic influence score

Age: Age in years

Outcome: 0 (Non-Diabetic) or 1 (Diabetic)

🚀 Workflow

1. Data Preprocessing
   Standardization was performed using StandardScaler to ensure all features are on a comparable scale, which is crucial for SVM performance.

Data was split into training (80%) and testing (20%) sets using stratified sampling to maintain class balance.

2. Model Training
   Algorithm: Support Vector Machine (SVM)

Kernel: Linear

Model Fitting: The classifier was trained on the standardized training data.

3. Evaluation Metrics
   The model demonstrates consistent performance across both training and testing datasets:

Training Data Accuracy: ~78.66%

Testing Data Accuracy: ~77.27%

🔍 Predictive System
The repository includes a script to predict the outcome for new, individual data points.

Python

# Example input for prediction

input_data = (4, 127, 88, 11, 155, 34.5, 0.598, 28)

# The system standardizes this input and predicts:

# [0] -> "The Person is not Diabetic."

📂 Repository Structure
Diabetes Prediction.ipynb: The complete Jupyter Notebook containing the code and analysis.

diabetes.csv: The dataset used for training and testing.

README.md: Documentation for the project.

💡 How to Use
Clone this repository.

Ensure you have the required libraries installed: pip install numpy pandas scikit-learn.

Run the Jupyter Notebook to see the step-by-step analysis and model training.
