<div align="center">

# 🚢 Titanic Survival Predictor

### <i>A hands-on machine-learning project exploring the journey from data to deployment.</i>

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

</div>

---

## ✦ Introduction

This project explores a complete machine-learning classification workflow, from preparing passenger data to building an interactive **Streamlit** application.

Rather than focusing only on model accuracy, the project was built to understand the practical steps involved in creating and deploying a machine-learning model.

The app lets users create a passenger profile and receive an **estimated survival probability**, along with predictions from four different models.

---

## ✦ Interactive Showcase

### 🚢 Try the application

[**Launch the Interactive UI →**](https://embers0113.streamlit.app/)

Explore the trained models through the interactive Streamlit application, create your own passenger profile, and view the estimated survival probability.

---

## ✦ How It Works

```text
Raw Data
   ↓
Data Cleaning
   ↓
Feature Engineering
   ↓
Feature Selection
   ↓
Encoding & Scaling
   ↓
Model Training
   ↓
Model Comparison
   ↓
Saved Models
   ↓
Streamlit Application
```

The final model features are:

| Feature | Description |
|---|---|
| `Pclass` | Passenger class |
| `Sex` | Passenger sex |
| `Age` | Passenger age |
| `Title` | Passenger title |
| `FamilySize` | Family group size |
| `IsAlone` | Whether the passenger travelled alone |

---

## ✦ Models

The project compares four classification algorithms:

**Logistic Regression**  
A simple linear model useful for understanding probability-based classification.

**K-Nearest Neighbors**  
A distance-based model that helped demonstrate the importance of feature scaling.

**Decision Tree**  
A rule-based model that makes decisions through learned feature splits.

**Random Forest**  
An ensemble of decision trees used to compare a single tree with a more robust tree-based approach.

---

## ✦ Streamlit Application

The application turns the trained models into an interactive experience.

Users can enter their own:

- Passenger class
- Sex
- Age
- Title
- Family size
- Travel status

Instead of returning only `0` or `1`, the application displays an estimated **survival percentage** using the models' probability outputs.

It also includes a **Historical Doppelgänger** feature that searches for an actual passenger with similar characteristics.

> The probability is a model estimate, not a guarantee or historically exact prediction.

---

## ✦ What I Learned

This project helped me understand several important parts of practical machine learning:

- **Data preprocessing** and why clean input matters.
- **Feature engineering**, particularly creating `Title`, `FamilySize`, and `IsAlone`.
- **Categorical encoding** and converting human-readable information into numerical features.
- **Feature scaling**, especially for distance-based algorithms such as KNN.
- **Model comparison** and why different algorithms can produce different predictions.
- **Model persistence** using Joblib.
- **Inference pipelines**, where new user data must undergo the same transformations used during training.
- **Streamlit application state** and using `st.session_state` for interactive predictions.
- The difference between building a model and building an application around that model.

---

## ✦ Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Joblib` · `Streamlit`

---

## ✦ Running the Project

Install the dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run Streamlit/app.py
```

---

<div align="center">

### <i>Learn the workflow. Understand the model. Build something with it.</i>

</div>
