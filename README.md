# demo-ML-project
 Project Overview
This project demonstrates a complete Machine Learning pipeline using the K-Nearest Neighbors (KNN) algorithm to classify iris flowers into 3 species based on their physical measurements.

 
Dataset

Name: Iris Dataset (built-in from sklearn)
Samples: 150 (50 per class)
Features: 4

FeatureDescriptionSepal LengthLength of sepal (cm)Sepal WidthWidth of sepal (cm)Petal LengthLength of petal (cm)Petal WidthWidth of petal (cm)

Target Classes: Setosa, Versicolor, Virginica


Pipeline Steps

Step 1 — Import Libraries
All necessary libraries are imported including sklearn modules for modeling and evaluation.

Step 2 — Load & Explore Data
The Iris dataset is loaded and converted into a pandas DataFrame. Basic exploration is done using .head(), .describe(), and .value_counts().

Step 3 — Split Data
Data is split into 80% training and 20% testing sets using train_test_split with random_state=42 for reproducibility.

Step 4 — Feature Scaling
StandardScaler is applied to normalize features. The scaler is fit only on training data and then applied to both train and test to prevent data leakage.

Step 5 — Train Model
A KNN classifier with K=5 is trained on the scaled training data.

Step 6 — Evaluate Model
Model is evaluated using:

>>Accuracy Score
>>Classification Report (Precision, Recall, F1-score)


** Results
MetricScoreAccuracy~100% (KNN performs very well on Iris)PrecisionHigh across all 3 classesRecallHigh across all 3 classes

