# Linear Regression Model: Predict Used Car Prices


## 📌 Project Overview
This project implements a **Linear Regression Model** to predict the selling price of used cars based on multiple features such as **Year, Mileage, Make, Model, City, and State**. The dataset, sourced from Kaggle, contains approximately **850,000 used car listings**, with comprehensive attributes influencing price estimation.

### 🎯 Objectives
- Develop a **Linear Regression Model** to predict used car prices.
- Identify significant predictor variables affecting car prices.
- Evaluate model performance using metrics like **Mean Squared Error (MSE)** and **R-squared**.
- Address potential **outliers** and **influential observations**.
- Interpret model coefficients to provide insights into price fluctuations.

---

## 📂 Project Files
- **📄 Project Report:** `Project Report.docx`
- **📊 Presentation:** `736 Presentation.pptx`
- **📓 Jupyter Notebook:** `Group 1 Final Project Linear Regression.ipynb`

---

## 📊 Dataset Information
- **Source:** Kaggle ([Used Car Price Predictions Dataset](https://www.kaggle.com/datasets/harikrishnareddyb/used-car-price-predictions/data))
- **Size:** ~850,000 used car listings
- **Key Features:**
  - `Price`: Target variable (selling price of the used car)
  - `Year`: Manufacturing year
  - `Mileage`: Distance traveled by the car
  - `Make`: Manufacturer brand
  - `Model`: Car model
  - `City` & `State`: Location details
  - `VIN`: Vehicle Identification Number (dropped as a unique identifier)

---

## 🛠️ Project Workflow
1. **Import Libraries:** Used `pandas`, `sklearn`, `matplotlib`, `seaborn`, and `category_encoders`.
2. **Data Preprocessing:**
   - Dropped `VIN` as it does not contribute to prediction.
   - Encoded categorical variables using `category_encoders`.
   - Standardized numerical variables using `sklearn.preprocessing`.
   - Handled outliers using **Interquartile Range (IQR) method**.
3. **Feature Selection:**
   - Selected best feature combination: `['Year', 'Mileage', 'Make', 'Model']`
   - **Average R-squared:** `0.7398`
4. **Model Development:**
   - **Algorithm Used:** Linear Regression
   - Split dataset into **80% training** and **20% testing** using `train_test_split()`.
   - Trained the regression model on the dataset.
5. **Evaluation Metrics:**
   - **Mean Squared Error (MSE):** `46205175.65`
   - **R-squared:** `0.749`
6. **Visualization:**
   - Created scatter plots of **actual vs. predicted values**.

---

## 📈 Results & Analysis
- **R-squared:** `0.749` (Indicates that ~74.9% of the variance in car prices is explained by the model).
- **MSE:** `46205175.65` (Indicates the model's prediction error is relatively low).
- **Key Predictor Variables:** `Year, Mileage, Make, Model`
- **Impact of Features on Price:**
  - **Newer cars** tend to have **higher prices**.
  - **Higher mileage** negatively impacts price.
  - Certain **brands & models** hold higher resale value.

---

## 🏆 Conclusion
- The **Linear Regression Model** effectively predicts used car prices with **74.9% accuracy**.
- **Key attributes** like `Year`, `Mileage`, `Make`, and `Model` significantly impact pricing.
- **Outlier handling & feature selection** improved model performance.
- The model provides valuable insights for **buyers, sellers, and dealerships**.

### 🚀 Future Enhancements
- Implement **Polynomial Regression** for capturing non-linear relationships.
- Compare performance with **other ML models** (e.g., Decision Trees, Random Forest).
- Deploy the model as a **web application** for real-time price estimation.

---

## 📚 References
1. [Anaconda Software Distribution](https://www.anaconda.com)
2. [Scikit-Learn Documentation](https://scikit-learn.org/stable/)
3. [Used Car Price Predictions Dataset - Kaggle](https://www.kaggle.com/datasets/harikrishnareddyb/used-car-price-predictions/data)
4. [Matplotlib - Data Visualization](https://matplotlib.org/)
5. [Project Jupyter](https://jupyter.org/)
6. [Python Software Foundation](https://www.python.org/)
7. [Pandas Library](https://pandas.pydata.org/)
8. [Seaborn - Statistical Data Visualization](https://seaborn.pydata.org/)
9. [Category Encoders Library](https://github.com/scikit-learn-contrib/category_encoders)

---

## Team Members
- Taravat Ashabi
- Mukesh Mohan
- Shahin Rajabi
- Tanmaya Rodda

---

## ⚙️ How to Run the Code
### 1️⃣ Prerequisite
- Install Python 3.8+ and Jupyter Notebook
- Required Python Libraries:
  ```bash
  pip install pandas scikit-learn matplotlib seaborn category_encoders


This `README.md` is structured for clarity, covering:
- **Project Overview**
- **Dataset Details**
- **Workflow**
- **Results**
- **Conclusion & Future Work**
- **How to Run the Code**
- **References & Contributors**

Let me know if you need any modifications! 🚀
