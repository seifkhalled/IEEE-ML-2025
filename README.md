# 💎 Diamond Price Prediction

This project uses machine learning regression techniques to predict the price of diamonds based on various physical and categorical features. It includes data cleaning, exploratory data analysis (EDA), feature engineering, outlier handling, model building, evaluation, and final interpretation.

---

## 📊 Dataset

**Source:** The dataset contains information on ~54,000 diamonds, including features such as:

- `carat`: Weight of the diamond
- `cut`: Quality of the cut (Fair, Good, Very Good, Premium, Ideal)
- `color`: Diamond color (from J [worst] to D [best])
- `clarity`: Measure of how clear the diamond is
- `depth`, `table`: Geometric proportions
- `x`, `y`, `z`: Dimensions of the diamond in mm
- `price`: Price in USD (target variable)

---

## 🛠️ Key Steps

### 1. 🔍 Exploratory Data Analysis (EDA)
- Statistical summaries and distribution plots
- Outlier detection using Z-score and IQR methods
- Correlation heatmaps and visual inspection

### 2. 🧹 Data Cleaning & Preprocessing
- Removed outliers (`zscore` and `IQR`)
- Handled skewed distributions
- Scaled numeric features using StandardScaler
- Mapped ordinal categorical features (cut, color, clarity)
- Applied train/test split to avoid data leakage

### 3. 🤖 Modeling
Trained and evaluated the following regression models:

- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **ElasticNet**

### 4. 📈 Evaluation Metrics
Used:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- Adjusted R² Score

📌 **Best Model:** Ridge Regression — it achieved the lowest error while offering regularization stability.

---

## 📌 Conclusion

All models performed similarly due to clean, well-preprocessed data and strong linear relationships between features and price. Ridge Regression was selected as the best due to its slightly better performance and added robustness.

---

## 🧠 Skills Applied

- Data Cleaning & EDA
- Feature Engineering
- Outlier Detection
- Regression Modeling
- Model Evaluation
- Python Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/diamond-price-prediction.git
   cd diamond-price-prediction
