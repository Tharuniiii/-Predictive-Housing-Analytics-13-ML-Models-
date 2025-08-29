# 🏡 Multi-Model Housing Price Prediction Web App (Flask + ML)

This project predicts house prices using multiple Machine Learning models and serves them through a **Flask web application**.  
Users can select from different ML models, input housing features, and get the predicted price instantly.

---

## 🚀 Features
- Trains and evaluates **13 ML models**:
  - Linear Regression, Ridge, Lasso, ElasticNet
  - Polynomial Regression
  - SGD Regressor
  - ANN (MLPRegressor)
  - Random Forest, XGBoost, LightGBM
  - SVM, KNN, Robust Regression
- Saves each trained model as a **pickle file**
- Flask web interface to:
  - Enter input values
  - Select ML model
  - View predicted house price
  - Compare model performances (MAE, MSE, R²) in a results table

---

## 📂 Project Structure

├── data/
│ └── USA_Housing.csv # Dataset
├── models/
│ ├── app.py # Flask app
│ ├── LinearRegression.pkl # Trained models
│ ├── RandomForest.pkl
│ └── ...
├── templates/
│ ├── index.html # Home page (form + model selection)
│ ├── results.html # Prediction output page
│ └── model.html # Model performance table
├── model_evaluation_results.csv # Evaluation metrics of all models
├── train_models.py # Script to train and save models
└── README.md


---

## 🖥️ Sample Input
- Avg. Area Income = `55000`  
- Avg. Area House Age = `5.5`  
- Avg. Area Number of Rooms = `7`  
- Avg. Area Number of Bedrooms = `3`  
- Area Population = `25000`  

## 📊 Sample Output
- Selected Model: **RandomForest**  
- Predicted Price: **$1,580,000**  

(Model performance table screenshot can also be added here 📷)

---

## ⚡ How to Run
1. Clone this repository
   ```bash
   git clone https://github.com/<your-username>/housing-price-flask.git
   cd housing-price-flask/models
2. Train models (if needed)
   ```bash
   python train_models.py
3. Run Flask app
   ```bash
   python app.py
4. Open browser → http://127.0.0.1:50

🛠️ # Tech Stack

Python, Flask

scikit-learn, XGBoost, LightGBM

HTML, CSS (templates)

Pandas, Numpy

📌 # Future Improvements

Add more advanced deep learning models

Deploy on cloud (Heroku/AWS/GCP)

Enhance UI with charts and visualizations

**screenshots** 
<img width="1801" height="864" alt="home page" src="https://github.com/user-attachments/assets/85b0957e-0772-4331-832d-0f13502c6c62" />
<img width="1780" height="697" alt="prediction" src="https://github.com/user-attachments/assets/adbe8d59-5fee-4263-a8bd-22a033e8582e" />
