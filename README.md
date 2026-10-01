# WDCS-CLR
Here My Practical Part in WDCS Project 


📌 Project Overview

This project demonstrates a complete Machine Learning workflow—from data acquisition and exploratory data analysis (EDA) to feature engineering, pipeline creation, model training, and performance evaluation.


📊 Dataset Information

    Source: iWildCam Dataset accessed via kagglehub.
    Inputs: Image file records and metadata files (metadata.csv & categories.csv).
    Engineered Features: Temporal features extracted from timestamps (year, month, hour) along with spatial identifiers (location, sequence_remapped).
    Target Variable: Species class labels (y / category_id).

🔄 Machine Learning Pipeline

    Data Collection & Exploration:
        Downloaded dataset using kagglehub and inspected raw directory structures.
        Examined data types (dtypes), verified record counts, and analyzed target variable distributions.

    Data Preprocessing & Feature Engineering:
        Parsed timestamps into datetime objects to extract year, month, and hour.
        Filtered out non-predictive identifiers and handled missing values (dropna()).

    Data Splitting:
        Split data into 80% training and 20% testing sets (test_size=0.20, random_state=42).

    Model Training:
        Built an sklearn.pipeline.Pipeline combining StandardScaler for feature normalization and LogisticRegression for classification.

    Model Evaluation:
        Evaluated model performance using Accuracy Score, Classification Report (Precision, Recall, F1-Score), and ConfusionMatrixDisplay.

📈 Model Performance

Test Accuracy 	[ 0.43 / 43.69% ]

