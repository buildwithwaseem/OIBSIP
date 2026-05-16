## 🚗 Task 3: Car Price Prediction with Machine Learning
For this task, I built a machine learning regression model to predict the price of used cars based on multiple features like brand goodwill, mileage, fuel type, engine capacity, and horsepower.

### What I did:
* **Feature Engineering & Preprocessing:** Handled categorical variables using One-Hot Encoding so that the algorithm could process non-numerical columns like 'Fuel Type' or 'Transmission'.
* **Model Selection:** Implemented a **Random Forest Regressor** to handle the non-linear relationships between a car's features and its market valuation.
* **Evaluation:** Scored the model using the **$R^2$ Score** and Mean Absolute Error (MAE) to ensure the predictions align closely with actual market prices.

### Key Insights:
* **The Price Drivers:** Engine horsepower and the brand's market segment have the highest weight when it comes to determining a car's resale value.
* **The Mileage Drop:** As expected, higher mileage shows a strong negative correlation with the price, causing a predictable drop in valuation.

### Tech Stack:
- Python (Pandas, NumPy, Scikit-learn, Seaborn)
- Google Colab



