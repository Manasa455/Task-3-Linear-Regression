# **Task-3: Linear Regression**

### **Dataset**

* **File:** `Housing.csv`
* **Location:** Local upload
* **Target Variable:** `price` (House price in INR)

### 🛠️ **Tools & Libraries**

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

### ✅ **Steps Performed**

1. **Loaded the dataset**
   * Checked dataset shape, used `head()` and `info()` for basic understanding.
2. **Preprocessed the data**
   * Handled **categorical variables** (`mainroad`, `guestroom`, `basement`, etc.) using **One-Hot Encoding** (`pd.get_dummies()`).
   * Split data into **features (X)** and **target (y)**.
3. **Split into Train-Test sets**
   * Used **80% for training**, **20% for testing** with `train_test_split()`.
4. **Built the Linear Regression Model**
   * Used **`LinearRegression`** from Scikit-learn.
   * Trained model using `.fit()` on training data.
5. **Evaluated Model Performance**
   * Calculated:
     * **Mean Absolute Error (MAE)**
     * **Mean Squared Error (MSE)**
     * **R-squared (R² Score)**
   * Metrics helped measure accuracy and error in price predictions.
6. **Visualized Actual vs Predicted Prices**
   * Created a **scatter plot** with Actual prices vs Predicted prices.
   * Added **red line** to represent perfect prediction line.
7. **Interpreted Model Coefficients**
   * Displayed how each feature (like `area`, `bedrooms`, `stories`, etc.) influences the house price.
   * Positive/negative values of coefficients indicate **positive/negative impact** on price.

### **Output**

* **Evaluation Metrics:**
  * MAE, MSE, R² for model quality check.
* **Regression Plot:**
  * Clear visualization of model fit.
* **Feature Impact:**
  * Table showing how much each feature affects the target price.
* **Conclusion:**
  * The model captures general price trends but has some error margin (visible from MAE/MSE).
  * Useful for predicting approximate house prices based on features.
