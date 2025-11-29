# 🏡 House Price Prediction Using Machine Learning  
*A complete ML pipeline + Streamlit Web App*

---

## 📌 Project Overview

This project predicts **house prices** based on features such as:

- Bedrooms  
- Bathrooms  
- Toilets  
- Neighborhood  
- City  
- Furnishing status  
- Serviced / Newly Built status  

It includes:

- End-to-end ML model training  
- Data preprocessing & feature engineering  
- Model selection (Linear Regression, Decision Tree, Random Forest, XGBoost)  
- Streamlit web application  
- Model evaluation & visualization  

---

## 🚀 Features

### ✔ Machine Learning Pipeline
- Removes outliers  
- Handles missing values  
- Replaces 0-values with median  
- One-hot encodes categorical features  
- Standard scaling  
- Log-transform target  
- Trains and compares 4 ML models  

### ✔ Streamlit Web App
- User authentication  
- Interactive prediction form  
- Analytics dashboard  
- Data visualizations  
- Auto-loads trained model + scaler  

### ✔ Saved Artifacts
- `best_model.pkl`  
- `scaler.pkl`  
- `feature_names.pkl`  

*(Stored locally; large models recommended to be stored via Google Drive or Git LFS)*

---

## 🧠 Model Training

Training script:

src/house_price_prediction.py


This script:

- Loads and preprocesses the dataset  
- Trains multiple ML models  
- Selects the best based on **R² Score**  
- Saves the model + scaler  

### Models Tested
- Linear Regression  
- Decision Tree  
- Random Forest  
- XGBoost  

---

## 📊 Model Evaluation

### Metrics:
- **MAE** – Mean Absolute Error  
- **RMSE** – Root Mean Squared Error  
- **R² Score**  

### Plots Generated:
- Actual vs Predicted  
- MAE / RMSE / R² bar charts  
- Feature importance by category  

---

## 📁 Project Structure

house-price-prediction/
│
├── app/
│ └── web.py # Streamlit app
│
├── src/
│ └── house_price_prediction.py
│
├── models/ # Trained ML models
│ ├── best_model.pkl
│ ├── scaler.pkl
│ └── feature_names.pkl
│
├── data/
│ └── Train.csv # Dataset
│
├── requirements.txt
├── README.md
└── .gitignore


---

## ▶️ Running the Streamlit App

Make sure your virtual environment is active:

```powershell
venv\Scripts\Activate.ps1

Then run:
streamlit run app/web.py

If Streamlit isn’t recognized:
python -m streamlit run app/web.py
Your browser will open the app automatically.

Installation
1️⃣ Clone the repository
git clone https://github.com/YOUR_USERNAME/house-price-prediction.git
cd house-price-prediction

2️⃣ Create virtual environment
python -m venv venv
venv\Scripts\Activate.ps1

3️⃣ Install dependencies
pip install -r requirements.txt

🎯 Future Improvements

Deploy app to Streamlit Cloud

Add more advanced ML models

Hyperparameter optimization

Add maps & geospatial features

Add database for saving predictions

👨‍💻 Author

Akinsinde Emmanuel
Machine Learning & Data Science Enthusiast,Mobile application 
Chrisland University

📜 License

This project is licensed under the MIT License.




