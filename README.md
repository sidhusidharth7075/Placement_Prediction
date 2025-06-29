# 🎓 Placement Prediction Using Machine Learning

This project aims to predict student placement outcomes and expected salary during campus recruitment using machine learning models—specifically, Random Forest classifiers. The purpose is to provide actionable insights to students and educational institutions for improved career guidance and placement strategies.

---

## 🔍 Final Results

<div align="center">
  <img src="static/images/pl1.png" alt="Dashboard Image" width="100%">
  <img src="static/images/pl2.png" alt="Result Screenshot" width="100%">
  <img src="static/images/pl3.png" alt="Prediction Interface" width="100%">
</div>

---

## 📚 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

---

## 📌 Overview

Campus placements are critical for students' career paths and institutional reputation. This project uses machine learning to:
- Predict whether a student will be placed or not.
- Estimate the salary for students who are expected to be placed.
- Help institutions analyze the factors that affect placement and salaries.

The models are deployed using a Flask-based web application, offering a user-friendly interface for real-time predictions.

---

## 🗂️ Dataset

The dataset includes various student attributes:
- CGPA / academic performance
- Internship experience
- Participation in hackathons
- Technical skills
- Communication skills
- Certifications
- Domain knowledge
- Projects completed
- Final year project quality
- Location preference

Both placement and salary prediction datasets are included:
- `Placement_prediction_data.csv`
- `salary_prediction_data.csv`

---

## Project Structure

```bash

placement-prediction-ml/
│
├── static/
│   └── css/                      # Stylesheets
│   └── images/                   # Image assets
│
├── templates/                    # HTML templates
│   ├── index.html
│   ├── about.html
│   └── result.html
│
├── app.py                        # Main Flask app
├── model.pkl                     # Placement prediction model
├── model1.pkl                    # Salary prediction model
├── requirements.txt              # Required packages
│
├── Placement_prediction.py       # ML model script for placement
├── salary_prediction.py          # ML model script for salary
├── preprocessing.ipynb           # Data cleaning and visualization (jupyter file)
├── Placement_prediction_data.csv
├── salary_prediction_data.csv
└── README.md

```
## Data Preprocessing

The data preprocessing steps include:
1. Handling missing values
2. Encoding categorical variables
3. Feature scaling
4. Feature selection

## Model Training

Two Random Forest classifiers are trained:
1. Placement Prediction Model: Predicts whether a student will be placed
2. Salary Prediction Model: Predicts the salary for placed students

The training process involves:
1. Splitting the data into training and testing sets
2. Initializing the Random Forest classifiers
3. Training the models on the training set
4. Fine-tuning hyperparameters using techniques like Grid Search or Random Search

## Evaluation

The models' performance is evaluated using various metrics, including:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Roc_Auc_Score

## Results

### Placement Prediction Model
- Accuracy: 0.9355
- Precision: 0.9205776173285198
- Recall: 0.9239130434782609
- F1 Score: 0.9222423146473779
- ROC AUC Score: 0.9829810102059323

**CONFUSION MATRIX**:

<img src="static/images/confusion_matrix.png " alt="Alt text" width=auto height=auto>

**ROC CURVE**:

<img src="static/images/roc_curve.png " alt="Alt text" width=auto height=auto>

**FEATURE IMPORTANCE**:

<img src="static/images/feature_importance.png " alt="Alt text" width=auto height=auto>


## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/sidhusidharth7075/Placement_Prediction.git
cd Placement_Prediction
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Server

```bash
python app.py
```

### 5. Access the Website

- not published yet.

## 📧 Contact

For inquiries or collaboration opportunities, reach out via:

- Email: [sidhusidharth7075@gmail.com](mailto:sidhusidharth7075@gmail.com)
- LinkedIn: [LohithSappa](https://www.linkedin.com/in/lohith-sappa-aab07629a/)

---

# ⭐ Don't forget to **star** this repository if you found it helpful!



