# MSDS422_Final Group 3 Project: Obesity Risk Prediction: A Machine Learning Approach

**Authors**: Jinghan Feng, Yahui Qian, Zixuan Zhang, Chenyi Zhao

**Dataset**: Access from [Kaggle - Obesity Prediction Dataset](https://www.kaggle.com/datasets/ruchikakumbhar/obesity-prediction/code)

## Table of Contents

- [Executive Summary](#executive-summary)
- [Problem Statement](#problem-statement)
- [Research Objectives](#research-objectives)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Deployment Strategy](#deployment-strategy)
- [Limitations](#limitations)
- [Future Improvements](#future-improvements)
- [License](#license)
  
## Executive Summary  
Obesity is a growing public health concern in Latin America, significantly impacting individual health and straining healthcare systems. This research investigates the complex factors contributing to obesity in Mexico, Colombia, and Peru, employing a multidisciplinary approach that combines dataset analysis, statistical modeling, and machine learning techniques.  

The research highlights key findings such as the role of socioeconomic, dietary, and behavioral factors and explores advanced computational tools for estimating obesity levels and predicting associated risks. This study leverages a dataset containing 17 attributes and 2,111 records, categorizing individuals into seven distinct obesity levels. The dataset encompasses diverse features such as demographic data, physical measurements, and lifestyle behaviors, including caloric intake, physical activity frequency, and alcohol consumption.  

By analyzing this dataset, the project aims to explore the complex interplay of these factors, identify patterns and trends, and develop predictive models to estimate obesity levels. Advanced statistical techniques, such as handling class imbalances with SMOTE and applying machine learning algorithms like Random Forest and Gradient Boosting, will be utilized to enhance prediction accuracy.  

This research provides a foundation for data-driven public health interventions, offering actionable insights for mitigating obesity through targeted, culturally sensitive strategies tailored to the unique demographic characteristics of these regions.  

## Problem Statement  
Obesity has emerged as a growing epidemic in Latin America, driven by a convergence of unhealthy eating habits, sedentary lifestyles, and socioeconomic disparities. Despite its widespread impact on health systems and populations, current interventions often fail to address the multifaceted nature of obesity or utilize data effectively to inform public health strategies. There is a pressing need for robust predictive models and analytical frameworks that can uncover underlying trends, identify at-risk populations, and guide targeted, evidence-based interventions.  

## Research Objectives  
- To explore and analyze the relationships between demographic factors, dietary habits, physical activity levels, and obesity levels in individuals from Mexico, Peru, and Colombia.  
- To provide actionable insights that can guide policymakers and public health practitioners in designing effective, culturally appropriate interventions to combat obesity in Latin America.  
- To identify key predictors of obesity levels, such as high-calorie food consumption, physical activity frequency, and technology usage, and assess their relative importance.  
- To develop and evaluate predictive models using machine learning algorithms such as Random Forest, Gradient Boosting, and Neural Networks for accurately estimating obesity levels.  

## Features
This project includes:
- **Exploratory Data Analysis (EDA):** Feature distributions, correlations, and key insights.
- **Feature Engineering:** Handling missing data, encoding categorical variables, and scaling numerical features.
- **Machine Learning Models:** Comparison of multiple models:
  - Random Forest
  - Gradient Boosting
  - Support Vector Machines (SVM)
  - Neural Network (MLP)
  - Deep Neural Network (DNN)
- **Evaluation Metrics:** Accuracy, Precision-Recall, ROC-AUC.

## Dataset
- **Source:** The dataset includes **numerical and categorical** features related to diet, activity, and BMI.
- **Target Variable:** Obesity levels classified into seven categories.

## Installation
To set up and run this project, install the required dependencies:

```bash
git clone https://github.com/yourusername/obesity-risk-prediction.git
cd obesity-risk-prediction
pip install -r requirements.txt
```

## Usage
Run the Jupyter Notebook for analysis:

```bash
jupyter notebook Obesity_Prediction.ipynb
```

## Methodology
- **Data Preprocessing:** Handling missing values, encoding categorical variables, and feature selection.
- **Model Training & Evaluation:** Models trained with **GridSearchCV** and cross-validation.
- **Hyperparameter Tuning:** Optimized parameters for each model to maximize accuracy.

## Results
| Model | Accuracy (%) |
|--------|------------|
| MLP | **97.64%** |
| SVM | 96.69% |
| Gradient Boosting | 96.22% |
| Random Forest | 94% |
| Deep Neural Network | 93.38% |

- **Key Takeaways:**
  - **MLP performed best** with the highest accuracy.
  - **SVM and Gradient Boosting** also showed strong results.
  - **Deep learning models require larger datasets** to generalize better.

## Deployment Strategy
- The model is designed for **on-premises deployment** to ensure **data privacy**.
- The machine learning pipeline is **automated** for continuous updates.
- Model integration with **healthcare applications** is recommended.

## Limitations
- The dataset lacks **socioeconomic and genetic factors**, which can impact obesity risk.
- Limited generalizability since the data primarily comes from Latin American countries.
- Some models (DNN) were prone to **overfitting due to small dataset size**.

## Future Improvements
- **Expand dataset** to include more diverse populations.
- **Improve feature engineering** by adding socioeconomic and behavioral data.
- **Optimize model selection** using deep learning advancements.

## License
This project is licensed under the [MIT License](LICENSE) - see the file for details.
