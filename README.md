Title: Predicting Therapist Burnout with Machine Learning

Overview

This project employs machine learning to address the critical issue of therapist burnout, affecting 45% of therapists. Using Python and Azure, the study aims to identify burned-out therapists, predict potential burnout cases, and implement preventative measures. The models, including Random Forest and Azure classifiers, offer advanced techniques for classification tasks. The dataset, collected from a 2007 survey, covers various factors contributing to therapist burnout.
Methodology
Data Exploration

    Utilizes a questionnaire dataset from Harvard Dataverse, mapping therapist responses to over 30 columns.
    Independent variables include demographic details, employment status, and problem-solving capabilities.
    Dependent variable is "Burned_Out," labeled as 1 for burnout and 2 for not burned out.

Data Preprocessing

    Handles missing values and drops unnecessary columns.
    Standardizes and balances the dataset using Synthetic Minority Over-sampling Technique (SMOTE).

Feature Selection

    Utilizes SelectKBest and Recursive Feature Elimination with Cross-Validation to identify significant features.

Modelling

    Random Forest Classifier:
        Trains the model using selected features and evaluates its performance.

    GradientBoostingClassifier:
        Applies GradientBoostingClassifier for comparison with Random Forest.

Azure Machine Learning Studio

    Sets up an Azure workspace and explores data using a drag-and-drop interface.
    Cleans, transforms, and splits data, creating a pipeline for model training.
    Trains Two-Class Decision Forest and Two-Class Boosted Decision Tree classifiers.

Results

    Evaluates models based on accuracy, recall, precision, and F1 score.
    Random Forest Classifier achieves the highest accuracy (0.81), followed by GradientBoostingClassifier (0.80).
    Two-Class Decision Forest excels in recall (0.841), crucial for positive instance identification.

Conclusion

    Identifies Two-Class Decision Forest as the preferred model due to higher recall and ease of scalability.
    Emphasizes the importance of recall in correctly identifying burned-out therapists.
    Proposes web deployment for patients to input data for quick evaluation, minimizing legal issues and ensuring accurate assessments.

Future Directions

    Continuous refinement of models to address overfitting.
    Integration of additional factors for a comprehensive study.
    Exploration of legal and ethical considerations in deploying web services for burnout prediction.
