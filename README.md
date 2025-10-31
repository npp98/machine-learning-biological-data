# An Ensemble Model to Predict Obesity Levels of Latin American Countries

[![Latest Release](https://img.shields.io/github/v/release/npp98/machine-learning-biological-data)](https://github.com/npp98/machine-learning-biological-data/releases/latest)

**Assignment:** DA5030 - Practicum in Data Analytics

## 📊 View Analysis Report

**[📥 Download Complete HTML Report from Latest Release](https://github.com/npp98/machine-learning-biological-data/releases/latest)**

The interactive HTML report includes all visualizations, model comparisons, confusion matrices, and performance metrics.

## Description

This project develops and evaluates ensemble machine learning models to classify individuals into seven obesity categories based on lifestyle and physical condition characteristics. The study focuses on populations from Latin American countries (Mexico, Peru, and Colombia) and compares the performance of logistic regression, decision trees, and neural networks using homogeneous and heterogeneous ensemble techniques.

## Key Results

- **Best Overall Performance:** C5.0 Boosted Decision Tree (98.58% accuracy, 0.9858 macro F1)
- **Most Robust Model:** Logistic Regression Homogeneous Ensemble with 10-fold CV (96.69% accuracy, 0.9669 macro F1)
- **Dataset:** 2,111 observations across 7 obesity categories with 18 features
- **Top Predictors:** BMI, weight, age, and family history of overweight
- **Validation:** Cross-validated results demonstrate strong generalization capability

## Getting Started

### Dependencies

* R (>= 4.0.0)
* RStudio (recommended)
* Required R packages: caret, caretEnsemble, nnet, rpart, rpart.plot, C50, VGAM, glmnet, dplyr, ggplot2

### Installing

* Clone or download this repository
* All required packages installation code is included in the document
* Dataset is automatically downloaded from UCI ML Repository during execution

### Executing Program

* Open `obesity_prediction_ensemble.Rmd` in RStudio
* Run all code chunks sequentially or knit to HTML
* Results and visualizations will be generated inline
* Expected runtime: ~15-20 minutes depending on system performance
* Progress messages displayed for major sections

## Models Implemented

1. **Multinomial Logistic Regression** (with LASSO feature selection)
2. **Decision Trees** (rpart and C5.0 with boosting)
3. **Neural Networks** (nnet with hyperparameter tuning)
4. **Homogeneous Ensembles** (bagging for each model type)
5. **Heterogeneous Ensemble** (majority voting)
6. **Stacked Ensemble** (meta-learner approach)

## Performance Comparison

| Model Type | Accuracy | Macro F1-Score |
|-----------|----------|----------------|
| Logistic Regression Ensemble (CV) | 96.69% | 0.9669 |
| C5.0 Boosted Decision Tree | 98.58% | 0.9858 |
| Neural Network Ensemble | 96.38% | 0.9637 |
| Stacked Heterogeneous Ensemble | 95.20% | 0.9520 |

## Repository Contents

* `obesity_prediction_ensemble.Rmd` - R Markdown source code for complete analysis
* `Obesity_Prediction_Ensemble.html` - Rendered HTML report (download from [Releases](https://github.com/npp98/machine-learning-biological-data/releases/latest))
* Complete ensemble modeling workflow with feature engineering

## Analysis Workflow

1. **Data Preprocessing**: Feature engineering (BMI calculation), encoding, normalization
2. **Exploratory Analysis**: Distribution analysis and feature relationships
3. **Individual Models**: Baseline performance of logistic regression, decision trees, and neural networks
4. **Homogeneous Ensembles**: Bagging techniques for each model type
5. **Heterogeneous Ensembles**: Majority voting and stacked meta-learner approaches
6. **Model Evaluation**: Cross-validation, confusion matrices, and performance metrics
7. **Feature Importance**: Analysis of key predictors across models

## Data Source

**Dataset:** Estimation of Obesity Levels Based on Eating Habits and Physical Condition  
**Repository:** UCI Machine Learning Repository  
**URL:** https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition

The dataset contains 2,111 observations with 17 attributes including demographic information, eating habits, physical condition, and lifestyle factors from individuals in Mexico, Peru, and Colombia.

**Citation:** Palechor, F.M. & de la Hoz Manotas, A. (2019). Dataset for estimation of obesity levels based on eating habits and physical condition. UCI Machine Learning Repository.

## Author

**Natalia Pretel Pretel**  
Master's Student in Bioinformatics  
Northeastern University  
📧 pretel.n@northeastern.edu

## Version History

* **v1.0.0** (Latest)
    * Complete ensemble analysis with bagging, boosting, and stacking
    * Comprehensive model comparison and evaluation
    * Feature engineering and hyperparameter tuning
    * Cross-validation and performance metrics

## Help

* All visualizations and model outputs are generated inline within the document
* Confusion matrices and performance metrics are automatically calculated
* Feature importance plots and model comparisons are included in results
* For troubleshooting package installations, refer to the package loading section

## Acknowledgments

* UCI Machine Learning Repository for the obesity dataset
* Kabongo & Luzolo (2020) for baseline comparison methodology
* Palechor & de la Hoz Manotas for dataset creation and curation
* Northeastern University DA5030 course framework
* R package maintainers (caret, nnet, rpart, caretEnsemble, etc.)
