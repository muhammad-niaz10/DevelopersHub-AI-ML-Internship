DevelopersHub AI/ML Engineering Internship – Final Project Portfolio
Overview

This repository contains my completed AI/ML Engineering Internship tasks for DevelopersHub Corporation. The projects cover the full machine learning lifecycle, from data exploration and preprocessing to model training, evaluation, explainability, and LLM-based chatbot development.

The work demonstrates practical understanding of:

Data analysis and visualization (EDA)
Machine learning pipelines
Model training and evaluation
Explainable AI using SHAP
Prompt engineering
Large Language Models (Mistral API)
LangChain-based chatbot architecture
Completed Tasks
Task 1: Iris Dataset Exploration and Visualization
Task 3: Heart Disease Prediction with Explainable AI (SHAP + DecisionTreeClassifier)
Task 4: General Health Query Chatbot using Mistral API + LangChain
Repository Structure
DevelopersHub-AI-ML-Internship/
│
├── Task-1-Iris-EDA/
├── Task-3-Heart-Disease-Prediction/
├── Task-4-Health-Chatbot/
│
└── README.md
Core Concepts Covered Across All Tasks
1. Exploratory Data Analysis (EDA)

Across Tasks 1 and 3, I performed structured EDA to understand data behavior before modeling.

Key steps included:

Understanding dataset structure (rows, columns, data types)
Identifying missing values and data quality issues
Statistical summary using descriptive analysis
Feature distribution analysis
Relationship visualization between variables

EDA helped in identifying important patterns and feature importance before training any model.

2. Data Preprocessing & Pipelines

In Task 3, I implemented a full preprocessing pipeline using Scikit-learn.

Key steps:

Handling categorical and numerical features separately
Encoding categorical variables
Feature scaling where required
Building a reusable ML pipeline

This ensured consistency between training data and real-time user input prediction.

3. Model Training & Evaluation
Task 3 Model: DecisionTreeClassifier

A Decision Tree Classifier was used for heart disease prediction due to its interpretability and suitability for structured medical data.

Evaluation techniques:

Accuracy score
Confusion matrix
Model performance analysis

This helped evaluate how well the model generalizes to unseen data.

4. Explainable AI (SHAP)

To move beyond black-box predictions, SHAP (SHapley Additive Explanations) was integrated.

Key contributions:

Computed SHAP values for individual predictions
Visualized feature impact on model output
Explained why a prediction was made, not just what was predicted
SHAP Insights:

The model explains:

Features that increase heart disease risk
Features that decrease risk
Relative contribution of each feature in final decision

This made the model transparent and interpretable, especially for healthcare use cases.

5. User Input Prediction System

A real-time prediction system was developed where:

Users enter medical attributes manually
Input is processed using the trained pipeline
Model predicts heart disease risk (Yes/No)
SHAP explanation is generated for transparency

This simulates a real-world medical decision support system.

6. Large Language Model (LLM) Chatbot
Task 4: Health Query Chatbot

A conversational AI system was built using:

Mistral API (LLM)
LangChain framework
7. Prompt Engineering

A system prompt was designed to control chatbot behavior:

Acts as a helpful health assistant
Provides general health information only
Avoids diagnosis or unsafe medical advice
Maintains simple and safe communication

Prompt engineering ensured controlled, safe, and relevant outputs.

8. LangChain Message Architecture

The chatbot uses structured message handling:

SystemMessage → defines behavior rules
HumanMessage → user queries
AIMessage → model responses

This structure enables contextual conversation memory instead of isolated responses.

9. Chatbot Memory Handling

LangChain message history was used to maintain conversation flow:

Stores previous interactions
Maintains context across multiple queries
Improves response relevance over time

This makes the chatbot more natural and interactive.

10. Safety in AI Systems

To ensure responsible AI usage:

No medical diagnosis is provided
Only general health guidance is given
Users are encouraged to consult professionals for serious conditions
Tools & Technologies Used
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
DecisionTreeClassifier
SHAP (Explainable AI)
Mistral API (LLM)
LangChain
Prompt Engineering
Key Learning Outcomes

Through this internship, I gained practical experience in:

End-to-end machine learning workflow
Data preprocessing and feature engineering
Model training and evaluation techniques
Explainable AI using SHAP
Real-time prediction systems
Building LLM-based applications
Prompt engineering for controlled AI responses
LangChain-based chatbot architecture
Designing safe and responsible AI systems
Conclusion

This project demonstrates a complete AI/ML workflow starting from data analysis to machine learning modeling and extending into modern LLM-based applications.

It reflects both technical and conceptual understanding of:

Traditional machine learning (EDA → Model → Evaluation → SHAP)
Modern AI systems (LLMs, LangChain, Prompt Engineering)

Overall, this internship strengthened my ability to build real-world, interpretable, and production-style AI applications.
