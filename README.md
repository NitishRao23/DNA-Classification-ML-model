# DNA-Classification-ML-model

This project demonstrates how to build and evaluate multiple classification algorithms to predict whether a DNA sequence is a promoter or not, using the UCI Promoter Gene Sequences dataset. Promoters are regions of DNA that initiate transcription of a particular gene, and identifying them is a fundamental problem in bioinformatics.

📂 Dataset

Description: The dataset contains 106 DNA sequences, each with 57 nucleotides.
Target Labels:
+: Promoter
-: Non-Promoter

📌 Project Workflow

1. Data Import & Exploration
Loaded the dataset using pandas from the UCI repository.
Parsed DNA sequences, cleaned unwanted tab characters, and separated nucleotide characters.
Visualized class distribution using seaborn.

2. Data Preprocessing
Converted DNA sequences into individual nucleotide columns.
Transformed categorical nucleotide data into numerical format using pd.get_dummies().
Split the dataset into training and testing sets.\


3. Modeling
Trained and evaluated multiple classification models using 10-fold cross-validation on training data:

K-Nearest Neighbors (KNN)
Gaussian Process Classifier
Decision Tree
Random Forest
Multilayer Perceptron (Neural Network)
AdaBoost
Naive Bayes
Support Vector Machines (SVM) with:
Linear kernel
RBF kernel
Sigmoid kernel



4. Evaluation
Used accuracy_score and classification_report to evaluate model performance.
Printed detailed classification reports for each algorithm on test data.


🛠️ Tech Stack

Python 3
NumPy, Pandas
Scikit-learn
Seaborn, Matplotlib

** Results

Each model's average cross-validation accuracy and standard deviation are printed, along with the final classification report on the test set.

Example output:

Nearest Neighbors: 0.703 (0.122)
Gaussian Process: 0.822 (0.091)
