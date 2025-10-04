Autism Spectrum Disorder Prediction

This project is a machine learning based web application designed to predict the likelihood of Autism Spectrum Disorder (ASD) in individuals.
The app uses a trained Random Forest Classifier to analyze questionnaire scores and basic medical details, then returns a prediction along with a confidence score and overall model accuracy.

What the Project Does

* Collects questionnaire responses (A1–A10 scores) and personal/medical details (gender, jaundice history, autism family history).
* Uses a trained ML model to predict ASD likelihood (Yes/No).
* Provides:

  * Individual confidence score for the prediction
  * Overall accuracy of the model
  * Visualization of feature importance

Requirements

The project uses the following Python libraries:

* Flask → for the web application framework
* Pandas → for data manipulation and handling datasets
* NumPy → for numerical computations
* SciPy → for scientific computing support
* Scikit-learn → for training and using the Random Forest Classifier

How It Works

1. Data Preprocessing

   * Loads dataset (`autism_data.csv`)
   * Encodes categorical variables (gender, jaundice, autism family history)
   * Splits data into training and testing sets

2. Model Training

   * A Random Forest Classifier is trained on the processed dataset
   * Model accuracy is calculated and saved
   * Feature importance is plotted for explainability

   Web Application

   * Flask app (`app.py`) serves a web interface
   * User submits inputs via an HTML form
   * Model predicts ASD likelihood and displays results with confidence score

Outputs
* Prediction result: Yes / No
* Confidence score: Percentage confidence for the prediction
* Model accuracy: Overall performance of the trained model
* Feature importance plot: Bar chart showing influential features

Purpose

The project demonstrates how machine learning can be integrated with a web application to build an accessible tool for ASD prediction. While it is not a medical diagnostic system, it serves as a 
learning project combining:

* Data science (model training and evaluation)
* Web development (Flask app)
* Visualization (feature importance)
