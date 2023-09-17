<img src="https://github.com/josefroslan/heartdisease/blob/main/img/background.jpg" alt="Background">

# Heart Disease Prediction

- [Heart Disease Prediction](#heart-disease-prediction)
  - [Introduction](#introduction)
  - [Installation](#installation)
  - [Data Collection](#data-collection)
  - [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Data Visualizations](#data-visualizations)
  - [Predictive Modeling](#predictive-modeling)
  - [Conclusion](#conclusion)
  - [Next Steps](#next-steps)
  - [License](#license)

## Introduction
Heart disease is a prevalent and life-threatening condition that affects millions of people worldwide. Timely detection and accurate prediction of heart disease are crucial for effective medical intervention and patient care. In this project, I delve into the realm of predictive analytics to develop a model that can assess the likelihood of individuals having heart disease based on various health attributes.

### Project Objective
The primary goal of this project is twofold:

- **Identify Key Predictive Features:** I aim to discern the most critical factors associated with the presence of heart disease. By analyzing a comprehensive dataset containing a range of health-related parameters, I seek to pinpoint which attributes are most likely to be present in individuals with heart disease.

- **Evaluate Predictive Models:** I employ predictive modeling techniques to construct and evaluate machine learning models. These models will assist me in predicting the likelihood of an individual having heart disease, allowing for early detection and intervention.

### Dataset Source
To achieve these objectives, I utilize the [UCI Machine Learning Repository - Heart Disease Data](https://archive.ics.uci.edu/dataset/45/heart+disease) as the primary source of data. This dataset offers valuable insights into various health indicators and serves as the foundation for my analysis.

### Importance of Early Detection
Early detection of heart disease is crucial, as it enables healthcare professionals to administer appropriate treatments and lifestyle recommendations promptly. By leveraging data-driven insights and advanced machine learning, I aim to contribute to the ongoing efforts to enhance cardiovascular health assessment.

Throughout this project, I conduct data cleaning, exploratory data analysis, and predictive modeling to extract meaningful patterns and create models that can aid in heart disease prediction. My findings provide valuable insights that can assist healthcare practitioners and researchers in their mission to combat heart disease effectively.

Join me on this data-driven journey as I explore the factors contributing to heart disease and evaluate the performance of predictive models designed to make a positive impact on healthcare outcomes.

## Installation
1) **Clone the Repository:** Clone this project repository to your local machine:
```
git clone https://github.com/josefroslan/heartdisease.git
```

2) **Set Up Python Environment:**
- Create and activate a virtual environment (recommended):
```
python -m venv venv
```

- Activate the virtual environment:
- **On Windows:**
```
venv\Scripts\activate
```
- **On macOS and Linux:**
```
source venv/bin/activate
```

3) **Install Dependencies:** Install required packages:
```
pip install -r requirements.txt
```

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

## Next Steps
While our current analysis has provided valuable insights into heart disease prediction, there are several avenues for further exploration and improvement in this project. Here are some potential next steps:
- **Advanced Machine Learning Algorithms**
Consider exploring more advanced machine learning algorithms. While Logistic Regression and Decision Trees have shown promise, other models such as Random Forests, Support Vector Machines, or Gradient Boosting might offer improved predictive performance. Experiment with these algorithms to assess their effectiveness in our context.

- **Feature Engineering**
Feature engineering plays a crucial role in enhancing model performance. Explore the possibility of creating new features or transforming existing ones to capture more nuanced information about individuals' health. Domain knowledge can be valuable in this process.

- **Hyperparameter Tuning**
Optimize the hyperparameters of our models to fine-tune their performance. Techniques like grid search or random search can help identify the best combination of hyperparameters for each algorithm, potentially boosting accuracy and other metrics.

- **Cross-Validation**
Implement robust cross-validation techniques to ensure our models' generalizability. K-fold cross-validation, for instance, can provide a more reliable estimate of performance on unseen data and reduce overfitting.

- **Ensemble Learning**
Explore ensemble learning methods, such as model stacking or bagging, to combine predictions from multiple models. Ensemble techniques often lead to improved predictive accuracy and robustness.

- **Interpretability**
Consider using techniques to enhance the interpretability of our models. Tools like SHAP (SHapley Additive exPlanations) or LIME (Local Interpretable Model-Agnostic Explanations) can help us understand why our models make specific predictions, which is essential in healthcare settings.

- **Data Augmentation**
If feasible, collect additional data sources related to individuals' health and lifestyle. More comprehensive datasets can provide a richer context for our models and potentially lead to better predictions.

- **Deployment**
Think about how to deploy our predictive model in real-world healthcare settings. This might involve building a user-friendly interface for healthcare professionals or integrating the model into electronic health record systems.

- **Ethical Considerations**
As we move forward, it's essential to consider ethical implications. Ensure that data privacy and fairness are maintained throughout the project, and conduct bias assessments to address potential disparities in model predictions.

- **Collaboration**
Collaborate with healthcare professionals and domain experts to gain further insights and refine the project's objectives. Their expertise can guide us in making more informed decisions and improving model interpretability.

These next steps outline a path for the continued development and enhancement of our Heart Disease Prediction project. By incorporating advanced techniques, fine-tuning models, and addressing ethical considerations, we can create a robust and impactful tool for early detection and intervention in individuals at risk of heart disease.

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
- This project is licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** License.

- You are free to:
  - Share: Copy and redistribute the material in any medium or format.
  - Adapt: Remix, transform, and build upon the material for any purpose, even commercially.

- Under the following terms:
  - Attribution: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
  - For more details, view the full license text [here](https://creativecommons.org/licenses/by/4.0/legalcode).

