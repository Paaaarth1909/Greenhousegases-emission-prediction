# Replit.md - Greenhouse Gas Emissions Prediction Project

## Overview

This is a machine learning project focused on analyzing and predicting greenhouse gas (GHG) emissions from various U.S. industries and commodities. The project uses data from the U.S. EPA Supply Chain Greenhouse Gas Emission Factors dataset covering the period 2010-2016. The analysis employs regression models including Linear Regression and Random Forest to predict supply chain emission factors.

## System Architecture

The project follows a typical data science workflow architecture:
- **Data Layer**: Excel-based dataset with multi-year sheets
- **Processing Layer**: Jupyter Notebook environment for data analysis
- **Model Layer**: Scikit-learn based machine learning models
- **Visualization Layer**: Matplotlib/Seaborn for data visualization

The architecture is designed for exploratory data analysis and prototyping rather than production deployment.

## Key Components

### Data Processing
- **Input**: Multi-sheet Excel file (`SupplyChainEmissionFactorsforUSIndustriesCommodities.xlsx`)
- **Format**: Yearly sheets (2010-2016) containing emission factors data
- **Target**: Supply Chain Emission Factors with Margins
- **Features**: Commodity codes, substance types, data quality metrics, emission factors

### Machine Learning Pipeline
- **Preprocessing**: Data cleaning, feature engineering, and encoding
- **Models**: 
  - Linear Regression (baseline model)
  - Random Forest (ensemble model)
- **Optimization**: Grid search hyperparameter tuning
- **Evaluation**: Performance metrics and comparative analysis

### Analysis Components
1. Exploratory Data Analysis (EDA)
2. Statistical analysis and visualization
3. Model training and evaluation
4. Hyperparameter optimization
5. Model comparison and selection

## Data Flow

1. **Data Ingestion**: Load multi-year Excel sheets into pandas DataFrames
2. **Data Exploration**: Statistical analysis and visualization of emission patterns
3. **Data Preprocessing**: Clean data, handle missing values, encode categorical variables
4. **Feature Engineering**: Create relevant features for model training
5. **Model Training**: Train Linear Regression and Random Forest models
6. **Model Evaluation**: Compare model performance using metrics
7. **Hyperparameter Tuning**: Optimize model parameters using grid search
8. **Model Selection**: Choose best performing model based on evaluation metrics

## External Dependencies

### Core Libraries
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **scikit-learn**: Machine learning algorithms
- **matplotlib**: Basic plotting and visualization
- **seaborn**: Statistical data visualization
- **jupyter**: Interactive notebook environment

### Data Source
- U.S. EPA Supply Chain Greenhouse Gas Emission Factors dataset
- Format: Excel file with multiple yearly sheets
- Time coverage: 2010-2016

## Deployment Strategy

This project is designed for research and analysis purposes:
- **Environment**: Jupyter Notebook for interactive analysis
- **Execution**: Local development environment
- **Dependencies**: Managed through requirements.txt
- **Data**: Manual placement of Excel file in project directory

The current architecture supports:
- Interactive data exploration
- Model experimentation
- Results visualization
- Reproducible analysis

## Recent Changes

✓ Created comprehensive Jupyter notebook with complete ML workflow
✓ Set up data loading from multi-year Excel sheets (2010-2016)
✓ Implemented EDA, feature engineering, and model training
✓ Built Linear Regression and Random Forest models with hyperparameter tuning
✓ Added model evaluation, comparison, and selection framework
✓ Included model persistence and metadata saving functionality

## Changelog

```
Changelog:
- June 27, 2025. Initial setup and complete ML workflow implementation
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```