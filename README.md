# Employee_Attrition_prediction using Machine Learning


## Project Overview
This project predicts whether an employee is likely to leave the company using Machine Learning. 
The model is trained using employee data such as job role, salary, work experience, and satisfaction level.
This helps organizations identify attrition risks and take preventive actions.

## Project Workflow
1. Data Cleaning
2. Data Preprocessing
3. Feature Selection
4. Model Training
5. Model Evaluation
6. Prediction


## Project structure
employee_attrition
│
├── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── attrition_model.pkl
├── attrition_scaler.pkl
├── attrition_prediction.ipynb
└── README.md


## Dataset
1. Source: IBM HR Analytics Dataset
2. Contains employee-related information such as:
- Age
- Job Role
- Monthly Income
- Work Experience
- Job Satisfaction
3. Target variable: Attrition (Yes / No)


## Data Preprocessing
1. Converted target variable:
- Yes → 1
- No → 0
2. Removed irrelevant columns:
- EmployeeNumber
- EmployeeCount
- Over18
- StandardHours
- Encoded categorical variables using Label Encoding
- Standardized numerical features using StandardScaler
- Split dataset into training (80%) and testing (20%)



## Model Used
- Logistic Regression
- Simple and interpretable classification model
- Suitable for binary classification problems

## Accuracy: ~80% (may vary slightly)



## Model Evaluation
- Accuracy Score
- Confusion Matrix
- Classification Report:
- Precision
- Recall
- F1-score


## Key Insights
- Salary, job satisfaction, and years at company influence attrition
- Logistic Regression provides a solid baseline model
- Balanced dataset improves prediction reliability


## How to Run
- Clone the repository
- Install dependencies:
- pip install pandas numpy scikit-learn joblib
- Run the notebook or script
- Train model → Saved as:
- attrition_model.pkl
- attrition_scaler.pkl
- Run prediction script with new employee data



## Example Prediction
prediction = model.predict(sample)

if prediction[0] == 1:
    print("⚠️ Employee likely to leave")
else:
    print("✅ Employee likely to stay")

    
## Project Highlights
- End-to-end Machine Learning pipeline
- Real-world HR analytics use case
- Model training, evaluation, and deployment-ready files
- Beginner-friendly project for interviews



## Future Improvements
- Use advanced models (Random Forest, XGBoost)
- Perform hyperparameter tuning
- Feature engineering (e.g., income-to-experience ratio)
- Deploy using Streamlit or Flask

## Author

Employee Attrition Prediction ML Project by  Hema Priya S.
