# COVID-19 Case Forecasting with Linear Regression

This project aims to **predict future COVID-19 case counts** using historical data and a **machine learning regression model**. It leverages **time-series analysis techniques** to model and forecast the daily number of new COVID-19 cases in India.

## 📦 Dataset

The dataset is sourced from a convenient global CSV file (`CONVENIENT_global_confirmed_cases.csv`) containing cumulative COVID-19 case counts by country. The project uses **India's data** for demonstration.

## 🚀 Project Workflow

1. **Extract the Dataset**  
   - The dataset is provided in a ZIP file (`covid.zip`) which is extracted in the working directory.

2. **Load and Clean Data**  
   - CSV file is loaded and unnecessary rows/columns are cleaned.
   - Dates are converted to datetime format, and India’s data is isolated.

3. **Feature Engineering**  
   - A new feature, `Day`, is created, representing the number of days since the start of the dataset.

4. **Train-Test Split**  
   - Data is split into training (all data except last 30 days) and testing (last 30 days) sets.

5. **Model Training**  
   - A **Linear Regression model** is trained using the historical case count data.

6. **Predictions and Forecasting**  
   - Model predicts case counts for the last 30 days (test data).
   - Future predictions for the next 30 days are generated.

7. **Visualization**  
   - A line plot visualizes:
     - Actual data  
     - Model’s predictions for test data  
     - Future 30-day forecast  

## 🧰 Libraries Used
- **pandas** for data manipulation  
- **numpy** for numerical operations  
- **scikit-learn** for Linear Regression  
- **matplotlib** for visualization  
- **zipfile** and **os** for file extraction  

## 📈 Results

The project produces a plot comparing:
✅ Actual COVID-19 cases  
✅ Model’s predictions on the last 30 days  
✅ Forecast for the next 30 days  

This allows for a straightforward understanding of how the model performs and its forecast for future COVID-19 trends.

## 📁 How to Run

1. **Clone the repository** (if applicable)  
2. Place your `covid.zip` file in the working directory (e.g., Google Colab or local environment).  
3. Run the Python script / Jupyter notebook to extract, clean, train the model, and visualize the results.

## 🤝 Contribution

Feel free to suggest improvements, additional forecasting techniques (like ARIMA, LSTM), or expand the analysis to other countries!

## 📄 License

This project is for educational purposes and uses publicly available data.

---

**Author:** [Your Name Here]  
**Date:** [Today’s Date]
