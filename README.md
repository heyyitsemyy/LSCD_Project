# LSCD Project
This project is currently a work-and-progress for one of my classes (Medical Informatics Programming Laboratory).

Goal/Objective: Create a machine learning model to identify the best location to extract stem cell in individuals with limbal stem cell deficiency based on eye scans. This is one part of a larger project.

Information:
- ML Model: logistic regression
- Evaluation Metric: Precision and Recall 
- Data Preparation: Created masks and used the Pyradiomics Python Library to extract features from each image (radiomics_features function). Appended labels and normalized each column of the feature matrix. 
- Results: Average Recall: 0.764 Average Precision: 0.820

Functions:
- radiomics_features: creates a feature matrix for training
- mean_norm: normalizes each columns in a data frame
- logreg_classifier: initializes and trains a logistic regression model
- photo_chooser: outputs a list of images above a 85% threshold to be used in the next step of the pipeline
- Evaluation: evaluates the logistic regression model
- logreg_classifier_features:  initializes and trains a logistic regression model w/ given feature matrix

Next steps:
- perform cross-validation to determine the best threshold for image selection
