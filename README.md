# 🚗 Car Price Prediction using Artificial Intelligence  

This project is an **AI-powered car price prediction system** built in **Google Colab**, trained using a **Kaggle car sales dataset**, and deployed with a **Gradio web interface** for easy user interaction.  

It combines **machine learning** and **interactive UI** to estimate car prices based on input details such as manufacturer, model, fuel type, engine size, mileage, and car age.  

---

## 🧠 Project Overview  

This notebook demonstrates a complete machine learning workflow:
1. Downloading and loading real-world car sales data  
2. Cleaning and transforming the dataset  
3. Training a **Random Forest Regressor** model  
4. Evaluating the model using RMSE and R² metrics  
5. Saving the trained model  
6. Building an interactive **Gradio** interface for live predictions  

---

## 📊 Dataset  

**Source:** [Kaggle - Car Sales Info](https://www.kaggle.com/datasets/minahilfatima12328/car-sales-info)  
**File used:** `car_sales_data.csv`  

| Feature | Description |
|----------|--------------|
| Manufacturer | Car manufacturer (e.g., Ford, BMW, Toyota) |
| Model | Model name |
| Engine size | Engine capacity in liters |
| Fuel type | Petrol, Diesel, or Hybrid |
| Year of manufacture | Year the car was made |
| Mileage | Total kilometers driven |
| Price | Car’s market price (target variable) |

---

## ⚙️ Model Pipeline  

A **scikit-learn Pipeline** was used for streamlined preprocessing and model training.  

### 🧩 Steps:
- **Categorical Encoding:** OneHotEncoder  
- **Numerical Scaling:** StandardScaler  
- **Model:** RandomForestRegressor (200 trees, random_state=42)  

### 🧪 Model Performance:
| Metric | Value |
|---------|--------|
| RMSE | 624.90 |
| R² | 0.99856 |

These results indicate a **highly accurate model** with excellent fit on the test data.

---

## 💻 User Interface (Gradio)

A simple yet elegant **Gradio interface** was created to allow users to test the model interactively.  
Users can select a car, enter its features, and instantly receive a predicted price.

### 🖥️ UI Features:
- Dropdown menus for car and fuel type  
- Numeric inputs for engine size, mileage, and age  
- “Predict Price” button  
- Styled output box with color-coded design  

### 🎨 Custom Styling:
The interface includes custom CSS for a modern, user-friendly look (blue headers, red buttons, and soft-themed input boxes).

---

## 🚀 How to Run  

### ▶️ In Google Colab:
1. Upload the `.ipynb` file to Colab.  
2. Run all cells to train and save the model.  
3. The Gradio app will launch with a public link for interaction.
