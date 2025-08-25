# 🚗 Car Price Prediction using Machine Learning  

## 📌 Overview  
This project develops a **Machine Learning model** to predict the **selling price of used cars** based on multiple factors such as purchase year, kilometers driven, fuel type, seller type, transmission type, and ownership history.  

The aim is to provide an accurate estimation of car resale values, which can assist both buyers and sellers in making data-driven decisions.  

---

## ⚙️ Features Implemented  
✔️ Data cleaning & preprocessing  
✔️ Handling categorical features with encoding  
✔️ Training models: **Linear Regression** & **Lasso Regression**  
✔️ Evaluation with **R² Score, MAE, MSE, RMSE**  
✔️ Visualization: **Actual vs Predicted** plots  
✔️ Console-based **predictive system** where users enter car details and receive predicted price  

---

## 📊 Dataset Features  
| Feature         | Description |
|-----------------|-------------|
| Year            | Year of purchase |
| Present_Price   | Current ex-showroom price (in lakhs) |
| Kms_Driven      | Kilometers driven by the car |
| Fuel_Type       | Petrol / Diesel / CNG |
| Seller_Type     | Dealer / Individual |
| Transmission    | Manual / Automatic |
| Owner           | Number of previous owners |
| Selling_Price   | Target variable – price to be predicted |

---

## 🛠️ Data Preprocessing  

### 🔹 Handling Categorical Data  
The dataset contains categorical features such as **Fuel_Type**, **Seller_Type**, and **Transmission**.  
These were converted into **numerical values** using `replace()` encoding:  

- **Fuel_Type**:  
  - Petrol → 0  
  - Diesel → 1  
  - CNG → 2  

- **Seller_Type**:  
  - Dealer → 0  
  - Individual → 1  

- **Transmission**:  
  - Manual → 0  
  - Automatic → 1  

### 🔹 Removing Unnecessary Columns  
- **Car_Name** was removed as it doesn’t provide predictive value.  
- The remaining features were used to train the model.  

---

## 🧠 Model Training  

### 🔹 Linear Regression  
- **R² Score (Train):** 0.8799  
- **R² Score (Test):** 0.8365  

---

### 🔹 Lasso Regression  
- **R² Score (Train):** 0.8427  
- **R² Score (Test):** ~0.83  

---
## 🎯 Predictive System (Console Based)  

We built a simple **console-based predictive system** where the user enters car details and the model predicts the resale price.  

### 🔹 Input Example  

```text
📅 Enter the Year of purchase: 2014
💰 Enter the Present Price (in lakhs): 5.59
📍 Enter the Kms Driven: 27000
⛽ Enter Fuel Type (Petrol/Diesel/CNG): petrol
🧑 Enter Seller Type (Dealer/Individual): dealer
⚙️ Enter Transmission Type (Manual/Automatic): manual
👤 Enter number of previous owners (0/1/2/3): 0
```
### 🔹Result

✅ Predicted Selling Price of the car is: ₹ 3.83 lakhs

---



