# Credit Risk Analysis Report

## Overview of the Analysis

The purpose of this analysis was to build and evaluate machine learning models to predict credit risk. Specifically, the analysis involved predicting whether loans are **healthy (low-risk)** or **high-risk** based on historical financial data. The dataset contained financial information about loans, with the `loan_status` column serving as the target variable, where:
- `0` represents **healthy loans**, and
- `1` represents **high-risk loans**.

### Variables:
- The target variable (`y`) was the `loan_status`.
- Features (`x`) included various financial indicators and loan-related attributes.

### Process Overview:
1. **Data Preparation**:
    - The dataset was split into features (`x`) and labels (`y`).
    - The data was further divided into training and testing subsets using `train_test_split`.

2. **Machine Learning Model**:
    - A **Logistic Regression** model was implemented to classify loans as either healthy or high-risk.
    - The model was trained using the training dataset and evaluated using the test dataset.

3. **Evaluation Metrics**:
    - The model's performance was assessed based on accuracy, precision, recall, and F1-score to determine its reliability.

## Results

The results of the logistic regression model are as follows:

- **Accuracy**: 99%
- **Precision**:
    - Class 0 (healthy loans): **100%**
    - Class 1 (high-risk loans): **85%**
- **Recall**:
    - Class 0 (healthy loans): **99%**
    - Class 1 (high-risk loans): **91%**
      
<img width="429" alt="Screenshot 2025-04-26 at 11 59 48 AM" src="https://github.com/user-attachments/assets/729101d9-d7a6-409f-af34-a1b6f89ab8cd" />

## Summary

The logistic regression model demonstrates excellent overall performance, achieving a **99% accuracy score**. It is highly effective at predicting **healthy loans (Class 0)** with a **100% precision** and **99% recall**, meaning it rarely misclassifies healthy loans. For **high-risk loans (Class 1)**, the model provides strong predictions with **85% precision** and **91% recall**, although slightly less accurate than for healthy loans.

The lower performance in predicting high-risk loans can be attributed to the imbalanced dataset, where Class 1 has significantly fewer instances **(619)** compared to Class 0 **(18,765).** This imbalance affects the model's ability to achieve equal performance across both classes.


### Recommendation:
This model is recommended for use by the company due to its high accuracy and strong performance overall. However, improvements could be made by addressing the data imbalance, such as:
- Oversampling or under-sampling the data.
- Applying class weights in the logistic regression model.
- Exploring other algorithms like 'Random Forest' or 'Support Vector Machines.'

These refinements could enhance the model's ability to predict high-risk loans more accurately, further benefiting the company's decision-making process.

# Sources of Help

- Resources from University of Oregon Continuing and Professional Education Data Analytics Boot Camp on 'Supervised Learning.'
- Microsoft Copilot for problem-solving and guidance.

# Acknowledgments

This project was created as part of a professional development challenge inspired by the Module 20 curriculum. Special thanks to the developers of open-source tools and libraries that made this analysis possible.

# Contact

- **Name**: Gurpreet Singh Badrain  
- **Role**: Market Research Analyst & Aspiring Data Analyst  
- **GitHub**: [https://github.com/gbadrain](https://github.com/gbadrain)  
- **LinkedIn**: [http://linkedin.com/in/gurpreet-badrain-b258a0219](http://linkedin.com/in/gurpreet-badrain-b258a0219)  
- **Email**: gbadrain@gmail.com  


