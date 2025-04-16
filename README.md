# Hotel Price Prediction Using Web Scraping and Machine Learning

When planning a vacation, accommodation takes up the majority of the budget. This project aims to help travelers make smarter budget decisions by building a predictive model to estimate hotel prices based on location, room type, discounts, and other features.

## Problem Statement

Manually tracking hotel prices is tedious. By scraping hotel listings from [Booking.com](https://www.booking.com), I aim to collect data and build a predictive model that accurately forecasts hotel prices.

## Key Features

- **Web Scraping**: Extracted hotel data using Selenium for ~763 hotels in Dubai
- **Data Cleaning**: Cleaned & transformed messy data (e.g., location strings, prices, distances)
- **Exploratory Data Analysis**: Identified trends & pricing patterns based on features
- **Machine Learning**: Built and compared Linear Regression and Random Forest Regressor models
- **Model Deployment**: Trained model saved using `joblib` and tested with new inputs
- **Final Model**: Random Forest Regressor with RMSE ≈ 31.05 and R² Score ≈ 0.98

## Technologies Used

- Python, Pandas, NumPy
- Selenium (Web Scraping)
- Scikit-Learn (ML Modeling)
- Matplotlib & Seaborn (EDA)
- Joblib (Model Saving)

## Files and Folders

| File/Folder                | Description |
|----------------------------|-------------|
| `hotel_cleaned.csv`        | Cleaned dataset used for modeling |
| `model_columns.pkl`        | Folder with saved model and encoded columns |
| `hotel_price_model.ipynb`  | Full pipeline: scraping → EDA → modeling |
| `predict.ipynb`            | Load model and test with new sample data |
| `hotel_price_predictor.pkl`| Trained Random Forest Regressor model

## How to Use

1. **Download the Files**  
   Ensure the following files are in the same directory:  
   - `hotel_price_predictor.pkl`  
   - `model_columns.pkl`  
   - `predict.ipynb`
2. **Edit & Run `predict.ipynb`**  
   - Open `predict.ipynb` in Jupyter Notebook  
   - Enter your input values in the provided template  
   - Run the cells to get the **predicted hotel price**

No need to retrain the model, just plug in your data and get predictions instantly!
