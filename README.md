# Medical-Medicine-Recommendation-System
A machine-learning powered healthcare assistant that predicts diseases based on symptoms and recommends medicines, precautions, workouts, and diets.

This system uses multiple datasets like symptom severity, description, medications, precautions, diet suggestions, and workout plans.
Models are trained using classical ML algorithms and the entire pipeline is structured for real-world medical assistance.

**Key Features**

✔ Predict disease based on symptoms
✔ Recommend medicines
✔ Suggest precautions for predicted disease
✔ Provide workouts & diet plans
✔ Explains symptoms in simple language
✔ Uses cleaned symptom dataset + trained ML model
✔ Exported models for deployment (svc.pkl, label_encoder.pkl)

## Project Structure
Medical-Disease-Prediction
│
├── README.md
├── Training.csv
├── Symptom-severity.csv
├── description.csv
├── medications.csv
├── precautions_df.csv
├── diets.csv
├── workout_df.csv
├── symtoms_df.csv
├── all_cleaned_symptoms.pkl
├── symptoms_df.pkl
├── svc.pkl
├── label_encoder.pkl
│
├── medicine recommendation.ipynb
├── medicine recommendation-checkpoint.ipynb
├── medicine, medical recommendation.ipynb
├── medicine, medical recommendation-checkpoint.ipynb

## Model Overview

This project uses a Support Vector Classifier (SVC) trained on cleaned symptom severity data.

Algorithms Used

Support Vector Machine (SVC)

Label Encoding

Custom Symptom Indexing

Probability-based ranking

Files
File	Purpose
svc.pkl	Trained machine learning model
label_encoder.pkl	Encodes disease labels
all_cleaned_symptoms.pkl	Cleaned symptom matrix
symptoms_df.pkl	Final processed symptom dataset

## Datasets
Dataset	Description
Training.csv	Disease vs Symptoms dataset
Symptom-severity.csv	Severity weight of each symptom
description.csv	Disease descriptions
medications.csv	Recommended medical treatments
precautions_df.csv	Safety precautions
diets.csv	Diet suggestions
workout_df.csv	Physical workout recommendations

## How It Works

User enters symptoms

Program converts symptoms → encoded format

ML model predicts the disease

Output includes:

Disease name

Recommended medicines

Precautions

Diet

Workout

Description of disease

## Use Cases

Symptom Checker Applications

Telemedicine Platforms

AI Health Assistants

Hospital Triage Systems

Personal Health Monitoring

## Limitations

⚠ Not a replacement for a doctor
⚠ Model accuracy depends on limited dataset
⚠ Generalized recommendations
⚠ No real medical validation yet

## Future Improvements

Add FastAPI backend for deployment

Connect with a React or Streamlit frontend

Add deep learning symptom embedding model

Build a chatbot-style symptom checker

Expand dataset with real-world clinical data
