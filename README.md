# Heart Disease Predictor

A Streamlit web app that predicts the likelihood of heart disease using a trained logistic regression model.

## Overview

This project loads a pre-trained model and feature metadata from `.pkl` files, collects patient information from a web form, and displays a risk prediction result.

## Features

- Interactive form for health and lifestyle inputs
- Uses a trained logistic regression model for prediction
- Displays high-risk vs low-risk output
- Built with Streamlit for a simple browser-based experience

## Project Files

- `app.py` – Streamlit application
- `LR_heart.pkl` – trained model
- `scaler.pkl` – scaler artifact
- `columns.pkl` – expected feature columns

## Requirements

Install the dependencies:

```bash
pip install streamlit pandas joblib scikit-learn
```

## Run the App

From the project directory:

```bash
streamlit run app.py
```

Then open the local URL shown in the terminal (usually `http://localhost:8501`).

## Input Fields

The app asks for values such as:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Fasting blood sugar
- Resting ECG
- Max heart rate
- Exercise-induced angina
- Oldpeak
- ST slope

## Output

- `High Risk of Heart Disease`
- `Low Risk of Heart Disease`

## Notes

The application expects the model and feature files to remain in the same directory as `app.py`.
