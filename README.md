# An Ensemble Model to Predict Obesity Levels of Latin American Countries

## Assignment: DA5030 - Practicum in Data Analytics  

## Description

This project develops and evaluates ensemble machine learning models to classify individuals into seven obesity categories based on lifestyle and physical condition characteristics. The study focuses on populations from Latin American countries (Mexico, Peru, and Colombia) and compares the performance of logistic regression, decision trees, and neural networks using homogeneous and heterogeneous ensemble techniques.

## Getting Started

### Dependencies

* R (>= 4.0.0)
* Required R packages: caret, caretEnsemble, nnet, rpart, rpart.plot, C50, VGAM, glmnet, dplyr, ggplot2
* RStudio (recommended)

### Installing

* Clone or download the repository containing `obesity_prediction_ensemble.Rmd`
* Ensure all required packages are installed (installation code included in the document)
* The dataset is automatically downloaded from the hosted URL during execution

### Executing program

* Open `obesity_prediction_ensemble.Rmd` in RStudio
* Run all code chunks sequentially or knit to HTML
* Results and visualizations will be generated inline
* Expected runtime is ~15-20 minutes depending on system performance
* The analysis will display progress messages for major sections

## Key Results

* **Best performing model**: Logistic Regression Homogeneous Ensemble with 10-fold CV (Accuracy: 96.69%, Macro F1: 0.9669)
* **Dataset**: 2,111 observations across 7 obesity categories with 18 features, including engineered BMI
* **Model comparison**: Ensemble methods significantly outperformed individual models
* **Feature importance**: BMI, weight, age, and family history were identified as primary predictors
* **Validation**: Cross-validated results demonstrate robust generalization capability

## Authors

Natalia Pretel Pretel  
pretel.n@northeastern.edu  
Master's in Bioinformatics, Northeastern University

## Version History

* 1.0
    * Complete ensemble analysis with bagging, boosting, and stacking
    * Comprehensive model comparison and evaluation
    * Feature engineering and hyperparameter tuning
    * Cross-validation and performance metrics

## Models Implemented

* Multinomial Logistic Regression (with LASSO feature selection)
* Decision Trees (rpart and C5.0 with boosting)
* Neural Networks (nnet with hyperparameter tuning)
* Homogeneous Ensembles (bagging for each model type)
* Heterogeneous Ensemble (majority voting)
* Stacked Ensemble (meta-learner approach)

## Performance Comparison

| Model Type | Accuracy | Macro F1-Score |
|------------|----------|----------------|
| Logistic Regression Ensemble (CV) | 96.69% | 0.9669 |
| C5.0 Boosted Decision Tree | 98.58% | 0.9858 |
| Neural Network Ensemble | 96.38% | 0.9637 |
| Stacked Heterogeneous Ensemble | 95.20% | 0.9520 |

## Data Source

**Dataset**: Estimation of Obesity Levels Based on Eating Habits and Physical Condition  
**Repository**: UCI Machine Learning Repository  
**URL**: https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition  
**Citation**: Palechor, F.M. & de la Hoz Manotas, A. (2019). Dataset for estimation of obesity levels based on eating habits and physical condition. UCI Machine Learning Repository.

The dataset contains 2,111 observations with 17 attributes including demographic information, eating habits, physical condition, and lifestyle factors from individuals in Mexico, Peru, and Colombia.

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
* Various R package maintainers (caret, nnet, rpart, etc.)

## Citation

Palechor, F.M. & de la Hoz Manotas, A. (2019). Dataset for estimation of obesity levels based on eating habits and physical condition. UCI Machine Learning Repository.
