# Heart Disease Prediction

- [Heart Disease Prediction](#heart-disease-prediction)
  - [Problem Statement](#problem-statement)
  - [Data Collection](#data-collection)
  - [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Data Visualizations](#data-visualizations)
  - [Predictive Modeling](#predictive-modeling)
  - [Conclusion](#conclusion)
  - [License](#license)

This project aims to predict the likelihood of individuals having heart disease and identify the most important features associated with heart disease. We will explore a dataset containing various health attributes and use predictive modeling techniques to accomplish this goal.

## Problem Statement

1. What features are most likely present in individuals with heart disease?
2. Which predictive model is the most effective in predicting the likelihood of individuals having heart disease?

## Data Collection

- Source of dataset: [UCI Machine Learning Repository - Heart Disease Data](https://archive.ics.uci.edu/dataset/45/heart+disease)
- Source of the publication: [International application of a new probability algorithm for the diagnosis of coronary artery disease](https://www.semanticscholar.org/paper/International-application-of-a-new-probability-for-Detrano-J%C3%A1nosi/a7d714f8f87bfc41351eb5ae1e5472f0ebbe0574)

## Data Cleaning and Preprocessing

We have preprocessed the dataset to ensure it's ready for analysis:

- Renamed columns with meaningful names.
- Handled missing data.
- Converted categorical variables to numerical format.

## Exploratory Data Analysis

We conducted exploratory data analysis (EDA) to gain insights into the dataset. Some key findings include:

- **Age:** Older individuals have a higher likelihood of having heart disease.
- **Sex:** Male individuals have a higher likelihood of having heart disease compared to females.
- **Chest Pain:** Individuals with asymptomatic chest pain have a higher likelihood of having heart disease.
- **Resting Blood Pressure:** Even though median resting blood pressure is similar for individual with and without heart disease, the maximum and minimum resting blood pressure tend to be significantly higher in individuals with heart disease.
- **Resting ECG:** LVH and abnormal ST-T waves is more prevalent among individuals with heart disease compared to without heart disease.
- **Maximum Heart Rate:** Individuals with heart disease tend to have lower maximum heart rates.
- **Exercise-induced Angina:** Individuals with exercise-induced angina tend to have a higher prevalence of heart disease compared to those without exercise-induced angina.
- **Exercise-induced ST Depression:** There is a significant difference in exercise-induced ST depression between individuals with and without heart disease.
- **Slope of Peak Exercise ST Segment:** Relatively high number of individuals with heart disease have a flat slope, while fewer have an upsloping or downsloping slope.
- **Number of Major Vessels Blockage:** Individuals with more colored vessels tend to have a higher prevalence of heart disease.
- **Thallium Stress Test:** Individuals with a reversible defect in the thallium stress test tend to have a higher prevalence of heart disease compared to those with fixed defect or normal results.

## Data Visualizations
<img src="https://github.com/josefroslan/heartdisease/blob/main/img/agevshd.png" alt="Age Distribution vs Heart Disease" width="30%"> <img src="https://github.com/josefroslan/heartdisease/blob/main/img/sexvshd.png" alt="Sex Distribution vs Heart Disease" width="30%"><img src="https://github.com/josefroslan/heartdisease/blob/main/img/bpvshd.png" alt="Resting Blood Pressure Distribution vs Heart Disease" width="30%"><img src="https://github.com/josefroslan/heartdisease/blob/main/img/cholvshd.png" alt="Cholesterol Distribution vs Heart Disease" width="30%"><img src="https://github.com/josefroslan/heartdisease/blob/main/img/hrvshd.png" alt="Maximum Heart Rate Distribution vs Heart Disease" width="30%"><img src="https://github.com/josefroslan/heartdisease/blob/main/img/corrheatmap.png" alt="Correlation Heatmap" width="35%">

## Predictive Modeling

### Model Comparison

- We evaluated multiple predictive models for heart disease prediction, including Logistic Regression and Decision Tree Classifier. 
- Here's a comparison of their performance:

| Model                | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | 88.33%   | 0.89      | 0.83   | 0.85     |
| Decision Tree        | 83.33%   | 0.86      | 0.79   | 0.83     |

## Conclusion

- In conclusion, our analysis indicates that age, gender, chest pain type, and several other factors are significant predictors of heart disease. The Logistic Regression model performed slightly better than the Decision Tree Classifier in terms of accuracy and precision.
- This predictive model can be valuable in healthcare settings for early detection and intervention in individuals at risk of heart disease. Further research could explore the integration of additional data sources and more advanced machine learning techniques to improve predictive accuracy.
- Thank you for exploring our Heart Disease Prediction project.

## Acknowledgments

We would like to acknowledge the following resources, libraries, tools, and sources that were instrumental in the success of this project:

### Data Sources:
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/45/heart+disease) for providing the heart disease dataset.
- [Semanticscholar.org](https://www.semanticscholar.org/paper/International-application-of-a-new-probability-for-Detrano-J%C3%A1nosi/a7d714f8f87bfc41351eb5ae1e5472f0ebbe0574) for valuable insights from the publication "International application of a new probability algorithm for the diagnosis of coronary artery disease."

### Libraries and Tools:
- [Python](https://www.python.org/) for the programming language used in data analysis and modeling.
- [Pandas](https://pandas.pydata.org/) for data manipulation and analysis.
- [NumPy](https://numpy.org/) for numerical computations.
- [Matplotlib](https://matplotlib.org/) and [Seaborn](https://seaborn.pydata.org/) for data visualization.
- [Scikit-Learn](https://scikit-learn.org/) for the machine learning tools and algorithms used in this project.
- [Jupyter Notebook](https://jupyter.org/) for interactive data analysis and documentation.

### Inspirational Papers:
- [International application of a new probability algorithm for the diagnosis of coronary artery disease](https://pubmed.ncbi.nlm.nih.gov/2756873/) for providing the foundation for our analysis and modeling.

These resources, libraries, and tools have played a crucial role in our project's development, and we are grateful for their contributions.

## License
- This dataset is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.
- This allows for the sharing and adaptation of the datasets for any purpose, provided that the appropriate credit is given.

