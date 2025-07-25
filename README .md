# 🚗 Car Price Predictor

<img src="https://github.com/CVRishi156/car-price-predictor/blob/master/demo.png" alt="App Demo" width="600">

---

# 🎯 Aim

This project aims to predict the price of a used car based on parameters such as the company name, model, year of purchase, fuel type, and kilometers driven. It helps users estimate the resale value of their vehicle using a trained machine learning model.

<img src="https://github.com/CVRishi156/car-price-predictor/blob/master/predict.png" alt="Prediction Result" width="600">

---

## ⚙️ How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/CVRishi156/car-price-predictor.git
   cd car-price-predictor
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/Scripts/activate   # Git Bash
   # or
   venv\Scripts\activate        # CMD
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

   Some important packages:
   - flask  
   - flask-cors  
   - numpy  
   - pandas  
   - scikit-learn

4. Run the Flask application:
   ```bash
   python application.py
   ```

5. Open your browser and visit:
   ```
   http://127.0.0.1:5000/
   ```

---

# 📖 Description

## 🔍 What This Project Does

1. Takes the following input:
   - Company name
   - Car model
   - Year of purchase
   - Fuel type
   - Kilometers driven

2. Uses a trained linear regression model to predict the resale price of the car.

3. Returns the predicted price on the screen.

Example result:

<img src="https://github.com/CVRishi156/car-price-predictor/blob/master/predict.png" alt="Result Example" width="600">

---

## ⚙️ How This Project Works

1. The original dataset was scraped from [Quikr](https://www.quikr.com) and cleaned.

2. Exploratory Data Analysis (EDA) was performed to identify key features.

3. A `Linear Regression` model was trained using `scikit-learn`, with:
   - OneHotEncoding for categorical variables
   - ColumnTransformer pipeline

4. The model achieved an R² score of **0.92**, and was saved as a `.pkl` file using `pickle`.

5. The prediction pipeline was integrated into a Flask web app, where users can interactively get price estimates.

---

## 📁 Files Included

- `application.py` – Flask backend app
- `LinearRegressionModel.pkl` – Trained ML model
- `Cleaned_Car_data.csv` – Cleaned dataset
- `templates/index.html` – Input form frontend
- `static/css/style.css` – Basic styling
- `requirements.txt` – Dependency list
- `.gitignore` – Ignored files (e.g., venv)

---

## 👨‍💻 Author

**CV Rishi**  
🔗 [GitHub](https://github.com/CVRishi156)  
🔗 [LinkedIn](https://linkedin.com/in/c-v-rishi-76613127a)

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
