# 🌱 Greenhouse Gas Emissions Prediction Project

## Overview
This project analyzes and predicts greenhouse gas (GHG) emissions from various U.S. industries and commodities using machine learning regression models. The analysis is based on supply chain emission data from 2010-2016.

## Dataset
**Source**: [U.S. EPA Supply Chain Greenhouse Gas Emission Factors](https://catalog.data.gov/dataset/supply-chain-greenhouse-gas-emission-factors-for-us-industries-and-commodities)

The dataset contains:
- **Target Variable**: Supply Chain Emission Factors with Margins
- **Features**: Commodity codes, substance types, data quality metrics, and emission factors
- **Time Period**: 2010-2016
- **Coverage**: Various U.S. industries and commodities

## Project Structure

### 📁 Files
- `GHG_Emissions_Prediction.ipynb` - Main Jupyter notebook with complete analysis
- `requirements.txt` - Python dependencies
- `README.md` - Project documentation

### 📊 Analysis Steps
1. **Data Loading**: Multi-year Excel file processing
2. **Exploratory Data Analysis**: Statistical analysis and visualization
3. **Data Preprocessing**: Cleaning, feature engineering, and encoding
4. **Model Training**: Linear Regression and Random Forest models
5. **Model Evaluation**: Performance metrics and visualization
6. **Hyperparameter Tuning**: Grid search optimization
7. **Model Selection**: Comparative analysis and best model selection

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required packages (see requirements.txt)

### Installation
1. Clone or download the project files
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Place your Excel data file in the project directory:
   - File name: `SupplyChainEmissionFactorsforUSIndustriesCommodities.xlsx`
   - Should contain sheets named by year (2010, 2011, ..., 2016)

### Running the Analysis
1. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `GHG_Emissions_Prediction.ipynb`
3. Run all cells to execute the complete analysis

## 📈 Key Features

### Machine Learning Models
- **Linear Regression**: Interpretable baseline model
- **Random Forest**: Advanced ensemble method with hyperparameter tuning

### Feature Engineering
- Data quality composite scores
- Margin ratio calculations
- Categorical encoding (Label encoding and One-hot encoding)
- Feature importance analysis

### Evaluation Metrics
- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)
- **R² Score** (Coefficient of Determination)
- **Cross-validation** performance

### Visualizations
- Target variable distributions
- Correlation heatmaps
- Feature importance plots
- Model performance comparisons
- Actual vs. predicted scatter plots
- Residual analysis

## 🎯 Results

The project identifies the best-performing model based on:
- Highest test R² score
- Lowest test RMSE
- Minimal overfitting
- Consistent cross-validation performance

Key insights include:
- Most important predictive features
- Industry/commodity emission patterns
- Data quality impact on predictions

## 📁 Output Files

After running the complete analysis, the following files are generated:
- `best_ghg_emissions_model_*.joblib` - Best trained model
- `best_ghg_emissions_model_*.pkl` - Model backup
- `ghg_emissions_model_metadata.pkl` - Model metadata and feature information
- `ghg_emissions_scaler.joblib` - Feature scaler (if needed)

## 🔧 Customization

### Adding New Models
To add additional models, modify the models dictionary in Step 4:
```python
models = {
    'Linear Regression': LinearRegression(),
    'Random Forest': RandomForestRegressor(random_state=42),
    'Your New Model': YourModelClass()
}
