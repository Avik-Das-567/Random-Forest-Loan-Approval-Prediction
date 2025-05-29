# Random Forest with Streamlit - Loan Approval Prediction
### App Link
* https://random-forest-loan-approval-prediction.streamlit.app/
## Objective
* Predicting Loan Approval Based on Income & Credit Score
* **Example Problem:** We have data with two features -
  * **Income.**
  * **Credit Score.**
  And the output is whether the **loan is approved or not**
## How it Works
* Data is loaded using **`pd.read_csv()`**
* Output column (Yes/No) is converted to 1/0 using **`.map()`**
* **`RandomForestClassifier`** builds many decision trees
* Final answer is given using **majority voting** from the trees
