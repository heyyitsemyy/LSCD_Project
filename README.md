# LSCD Project
This project is currently a work-and-progress for one of my classes (Medical Informatics Programming Laboratory).

Objective: Create a machine learning model to identify the best location to extract stem cell in individuals with limbal stem cell deficiency based on eye scans. This is one part of a larger project.

Information:
- My model is a logistic regression model
- Evaluation Metric: Precision and Recall 


Functions:
- radiomics_features: creates a feature matrix for training
- mean_norm: normalizes each columns in a data frame
- logreg_classifier: initializes and trains a logistic regression model
- photo_chooser: outputs a list of images above a 85% threshold to be used in the next step of the pipeline
- Evaluation: evaluates the logistic regression model
- logreg_classifier_features:  initializes and trains a logistic regression model w/ given feature matrix

Next steps:
- perform cross-validation to determine the best threshold for image selection
