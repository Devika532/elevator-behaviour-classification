# elevator-behaviour-classification
Machine learning project exploring synthetic behavioural data to classify elevator users using Logistic Regression, SVM (RBF) and Random Forest
# Elevator User Classification Project

This repository contains the full code, dataset, and results for my 7072CEM Machine Learning coursework at Coventry University. The aim of the project is to investigate whether elevator button-press patterns can be used to classify different categories of building occupants. A realistic synthetic dataset was generated to simulate the behaviour of students, faculty, cleaners, visitors, and contractors, and several supervised learning models were trained and evaluated on this data.

---

## 📁 Repository Contents

- **Elevator_Classification_Project.ipynb**  
  Full notebook containing data generation, preprocessing, feature engineering, model training, and visual outputs.

- **model_training.py**  
  Python script that trains all models, tunes the hyperparameters, evaluates performance, and saves all figures.

- **data_generation.py**  
  Stand-alone script used to create the synthetic dataset.

- **synthetic_elevator_dataset.csv**  
  The dataset used for training and evaluation.

- **figures/**  
  Folder containing confusion matrices, feature-importance plots, and any additional saved images.

- **requirements.txt**  
  List of Python dependencies required to run the project.

- **README.md**  
  Project overview and instructions.

---

## 🧠 Project Overview

The project explores how elevator interaction data can reveal behavioural patterns linked to different groups of building users. Each record in the dataset represents a single elevator trip and includes features such as:

- Floors pressed  
- Number of buttons pressed  
- Longest consecutive run  
- Floor span  
- Basement and ground-floor usage  
- Weekend indicator  
- Time of day (hour, sine, cosine encoding)

Three supervised learning models were developed:

1. **Logistic Regression (One-vs-Rest)**  
2. **Support Vector Machine (RBF kernel)**  
3. **Random Forest Classifier**

GridSearchCV was used to tune each model, and macro-F1 was the primary metric.

---

## 📦 Installation

To install the required packages, run:

```bash
pip install -r requirements.txt

## ▶️ How to Run the Project
Run the main training pipeline
python model_training.py
This will:
Load the dataset
Preprocess the features
Train all three models
Perform hyperparameter tuning
Print accuracy and macro-F1 results
Save confusion matrices and feature-importance plots into figures/

