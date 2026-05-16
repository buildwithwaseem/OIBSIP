# 📊 Task 5: Sales Prediction Using Python

This project focuses on building a predictive analytics model to forecast product sales volumes based on advertising budgets allocated across three major channels: **TV, Radio, and Newspaper**. 

This is a classic **Regression** problem in data science, demonstrating how historical marketing data can be leveraged to optimize corporate advertising spend and maximize Return on Investment (ROI).

---

## 💻 Technical Workflow & Architecture

The project is structured into a clean, end-to-end data science pipeline inside a Jupyter Notebook:

### 1. Exploratory Data Analysis (EDA) & Inspection
Before training the model, I performed a thorough data audit:
* **Shape & Structure:** Checked the total number of records and feature distributions.
* **Data Cleaning:** Verified that there are zero missing/null values in the dataset to prevent any mathematical discrepancy during gradient descent.
* **Statistical Summary:** Analyzed the mean, standard deviation, and quartiles of expenditures to understand the scaling of different advertising mediums.

### 2. Feature Engineering & Selection
* **Independent Variables (X):** `TV`, `Radio`, and `Newspaper` ad budgets.
* **Dependent Variable (y):** Total `Sales` volume.
* **Correlation Mapping:** Used a Seaborn Heatmap to visualize linear relationships. It became immediately clear that different channels have vastly different impacts on conversions.

### 3. Model Training & Data Splitting
* **The Strategy:** Split the dataset into **70% Training data** and **30% Testing data** using Scikit-learn to ensure robust validation and detect any potential overfitting.
* **The Algorithm:** Implemented a **Linear Regression** model to compute the optimal weights (coefficients) and bias (intercept) for the feature matrix equation.

### 4. Comprehensive Performance Metrics
Instead of relying on a single score, the model's error margins were validated using multiple continuous variables evaluation metrics:
* **Mean Absolute Error (MAE):** To measure the average magnitude of errors in predictions.
* **Mean Squared Error (MSE):** To penalize larger errors significantly, ensuring the model doesn't make extreme miscalculations.
* **Root Mean Squared Error (RMSE):** To interpret the error directly in the same unit as the target variable (Sales numbers).

---

## 📈 Real-World Business Insights

After running the predictions and evaluating the coefficients, here are the core analytical takeaways:

1. **TV Dominance:** The model confirms that **TV advertising has the strongest positive correlation** with sales. Every unit increase in the TV budget yields the highest spike in product revenue.
2. **Radio vs. Newspaper:** Radio holds a moderate positive impact, whereas **Newspaper spend has an almost negligible correlation** with sales performance. From a business perspective, shifting budget from Print media to Digital/TV would optimize efficiency.
3. **Linearity:** The low error margins (MAE/RMSE) prove that advertising spends and sales follow a distinctly linear trend, making a simple Linear Regression model highly effective and easily interpretable for stakeholders.

---

## 🛠️ Tooling & Dependency Matrix
- **Language Stack:** Python 3.x
- **Core Libraries:** Pandas (Dataframes), NumPy (Matrix Math), Scikit-learn (Modeling & Evaluation), Seaborn & Matplotlib (Data Visualizations)
- **Execution Environment:** Google Colab / VS Code
