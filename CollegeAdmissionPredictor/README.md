# 🎓 College Admission Predictor

A Machine Learning project that predicts a student's probability of admission to a university based on academic and profile-related factors such as GRE score, TOEFL score, CGPA, SOP strength, LOR strength, university rating, and research experience.

## 📌 Project Overview

The goal of this project is to build a regression model capable of estimating a student's chance of admission using historical admission data. The project follows the complete machine learning workflow, including data preprocessing, exploratory data analysis, model training, evaluation, and prediction.

## 📊 Dataset Features

The dataset contains the following features:

| Feature | Description |
|----------|------------|
| GRE | Graduate Record Examination Score |
| TOEFL | Test of English as a Foreign Language Score |
| University Rating | Rating of the University (1–5) |
| SOP | Statement of Purpose Strength (1–5) |
| LOR | Letter of Recommendation Strength (1–5) |
| CGPA | Undergraduate CGPA |
| Research | Research Experience (0 = No, 1 = Yes) |
| Probability | Chance of Admission (Target Variable) |

## 🔍 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Data shape and structure inspection
- Missing value analysis
- Duplicate value check
- Feature distribution using histograms
- Statistical summary of numerical features
- Data quality validation

### Key Observations

- Most students have GRE scores between 310–330.
- TOEFL scores are concentrated around 100–115.
- Higher CGPA generally corresponds to a higher admission probability.
- Research experience positively influences admission chances.
- The dataset contains no significant missing values.

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

- Removed unnecessary columns such as Serial Number.
- Renamed columns for easier access.
- Verified data types.
- Checked for hidden missing values represented by zeros.
- Prepared feature and target variables.

## 🤖 Machine Learning Models

Multiple regression algorithms were trained and evaluated:

- Linear Regression
- Lasso Regression
- Support Vector Regressor (SVR)
- Decision Tree Regressor
- Random Forest Regressor
- K-Nearest Neighbors Regressor (KNN)

Hyperparameter tuning was performed using GridSearchCV where applicable.

## 📈 Model Evaluation

Models were compared using cross-validation and regression metrics.

Evaluation Metrics:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

### Best Performing Model

Linear Regression achieved the best overall performance with approximately 81% accuracy during cross-validation.

## 🚀 Example Prediction

Input:

- GRE: 337
- TOEFL: 118
- University Rating: 4
- SOP: 4.5
- LOR: 4.5
- CGPA: 9.65
- Research: 0

Predicted Admission Chance:

92.85%

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

## 📂 Project Structure

text CollegeAdmissionPredictor/ │ ├── Admission prediction.ipynb ├── admission_predict.csv ├── README.md │ └── outputs/ 

## 🎯 Future Improvements

- Deploy the model using Streamlit or Flask.
- Add feature importance visualization.
- Implement SHAP explainability.
- Create an interactive web application.
- Experiment with advanced ensemble models.

## 📚 Learning Outcomes

Through this project, I learned:

- Data preprocessing techniques
- Exploratory Data Analysis (EDA)
- Feature selection
- Regression modeling
- Model evaluation and comparison
- Hyperparameter tuning using GridSearchCV
- End-to-end machine learning workflow

## 👨‍💻 Author

Shiva

If you found this project useful, feel free to star the repository and connect with me.