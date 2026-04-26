1. Exploratory Data Analysis (EDA)

Before building the model, I performed detailed EDA to understand the dataset:

Checked feature distributions and data types
Identified relationships between features and target variable
Visualized patterns in key medical attributes
Detected important features like chest pain type, thalach, and oldpeak

This step helped in understanding which features are most influential for heart disease prediction.

2. Data Preprocessing & Pipeline

To ensure clean and consistent input for the model:

Handled categorical and numerical features separately
Applied encoding for categorical variables
Scaled numerical features where required
Built a complete preprocessing pipeline using Scikit-learn

This ensured that both training data and user input follow the same transformation process.

3. Model Training
Trained a DecisionTreeClassifier model using the processed dataset
Used a pipeline-based approach for better structure and reusability
Evaluated performance using accuracy and confusion matrix

The Decision Tree model was selected because it provides better interpretability and works well with structured medical data.

4. User Input Prediction System

I built an interactive prediction function where:

User enters medical details manually
Input is transformed using the same preprocessing pipeline
Model predicts whether the person is at risk of heart disease
5. Explainable AI using SHAP

To make the model interpretable, I integrated SHAP values:

Computed SHAP values for user input
Visualized feature contribution for each prediction
Identified how each feature pushes prediction toward risk or no risk
Key Insight from SHAP

Instead of only giving a prediction (0 or 1), the model also explains:

Which features increased the risk
Which features decreased the risk
Relative importance of each feature in final prediction

This makes the model transparent and medically interpretable.

Example Output Behavior
Model predicts: High / Low risk of heart disease
SHAP explains:
Positive impact features (increase risk)
Negative impact features (reduce risk)
Strength of each feature contribution
Tools & Libraries Used
Pandas, NumPy
Scikit-learn (Pipeline, preprocessing, DecisionTreeClassifier)
Matplotlib, Seaborn (EDA visualization)
SHAP (model interpretability)
Key Learning Outcomes
Learned end-to-end ML pipeline development
Understood importance of EDA before modeling
Built structured preprocessing pipelines
Implemented real-world model interpretability using SHAP
Gained experience in explainable AI for healthcare data
Conclusion

This project demonstrates not only how to build a predictive model for heart disease but also how to make it explainable. Using SHAP values, the model becomes transparent, allowing users to understand why a specific prediction was made instead of treating it as a black box.
