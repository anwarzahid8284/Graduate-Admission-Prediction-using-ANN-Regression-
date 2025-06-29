# 🎓 Graduate Admission Prediction using ANN (Regression)

This project aims to predict the **Chance of Admission** of a student into a graduate program based on academic and profile features using an **Artificial Neural Network (ANN)**. This is a **regression problem** solved using deep learning techniques.

---

## 📌 Problem Statement

Predict the likelihood (`Chance of Admit`) that a student will be admitted to a graduate school given features like:

- GRE Score
- TOEFL Score
- University Rating
- Statement of Purpose (SOP) Strength
- Letter of Recommendation (LOR) Strength
- Undergraduate CGPA
- Research Experience

---

## 📊 Dataset

Each row in the dataset represents a student profile:

| Feature            | Description                                  |
|--------------------|----------------------------------------------|
| GRE Score          | Graduate Record Exam Score (out of 340)      |
| TOEFL Score        | English Proficiency Test (out of 120)        |
| University Rating  | University's rating (1 to 5)                 |
| SOP                | Statement of Purpose strength (1 to 5)       |
| LOR                | Letter of Recommendation strength (1 to 5)   |
| CGPA               | Undergraduate GPA (out of 10)                |
| Research           | 1 if research experience, else 0             |
| Chance of Admit    | Target variable (0.0 to 1.0)                 |

---

## 🧠 Model Architecture (ANN)

A fully connected feedforward neural network is used:

- **Input Layer:** 7 features
- **Hidden Layers:** Dense layers with ReLU activation
- **Output Layer:** 1 neuron with linear activation (for regression)

```python
model = Sequential()
model.add(Dense(7,activation="relu",input_dim=7))
model.add(Dense(7,activation="relu"))
model.add(Dense(1,activation="linear")) # for regression problem the activation function always linear

```

## 📈 Loss Curve
![Loss Curve](images/loss1.png)


## 📉 Model Evaluation

| Metric                    | Value   |
|---------------------------|---------|
| Mean Squared Error (MSE)  | 0.0024  |
| Mean Absolute Error (MAE) | 0.0342  |
| **R² Score**              | 0.9684  |



---

## 🤖 Neural Network Humor

> **"My neural network has trust issues... it always overfits."**  
> **"I told my model to relax — now it just drops out randomly!"**


