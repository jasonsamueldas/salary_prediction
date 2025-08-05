
# Salary Estimation App

A **Streamlit-based web application** that predicts employee salary based on:
- Years at the company
- Satisfaction level
- Average monthly working hours

This project is the culmination of a **Machine Learning Placement Training Capstone**, featuring multiple ML models and an interactive frontend.

---

## Features

- User-friendly UI built with **Streamlit**
- Visual feedback with **Plotly** bar charts
- Real-time predictions using a trained **Linear Regression** model
- Scaled inputs using **StandardScaler**
- Fun UI enhancements (like confetti balloons)

---

## ML Models Used

The training notebook explores and compares:
- **Linear Regression** *(Best model - used in app)*
- **Support Vector Regressor (SVR)** with GridSearchCV
- **Random Forest Regressor** with hyperparameter tuning

---

## Project Structure

```
├── app.py                        # Streamlit app code
├── ml_placement_training_capstone_project.py   # Model training notebook (Colab)
├── scaler.pkl                   # Saved StandardScaler
├── model.pkl                    # Trained Linear Regression model
├── employee_attrition_data.csv  # Dataset (not included here)
└── README.md                    # This file
```

---

## Requirements

Install the following Python packages:

```bash
pip install streamlit joblib scikit-learn pandas numpy plotly matplotlib seaborn
```

---

## How to Run the App

1. Clone this repo or download the files.
2. Ensure `scaler.pkl` and `model.pkl` are present in the same directory.
3. Run the Streamlit app:

```bash
streamlit run app.py
```

> Note: Replace the hardcoded image path in `app.py` with a valid image URL or a local file in the same directory.

---

## Sample Input Features

- **Years at Company:** `0` to `20`
- **Satisfaction Level:** `0.0` to `1.0`
- **Average Monthly Hours:** `120` to `310`

---

## Example Output

Upon entering valid inputs and clicking **Predict Salary**, the app:
- Displays the predicted salary in INR
- Shows a bar chart of your input features

---

## Dataset Info

- Used a synthetic `employee_attrition_data.csv` dataset.
- Features include job satisfaction, work hours, tenure, and salary.

---

## Evaluation Metrics

Evaluated model performance using:
- **Mean Absolute Error**
- **Mean Squared Error**

---

## Author

**Jason Samuel Das**  
