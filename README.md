# 🎧 Podcast Analytics: Predicting Listener Engagement with PySpark

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![PySpark](https://img.shields.io/badge/PySpark-3.3+-orange.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-2.1+-green.svg)
![AWS](https://img.shields.io/badge/AWS-S3-yellow.svg)
![ML](https://img.shields.io/badge/ML-Regression-purple.svg)

## Project Overview

This project uses PySpark and XGBoost to predict podcast listening time based on various podcast attributes. By leveraging distributed computing capabilities, the model can efficiently process large datasets to identify factors that impact listener engagement.

## 📊 Data Features

The model analyzes diverse podcast attributes:

- **Content Features**: Episode length, genre, episode number, sentiment analysis
- **Publication Patterns**: Day and time of publication
- **Social Elements**: Host popularity, guest presence and popularity 
- **Monetization**: Number of advertisements

## 🛠️ Technical Implementation

### Data Processing Pipeline

- **Missing Value Handling**: Genre-specific median imputation for episode length
- **Feature Engineering**:
  - Creation of binary guest presence indicators
  - Extraction of numeric episode numbers from titles
  - Categorical encoding for publication days, times, and sentiment
  - Frequency analysis of podcasts as a popularity measure

### Machine Learning Architecture

- **Framework**: Distributed XGBoost on PySpark
- **Cross-Validation**: 3-fold CV with parallelized execution
- **Hyperparameter Tuning**: Grid search across tree depth, learning rate, and estimator count
- **Evaluation Metric**: Root Mean Square Error (RMSE)

### Cloud Integration

- Seamless AWS S3 integration for scalable data storage

## 📈 Model Performance

The model achieved a validation RMSE of 13.05, demonstrating strong predictive capability for listener engagement.

## 💻 Technologies Used

- **PySpark**: Data processing and ML pipeline orchestration
- **XGBoost**: Gradient boosting implementation
- **AWS S3**: Data storage
- **Databricks**: Notebook development environment

## 🔍 Key Insights

The project allows podcast creators to identify optimal:
- Content characteristics that maximize engagement
- Publishing schedules for maximum audience reach
- Guest and advertising strategies that balance monetization with listener retention

## 🚀 Future Enhancements

- Feature importance analysis to pinpoint strongest engagement drivers
- Time series analysis for seasonal listening patterns
- A/B testing framework for content strategy optimization
- Integration with recommendation systems

## 📚 Skills Demonstrated

- Big data processing with PySpark
- Machine learning with distributed XGBoost
- Feature engineering and data preparation
- AWS cloud integration
- Hyperparameter tuning and model optimization
- Cross-validation techniques
