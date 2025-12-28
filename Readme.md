Rocks vs. Mines Prediction
This project implements a binary classification model to identify underwater objects based on sonar data. It uses Logistic Regression to distinguish between metal cylinders (mines) and rocks.

Project Overview
The dataset contains sonar signals collected from various angles. The model is trained to recognize patterns in these signals to determine if the object detected is a rock (labeled as 'R') or a mine (labeled as 'M').

Workflow
Data Collection: Loading sonar signal data via a CSV file.

Data Processing:

Statistical analysis using describe() and mean() grouped by labels.

Separating features (X) from labels (Y).

Model Training:

Splitting data into training and testing sets (10% for testing).

Implementing a Logistic Regression model.

Evaluation:

Training Accuracy: ~83.42%.

Testing Accuracy: ~76.19%.

Predictive System: A custom script that takes a single sonar data instance and predicts whether it is a Rock or a Mine.

Dependencies
This project requires the following Python libraries:

numpy (for array processing)

pandas (for data manipulation)

scikit-learn (for model building, splitting data, and accuracy metrics)

Dataset Structure
Rows: 208

Columns: 60 features (sonar signal frequencies) and 1 label column.

Classes:

M: 111 instances (Mines)

R: 97 instances (Rocks)

How to Use
Ensure you have your dataset uploaded as /content/Copy of sonar data.csv.

Run the notebook cells sequentially to train the model.

Use the "Predictive System" section to input new sonar readings for real-time classification.
