# Task 1 - Data Cleaning & Preprocessing
Perform data cleaning on raw data for ML

## Tools
- **Python**
- **Numpy**
- **Pandas**
- **Matplotlib/Seaborn**
- **Dataset:** Titanic - Machine Learning from Disaster

## ✅ Steps Covered

### 1. Data Cleaning & Preprocessing
- Handled missing values (e.g., `Age` using median, filled `Embarked` using mode)
- Dropped irrelevant features (`Ticket`, `Name`, `PassengerId`)
- Encoded categorical features:
  - `Sex`: label encoded
  - `Embarked`: one-hot encoded
- Standardized numerical features (`Age`, `Fare`, `SibSp`)
- Removed outliers using the IQR method

### 2. Exploratory Data Analysis (EDA)
- Visualized survival distribution
- Analyzed survival by `gender` and `class`
- Plotted `age` and `fare` distributions by survival
- Explored `family size` vs `survived`
- Correlation heatmap of all numeric features

## 🏆 Best Model
**K-Nearest Neighbors** achieved the highest accuracy on cleaned data : **0.82**
