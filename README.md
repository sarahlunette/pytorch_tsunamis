# PyTorch Tsunami Prediction

A machine learning project for predicting human casualties and property damages caused by tsunamis using PyTorch and other ML techniques.

## Overview

This repository contains a comprehensive analysis and prediction model for tsunami-related damages. The project explores various machine learning approaches to predict both human casualties (deaths and injuries) and property damages (destroyed and damaged houses) based on tsunami characteristics, geographical data, and socio-economic factors.

## Features

- **Data Analysis**: Exploratory data analysis of tsunami datasets
- **Feature Engineering**: Encoding, scaling, and feature selection
- **Multiple ML Models**: ElasticNet, GradientBoostingRegressor, XGBoost, and custom PyTorch neural networks
- **Dimensionality Reduction**: UMAP and t-SNE for visualization
- **Data Augmentation**: Noise injection for improved model training
- **Clustering**: K-means and agglomerative clustering for pattern discovery
- **Interpretability**: SHAP analysis for model explanations

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/pytorch_tsunamis.git
cd pytorch_tsunamis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Data Preparation
The project uses several datasets:
- `data/tsunamis.csv`: Main tsunami event data
- `data/population.csv`: Population data by country
- `data/gdp.csv`: GDP per capita data
- `data/dist2coast.txt.bz2`: Distance to coast data

### Running the Analysis
Open and run the Jupyter notebook `pytorch_tsunamis.ipynb` to:
1. Load and preprocess data
2. Perform exploratory data analysis
3. Train various machine learning models
4. Evaluate model performance
5. Visualize results

### Key Models Implemented

#### Traditional ML Models
- ElasticNet regression
- Gradient Boosting Regressor
- XGBoost Regressor

#### Deep Learning Models
- Custom PyTorch neural network
- TabNet regressor

#### Advanced Techniques
- Clustering-based feature engineering
- Dimensionality reduction
- Data augmentation

## Data Description

The dataset includes information about:
- Tsunami characteristics (magnitude, depth, wave height)
- Geographical data (latitude, longitude, country)
- Temporal data (year, month, day)
- Socio-economic factors (population, GDP per capita)
- Damage metrics (deaths, injuries, houses damaged/destroyed)

## Model Performance

The project evaluates models using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R-squared (R²) score

Results show varying performance across different approaches, with ensemble methods generally performing best.

## Project Structure

```
pytorch_tsunamis/
├── pytorch_tsunamis.ipynb    # Main analysis notebook
├── README.md                 # Project documentation
├── requirements.txt          # Python dependencies
├── data/                     # Dataset files
│   ├── tsunamis.csv
│   ├── population.csv
│   ├── gdp.csv
│   └── dist2coast.txt.bz2
└── git/                      # Git repository (for reference)
```

## Dependencies

- Python 3.7+
- PyTorch
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- xgboost
- pytorch-tabnet
- umap-learn
- shap

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Data sources: NOAA, World Bank, United Nations
- Inspired by real-world disaster prediction challenges
- Part of machine learning interview preparation materials
