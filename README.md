# Random Forest with Streamlit - Loan Approval Prediction
### App Link
- https://random-forest-loan-approval-prediction.streamlit.app/
---
### What is Random Forest?
- Random Forest is a **machine learning algorithm** that uses **many decision trees** to make a strong prediction.
- **Real-Life Example:** Just like asking advice from **many teachers** to decide if a student passes, Random Forest takes **votes from multiple trees** to give a better result.
- Random Forest is called **Ensemble Model** because it combines many trees.
- It is **more accurate** than using just one decision tree.
- It can be used for **classification (Yes/No)** and **regression (number)**.
---
### Required Python Packages
- **`scikit-learn`** - To build machine learning models
- **`streamlit`** - To build data apps
- **`pandas`** - To work with the dataset
---
### Example Problem
- We have data with two features: **Income** and **Credit Score**.
- The output is whether the **Loan is approved or not**.

| Income | Credit\_Score | Loan\_Approved |
| ------ | ------------- | -------------- |
| 25000  | 600           | No             |
| 30000  | 650           | Yes            |
| 40000  | 700           | Yes            |
| 15000  | 550           | No             |
| 50000  | 750           | Yes            |

---
### How It Works
- The data is loaded using **`pd.read_csv()`**.
- Output column (Yes/No) is converted to 1/0 using **`.map()`**.
- **`RandomForestClassifier`** builds many decision trees.
- Final answer is given using **majority voting** from the trees.
---
