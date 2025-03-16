🍷 Wine Quality Prediction with Machine Learning

📖 Project Overview

This project aims to predict wine quality using Machine Learning techniques. The dataset contains physicochemical properties of white wine samples and their respective quality ratings. The objective is to build a model that can classify wines as good or bad/medium based on these properties.

📊 Dataset and Problem Definition

Dataset: winequality-white.csv

Source: UCI Machine Learning Repository

Target Variable: quality (originally a multiclass variable from 3 to 9)

Binary Classification: Wines with quality > 6 are labeled as 1 (good), while those with quality ≤ 6 are labeled as 0 (bad/medium).

📊 Visualizations

1️⃣ Wine Quality Distribution

Before and after binarization of quality:



2️⃣ Feature Correlation Matrix

Understanding the relationships between features:


3️⃣ Confusion Matrix - Best Model

Performance evaluation of the final Random Forest model:


4️⃣ Model Performance Comparison

Comparison of Accuracy, F1-Score, and Balanced Accuracy across models:


🏆 Models Tested and Comparison

Several Machine Learning models were tested to find the best classifier:

Model

Accuracy

F1-Score

Balanced Accuracy

Logistic Regression

0.7201

0.5294

0.7272

Decision Tree

0.8095

0.8088

0.7124

KNN

0.8581

0.8451

0.7199

Random Forest (Best Model)

0.8601

0.8547

0.7579

The Random Forest Classifier provided the best results and was selected as the final model.

⚙️ How to Run the Project

1️⃣ Clone the Repository

git clone https://github.com/yourusername/wine-quality-prediction.git
cd wine-quality-prediction

2️⃣ Install Dependencies

pip install -r requirements.txt

3️⃣ Run the Notebook

Open Wine_quality_Yut_Rocio.ipynb in Jupyter Notebook and execute all cells.

🔮 Possible Improvements

Multiclass Classification: Instead of binarizing quality, use all original categories (3-9).

Further Hyperparameter Tuning: Continue refining models for better performance.

API Deployment: Create a REST API with Flask/FastAPI to make real-time predictions.

📂 Direct Links to Images

📊 Model Performance Comparison📊 Correlation Matrix📊 Distribution of Binarized Wine Quality📊 Distribution of Wine Quality Ratings

🚀 Feel free to contribute or suggest improvements!