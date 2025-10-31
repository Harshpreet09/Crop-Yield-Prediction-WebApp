# 🌾 Crop Yield Prediction (Streamlit + Scikit-learn)

A simple **machine learning web app** built with **Streamlit** to predict **crop yield (Q/acre)** using environmental and agricultural features like temperature, rainfall, fertilizer, and soil nutrients (N, P, K).

---

## 1️⃣ Data Setup
- Load dataset from `crop yield data sheet.xlsx`
- Clean invalid/missing values
- Split into train–test sets (80/20)

---

## 2️⃣ Streamlit UI
- Sidebar shows dataset info  
- Tabs:
  - 📊 EDA – visualize rainfall, fertilizer, and yield trends  
  - 🤖 Model Training – Decision Tree & Random Forest  
  - 📈 Results – compare predictions, view feature importance  

---

## 3️⃣ Model Training
- Uses **GridSearchCV** for hyperparameter tuning  
- Displays best parameters and R² score  
- Supports:
  - `DecisionTreeRegressor`
  - `RandomForestRegressor`

---

## 4️⃣ Results & Metrics
- Shows actual vs predicted yield  
- Key metrics: **R²**, **MSE**, **MAE**  
- Feature importance visualization

---

## 💡 Tech Stack
Streamlit · Python · Pandas · NumPy · Seaborn · Matplotlib · Scikit-learn

---

## ⚙️ Run Locally
```bash
git clone https://github.com/<your-username>/Crop_Yield_Prediction.git
cd Crop_Yield_Prediction
pip install -r requirements.txt
streamlit run crop_yield_app.py
