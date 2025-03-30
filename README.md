MBTI Personality Prediction using Machine Learning:
1. Problem Statement:
   Can we accurately classify individuals into one of 16 MBTI personality types based on their responses to a set of survey questions using machine learning,
   while minimizing the number of questions required for high accuracy ?

2. Dataset Details:
Source: Question-based dataset with personality responses.
Size: 59,999 responses.
Features: 61 questions with responses ranging from -3 to 3.
Target Variable: 16 Personality types (e.g., INFJ, ENFP, ESTJ, etc.).
Initial Approach: Splitting into subtypes (IE, SN, FT, PJ) resulted in poor accuracy due to class balance.

3. Data Preprocessing & Feature Engineering:
Converted categorical personality labels into numerical classes.
Applied feature selection to reduce the number of survey questions while maintaining accuracy.
Experimented with different feature groupings (IE, SN, FT, PJ vs. all features).

4. Solution Approach:
Machine Learning Model: Random Forest Classifier.
Feature Selection: Identified the most important survey questions to minimize redundancy.
Optimization: Reduced the number of questions while maintaining high accuracy.
Voting Mechanism: Used multiple decision trees to improve classification reliability.
Final Accuracy: Achieved 91% accuracy after optimizing the question set.

5. Challenges Faced:
Class Overlap: Some personality types have similar traits, making classification difficult.
Feature Correlation: Many survey questions are highly correlated, leading to redundancy.
Reducing Questions Without Losing Accuracy: Finding the optimal subset of questions was complex.
Generalization Issues: The model needs to perform well on unseen data and not just the training set.
Model Complexity vs. Interpretability: Ensuring a balance between high accuracy and easy interpretability of results.

6. Results & Key Insights:
Accuracy Improvement: Achieved 91% accuracy by optimizing the number of survey questions.
Feature Selection Efficiency: Reduced the number of questions while retaining model performance.
Random Forest Effectiveness: Performed well in handling non-linearity and feature interactions.
Balanced Dataset Impact: The model benefitted from a balanced dataset, improving classification consistency.
Interpretability: Feature importance analysis provided insights into the most influential personality traits.

7. How to Use the Code:
Install required libraries: pip install pandas numpy scikit-learn
Load the dataset and preprocess features.
Train the Random Forest model.
Evaluate performance and analyze feature importance.
Optimize by reducing the number of survey questions.

8. Contributors:
Anushka Kumar - J007
Laavanya Mishra - J035
Yatharth Desai - J075
