# Customer Churn Prediction Web App

This project is a machine learning-powered web application that predicts whether a bank customer will churn based on input features like age, gender, geography, balance, and credit score. The model is built using TensorFlow and can be deployed with Streamlit or other Python-based frameworks.

## Features

- Predicts customer churn using real-world banking data
- Preprocessing includes Label Encoding and One-Hot Encoding
- Feature scaling using StandardScaler
- Trained using a Sequential Keras model
- Ready for integration into a Streamlit or Flask app

## Model Inputs

The model requires the following input features:
- Geography (encoded)
- Gender (encoded)
- Age
- Balance
- Credit Score
- Estimated Salary
- Number of Products
- Tenure
- Has Credit Card
- Is Active Member

## Target Variable

- Exited (1 if the customer left the bank, 0 otherwise)

## Project Structure
```
├── model_tr.ipynb # Jupyter Notebook for training the model
├── prediction.py # Python script for prediction
├── model.h5 # Trained Keras model
├── scaler.pkl # StandardScaler object
├── label_encoder_gender.pkl # Label encoder for Gender
├── onehot_encoder_geo.pkl # One-hot encoder for Geography
├── Churn_Modelling.csv # Dataset file
├── requirements.txt # Python dependencies
```

## How to Run the App

1. Clone the repository:
```
git clone https://github.com/mharoon1578/churn-prediction.git
cd churn-prediction
```

2. Install required dependencies:
```
pip install -r requirements.txt
```

3. Run the prediction script:
```
python prediction.py
```


## Training the Model

To retrain the model:

1. Open the `model_tr.ipynb` notebook
2. Run all cells in order
3. The following artifacts will be saved:
- Trained model file
- Encoders and scaler

## Example Prediction

Input:
- Geography: France
- Gender: Female
- Age: 42
- Credit Score: 600
- Balance: 50,000
- Tenure: 5
- Number of Products: 2
- Has Credit Card: Yes
- Is Active Member: No
- Estimated Salary: 58,000

Predicted Output: Churn (1)

## Built With

- Python
- Pandas and NumPy
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

## License

This project is open-source and free to use under the terms of the MIT license.

## Author

Muhammad Haroon  
GitHub: [@mharoon1578](https://github.com/mharoon1578)
