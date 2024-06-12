# Car Repurchase Prediction using Classification Models

This repository contains the implementation and analysis of a car repurchase prediction project conducted by Shaqran Bin Saleh for the 36106 - Machine Learning Algorithms and Applications course at the University of Technology Sydney.

## Project Details
- **Student Name:** Shaqran Bin Saleh
- **Student ID:** 25010238
- **Date:** 26-04-2024
- **Course:** 36106 - Machine Learning Algorithms and Applications
- **Program:** Master of Data Science and Innovation

## Table of Contents
1. [Business Understanding](#business-understanding)
2. [Data Understanding](#data-understanding)
3. [Data Preparation](#data-preparation)
4. [Modeling](#modeling)
5. [Evaluation](#evaluation)
    - [Results and Analysis](#results-and-analysis)
    - [Business Impact and Benefits](#business-impact-and-benefits)
    - [Data Privacy and Ethical Concerns](#data-privacy-and-ethical-concerns)
6. [Conclusion](#conclusion)
7. [References](#references)

## Business Understanding
### Business Use Cases
The project aims to leverage machine learning algorithms to predict car repurchase behavior. Key business use cases include:
1. **Customer Retention:** Identifying customers with high repurchase probability to tailor campaigns and maximize retention.
2. **Inventory Optimization:** Forecasting vehicle features and models likely to be popular to optimize inventory.
3. **Strategic Campaigns:** Efficiently allocating marketing resources to campaigns with the highest ROI.

### Key Objectives
- Evaluate classification models for predicting customer repurchase behavior.
- Optimize model performance through hyperparameter tuning.
- Identify key factors influencing repurchase decisions.

## Data Understanding
The dataset consists of various vehicle characteristics and customer interaction metrics. Key features include:
- **Demographics:** Age band, gender.
- **Vehicle Characteristics:** Car model, car segment, age of vehicle.
- **Service Metrics:** Number of scheduled/unscheduled services, total services, amount paid for services, time since last service, annual mileage.
- **Dealership Interactions:** Number of dealers visited, number of services at purchase dealer.

### Data Exploration
- Visualizations: Histograms, box plots, count plots, and pie charts were used to explore distributions and relationships with the target variable.

## Data Preparation
Steps taken include:
- **Data Loading:** Loaded from CSV into a pandas DataFrame.
- **Data Cleaning:** Addressed missing values and removed duplicates.
- **Feature Engineering:** Applied one-hot encoding to categorical features.
- **Data Splitting:** Divided data into training, validation, and test sets.
- **Feature Scaling:** Applied scaling to numerical features to ensure uniformity.

## Modeling
Five machine learning algorithms were selected:
1. **K-Nearest Neighbors (KNN)**
2. **Support Vector Machine (SVC)**
3. **Decision Tree Classifier**
4. **Random Forest Classifier**
5. **Extra Trees Classifier**

### Hyperparameter Tuning
Hyperparameters were optimized using grid search and random search techniques for each model.

## Evaluation
### Results and Analysis
Performance of models was evaluated using accuracy, F1 score, and precision. Key observations include:
- **Extra Trees Classifier:** High accuracy but low F1 score and precision due to potential class imbalance.
- **Random Forest and Decision Tree Classifiers:** Perfect scores indicating overfitting.
- **Support Vector Classifier (SVC):** Best performance with high generalization capability.
- **KNN:** Performance varied with hyperparameter settings, highlighting the importance of tuning.

### Business Impact and Benefits
The SVC model offers significant business advantages by:
- Enhancing customer retention through targeted engagement strategies.
- Optimizing inventory management with better demand forecasting.
- Improving marketing efficiency and ROI.

### Data Privacy and Ethical Concerns
Addressing privacy and ethical concerns involves:
- Anonymizing data and securing customer information.
- Ensuring transparency and informed consent.
- Avoiding biases and promoting inclusiveness in data handling and model development.

## Conclusion
The project identified the SVC model as the most effective for predicting car repurchases, providing valuable insights for customer retention, inventory management, and marketing strategies. Future work includes model deployment and ensuring data privacy and ethical practices.

## References
- Soofi, A., & Awan, A. (2017). Classification Techniques in Machine Learning: Applications and Issues. *Journal of Basic & Applied Sciences, 13*, 459–465. [doi:10.6000/1927-5129.2017.13.76](https://doi.org/10.6000/1927-5129.2017.13.76)
- Cheriyan, S., Ibrahim, S., Mohanan, S., & Treesa, S. (2018). Intelligent Sales Prediction Using Machine Learning Techniques. *IEEE Xplore*. [doi:10.1109/iCCECOME.2018.8659115](https://doi.org/10.1109/iCCECOME.2018.8659115)
- Gurnani, M., Korke, Y., Shah, P., Udmale, S., Sambhe, V., & Bhirud, S. (2017). Forecasting of sales by using fusion of machine learning techniques. *2017 International Conference on Data Management, Analytics and Innovation (ICDMAI)*. [doi:10.1109/icdmai.2017.8073492](https://doi.org/10.1109/icdmai.2017.8073492)
- Amari, S., & Wu, S. (1999). Improving support vector machine classifiers by modifying kernel functions. *Neural Networks, 12*(6), 783–789. [doi:10.1016/s0893-6080(99)00032-5](https://doi.org/10.1016/s0893-6080(99)00032-5)
