# Houses Price Prediction of Karachi (2024–25)

**This project is an end-to-end machine learning pipeline to predict house prices in Karachi using real estate data scraped from [Zameen.com](https://www.zameen.com/) for the years 2024 and 2025.**

## Objective
The goal of this project is to:
- Understand the key factors influencing house prices in Karachi
- Practice real-world web scraping and feature engineering
- Build and evaluate multiple regression models to predict prices accurately

## Dataset
- **Source:** Zameen.com
- **Scope:** Houses listed in **Karachi** during **2024 and 2025**
- **Scraped Attributes:** Title, Price, Area (sqft), Bedrooms, Bathrooms, Location (Society, Town), etc.

## Project Pipeline

### 1. Web Scraping
- Tool: `BeautifulSoup` + `Requests`
- Targeted Karachi houses from Zameen.com (2024–2025)
- Cleaned and structured the scraped HTML into a usable CSV format

### 2. Data Cleaning & Preprocessing
- Handled missing values and inconsistent formatting
- Converted prices and areas to numeric types
- Extracted structured location components (Society, Town)

### 3. Exploratory Data Analysis (EDA)
- Visualized price distributions
- Identified high-price and low-price areas
- Analyzed relationships between price, area, location, and bedrooms

### 4. Feature Engineering
To improve model performance, the following new features were created:
- `price_per_sqft` = Price / Area  
- `avg_price_per_society` = Average price per society  
- `area_per_bedroom` = Area / Bedrooms  
- `price_per_bedroom` = Price / Bedrooms  

These helped the models better capture pricing patterns and increased accuracy.

### 5. Model Building
- **Linear Regression**

### 6. Evaluation Metrics
- R² Score
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)

## Results & Insights
- **Linear Regression** achieved the best R² score and lowest RMSE
- Societies like DHA, Clifton had the highest average prices
- Price was strongly influenced by **location**, **area**, and **engineered features**

## Tech Stack
- Python
- Pandas
- NumPy
- BeautifulSoup
- Matplotlib & Seaborn
- Scikit-learn

**Author**
- Danish Karim
- danisharain253@gmail.com

