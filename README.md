# 🏥 Medical Insurance Cost Prediction Using Machine Learning

This project demonstrates how to build a machine learning model to predict the medical insurance cost of individuals based on demographic and lifestyle features such as age, gender, BMI, number of children, smoking status, and region.

## 📌 Project Overview

The goal of this project is to build a regression model that can predict the **insurance charges** a person is likely to incur. This is achieved using **Linear Regression**, and the workflow includes data preprocessing, visualization, model training, evaluation, and prediction.

## 📊 Dataset

- **Source**: [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Features**:
  - `age`: Age of the primary beneficiary
  - `sex`: Gender (male/female)
  - `bmi`: Body mass index
  - `children`: Number of children covered by insurance
  - `smoker`: Smoking status (yes/no)
  - `region`: Residential region in the US
  - `charges`: Medical insurance cost (target variable)

## 🔧 Technologies Used

- **Python** (Jupyter Notebook)
- **Libraries**:
  - `pandas` for data manipulation
  - `numpy` for numerical operations
  - `matplotlib` and `seaborn` for data visualization
  - `scikit-learn` for model training and evaluation

## 🧪 Workflow

1. **Data Collection & Exploration**
   - Load and inspect dataset
   - Analyze distribution of features
2. **Data Preprocessing**
   - Encode categorical features (sex, smoker, region)
   - Check for missing values
3. **Feature Engineering**
   - Split data into features (X) and target (y)
   - Train-test split (80/20)
4. **Modeling**
   - Train a **Linear Regression** model
   - Evaluate with **R² score**
5. **Prediction System**
   - Accept custom user input
   - Predict insurance cost using trained model

## 📈 Model Performance

- Target: Achieve an **R² score of ~0.75**, indicating the model explains 75% of the variance in medical insurance costs.

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/medical-insurance-prediction.git
   cd medical-insurance-prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   - Open `insurance_cost_prediction.ipynb` in Jupyter Notebook
   - Follow the step-by-step cells

## 🔮 Example Prediction

```python
# Sample input: [age, sex, bmi, children, smoker, region]
# Encoded as: [19, 1 (female), 27.9, 0, 0 (non-smoker), 2 (southeast)]
model.predict([[19, 1, 27.9, 0, 0, 2]])  # ➝ Expected output: ~$3,756
```

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](../../issues).