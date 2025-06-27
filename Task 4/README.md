# Task 4: Classification with Logistic Regression

## 🔍 Objective
Build a binary classification model using **Logistic Regression** to predict outcomes on a medical dataset.


## 🛠️ Tools & Libraries Used

- **Python**
- **Scikit-learn**
- **Pandas**
- **Matplotlib**


## 📊 Dataset

- **Name**: Breast Cancer Wisconsin Diagnostic Dataset
- **Source**: Built-in dataset from `sklearn.datasets`
- **Target Variable**: `diagnosis` (Malignant = 0, Benign = 1)
- **Features**: 30 numeric features such as radius, texture, perimeter, area, smoothness, etc.

## ⚙️ Steps Followed

1. **Loaded the Dataset** using `sklearn.datasets.load_breast_cancer()`.
2. **Preprocessed the Data**:
   - Split into train/test sets.
   - Standardized features using `StandardScaler`.
3. **Model Training**:
   - Trained a Logistic Regression model using `LogisticRegression()` from `sklearn.linear_model`.
4. **Evaluation**:
   - Calculated metrics: Confusion Matrix, Accuracy, Precision, Recall, F1 Score, ROC-AUC.
   - Visualized ROC Curve.
5. **Threshold Tuning & Sigmoid Explanation**:
   - Demonstrated effect of changing probability threshold on classification.
   - Explained the role of sigmoid in mapping outputs to probabilities.


## 📈 Results

- **Accuracy**: *97%*
- **ROC-AUC**: *0.99*
- The model performs well in distinguishing between benign and malignant tumors.
- ROC Curve shows strong separation between the classes.


## 📌 Key Concepts Explained

- **Logistic Regression**: A linear model used for binary classification that outputs probabilities via the sigmoid function.
- **Sigmoid Function**: 
  \[
  \sigma(z) = \frac{1}{1 + e^{-z}}
  \]
  It maps model output to a probability between 0 and 1.
- **Threshold Tuning**: By changing the classification threshold (default is 0.5), you can shift the model to prioritize precision or recall depending on the use case.


## 🖼️ Visuals

- Confusion Matrix
- ROC Curve
