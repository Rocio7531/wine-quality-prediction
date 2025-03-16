🍷 Wine Quality Prediction - Machine Learning Project

📌 Project Description

This project applies Machine Learning techniques to predict the quality of white wines based on their physicochemical properties. The dataset consists of several features related to the chemical composition of the wine, and the goal is to build a predictive model that accurately classifies wines as good or bad/medium based on these attributes.

🛠 Technologies Used

Python

Pandas (Data manipulation)

Scikit-learn (Machine Learning model training & evaluation)

Matplotlib & Seaborn (Data visualization)

Google Colab / Jupyter Notebook

📂 Repository Structure

📂 Wine_Quality_Prediction
├── 📄 README.md (Project documentation)
├── 📂 data/ (Dataset files)
├── 📂 notebooks/ (Jupyter/Colab Notebooks with full code)
├── 📂 scripts/ (Python scripts for model training and evaluation)
├── 📄 requirements.txt (List of necessary libraries)
├── 📂 results/ (Graphs, visualizations, and final model evaluation)

📊 Dataset Overview

The dataset consists of 4,898 rows and 12 features. Below is a description of each variable:

fixed acidity: Concentration of fixed acids in the wine.

volatile acidity: Amount of volatile acids contributing to vinegar taste.

citric acid: Presence of citric acid, adding freshness to wine.

residual sugar: Sugar remaining after fermentation.

chlorides: Salt content affecting the wine's taste.

free sulfur dioxide: Free SO₂ used as a preservative.

total sulfur dioxide: Total amount of SO₂ present.

density: Density of the wine.

pH: Acidity level of the wine.

sulphates: Sulfate concentration contributing to preservation.

alcohol: Alcohol content in the wine.

quality: Original wine quality score (0-10 scale, based on expert ratings).

🔎 Exploratory Data Analysis (EDA) & Data Preprocessing

1️⃣ Handling Missing Values

Checked for missing values and ensured data completeness.

Outliers in residual sugar and volatile acidity were analyzed.

2️⃣ Feature Engineering & Column Transformation

Created a new binary classification label:

Wines with quality > 6 labeled as 1 (good).

Wines with quality ≤ 6 labeled as 0 (bad/medium).

Standardized features using StandardScaler to prevent scale bias.

Analyzed correlations between features to avoid multicollinearity.

3️⃣ Data Splitting for Machine Learning

Training & Testing Split (70/30) → X_train, X_test, y_train, y_test.

Validation Split (80/20 within training) → X_train_val, X_test_val, y_train_val, y_test_val.

📈 Machine Learning Models & Hyperparameter Tuning

The following models were tested:

1️⃣ Logistic Regression
2️⃣ Decision Tree
3️⃣ K-Nearest Neighbors (KNN)
4️⃣ Random Forest

Hyperparameter Optimization

Used GridSearchCV for hyperparameter tuning.

Adjusted C values and solver types for Logistic Regression.

Optimized max_depth for Decision Tree & Random Forest.

Experimented with different n_neighbors and distance metrics for KNN.

Model Performance Comparison

Model

Accuracy

F1 Score

Balanced Accuracy

Logistic Regression

0.8056

0.72

0.7272

Decision Tree

0.5471

0.81

0.7124

KNN

0.5568

0.84

0.7199

Random Forest

0.8601

0.85

0.7579

🎨 Data Visualizations Used

📊 Data distribution & feature correlations:



📉 Model evaluation:



🚀 Final Model Selection & Conclusion

📌 Best Model: Random Forest (Accuracy 86.01%)

📌 Why?

Highest accuracy and F1 score, showing strong classification performance.

Outperforms Logistic Regression, Decision Tree, and KNN.

Balanced precision and recall, ensuring good generalization.

Final Decision:

💡 The Random Forest model is chosen for final training using 100% of the data.

🚀 How to Run the Project

1️⃣ Clone the repository

git clone https://github.com/yourusername/Wine_Quality_Prediction.git
cd Wine_Quality_Prediction

2️⃣ Install dependencies

pip install -r requirements.txt

3️⃣ Run the Jupyter Notebook (Google Colab recommended):

import pandas as pd
data = pd.read_csv('data/winequality-white.csv')
data.head()

📎 References

Wine Quality Dataset - UCI Repository

Scikit-learn Documentation

🏆 Author

👤 Rocio Yut📧 rocio.yut@gmail.com🔗 GitHub Profile: Rocio7531

🚀 Feel free to contribute or suggest improvements!