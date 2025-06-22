# 🌍 Greenhouse Gas (GHG) Emissions Prediction

This project uses machine learning to predict greenhouse gas emissions based on industrial activity and substance data. It involves data preprocessing, exploratory data analysis, and model evaluation using both linear and ensemble methods.

---

## 📊 Dataset

- **Source**: Provided Excel dataset (`af60b10b8dad38110304.xlsx`)
- **Sheet Used**: `2016_Summary_Industry`
- **Features**:
  - Industry
  - Gas Type
  - Emission Quantity
  - Others...
- **Target Variable**: `Emissions (kt CO2e)`

---

## 🧠 ML Models Used

| Model             | Purpose                      |
|------------------|------------------------------|
| Linear Regression | Baseline prediction model    |
| Random Forest     | Non-linear ensemble model    |

---

## 📈 Evaluation Metrics

- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- R² Score

Results are visualized with scatter plots of actual vs. predicted emissions.

---

## 🛠️ Technologies Used

- Python 3.x
- Jupyter Notebook
- pandas
- scikit-learn
- matplotlib
- seaborn
- openpyxl (for Excel support)

---

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/ghg-emission-prediction.git
cd ghg-emission-prediction
```

2. Install required libraries:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter:
```bash
jupyter notebook
```

---

## 📂 File Structure

```
GHG_Emissions_Project/
│
├── af60b10b8dad38110304.xlsx     # Dataset
├── GHG_Emissions_Prediction.ipynb # Main notebook
├── README.md                     # Project readme
├── requirements.txt              # Python dependencies
```

---

## 📌 How to Use

- Open the notebook in Jupyter
- Run cells one by one
- Modify parameters or try new models
- Analyze evaluation output

---

## 🚀 Future Improvements

- Use more years and combine multiple sheets
- Add support for more ML algorithms (XGBoost, SVR)
- Deploy the model using Streamlit or Flask

---

## ⭐️ Show your support!

If you like this project, drop a ⭐️ on the repo or contribute!