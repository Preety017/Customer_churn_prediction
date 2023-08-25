# Customer_churn_prediction
"Predict customer churn using Random Forest. Jupyter Notebook covers data preprocessing, model training, evaluation, and API deployment."
Customer churn prediction involves identifying customers who are likely to stop using a service or product. In this project, we use the Random Forest machine learning algorithm to predict customer churn based on historical data.

## Project Overview

This project demonstrates how to build a customer churn prediction model using the Random Forest algorithm and deploy it for making predictions. The steps include data preprocessing, model training, saving the model using `pickle`, and creating an endpoint to predict customer churn using sample input.

## Implementation

1. **Model Training and Saving:**
   - The Random Forest model is trained on historical customer data.
   - The trained model is saved to a file named `rf_model.sav` using `pickle`.

2. **Data Scaling:**
   - A scaler (`df`) is used to preprocess input data before prediction.
   - The scaler is saved to a file named `rf_scaler.pkl` using `joblib`.

3. **Making Predictions:**
   - A function `return_prediction` takes a trained model and sample input.
     
4. ## Usage

1. Clone the repository: git clone https://github.com/Preety017/Customer_churn_prediction.git 
2. Navigate to the project directory: cd Customer_churn_prediction
3. Install the required libraries (assuming you have Python and pip installed): pip install -r requirements.txt
4. Open and run the Jupyter Notebook: jupyter notebook Customer_Churn_Prediction.ipynb
5. Use the provided code for making predictions using the trained model.

5. ## Sample Prediction

```python
# Sample input for prediction
rf_input = {
 'CustomerID': 1,
 'Age': 63,
 'Gender': 0,
 'Subscription_Length_Months': 17,
 'Monthly_Bill': 73.36,
 'Total_Usage_GB': 236
}
# Make a prediction using the loaded model and sample input
prediction = return_prediction(rf_Model, rf_input)
print("Predicted Class:", prediction)

6. ## License: This project is licensed under the MIT License.




  
  
 

   
   



   - Sample input is provided in the `rf_input` dictionary.
   - The function returns a prediction class for customer churn.

## Usage

1. Clone the repository:
