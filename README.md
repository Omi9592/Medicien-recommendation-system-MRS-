🧪 Medicine Recommendation System (MRS)

A machine-learning powered web application that predicts possible diseases based on symptoms and recommends relevant medicines.
Built using Python, Flask, and scikit-learn — with a clean UI and a trained classification model.

📌 Table of Contents

Overview

Features

Tech Stack

Project Structure

Installation

How It Works

Usage

Model Training

Future Improvements

Disclaimer

🔍 Overview

The Medicine Recommendation System (MRS) is designed to take user symptoms, predict the likely disease using a machine-learning model, and then recommend suitable medicines from the dataset.

This project is intended for learning and demonstration, not real medical use.

⭐ Features

Symptom input through a simple web interface.

Machine learning model (SVC) trained on custom dataset.

Predicts disease from given symptoms.

Maps predicted disease → suggested medicines.

Clean, responsive frontend.

Easy to retrain and update model.

🛠 Tech Stack

Backend: Python, Flask, scikit-learn, pandas, numpy
Frontend: HTML, CSS
Model: Support Vector Classifier (stored as svc.pkl)

📁 Project Structure
Medicien-recommendation-system-MRS/
│
├── datasets/
│   └── ... datasets used for training
│
├── static/
│   └── style.css  # styling for UI
│
├── templates/
│   ├── index.html
│   └── result.html
│
├── Medicine Recommendation System.ipynb   # model training notebook
├── main.py                               # main Flask application
├── svc.pkl                               # trained ML model
└── README.md

⚙️ Installation
1. Clone the project
git clone https://github.com/Omi9592/Medicien-recommendation-system-MRS-.git
cd Medicien-recommendation-system-MRS-

2. Install dependencies

If you have requirements.txt, run:

pip install -r requirements.txt


Otherwise install manually:

pip install flask pandas numpy scikit-learn

3. Run the app
python main.py


Open your browser at:
👉 http://localhost:5000/

🧠 How It Works
1. User enters symptoms

Input fields → symptoms like:

headache, cough, fever

2. Preprocessing

Inputs are cleaned and converted to numerical format.

3. Model Prediction

The SVC model (svc.pkl) predicts the most likely disease.

4. Medicine Mapping

Based on the predicted disease, medicines are fetched from the dataset.

5. Final Output

User gets:

Predicted disease

List of suggested medicines

🚀 Usage

Open homepage

Enter symptoms

Click Submit

View predicted disease + medicines

Simple and fast.

🧩 Model Training

You can retrain the ML model using the notebook:

Medicine Recommendation System.ipynb


Training pipeline includes:

Reading dataset

Cleaning / preprocessing

Encoding

Training SVC

Exporting model using pickle

After retraining, replace:

svc.pkl

🔮 Future Improvements

Here’s where your project can grow:

Add side-effects and precautions

Include medicine dosage

Add patient details (age, gender, allergies)

Improve UI with Bootstrap / React

Add alternative disease suggestions

Build an API endpoint for mobile apps

⚠️ Disclaimer

This project is not a medical tool.
It should never be used for actual diagnosis or medication decisions.
Consult a certified doctor for real medical issues.
