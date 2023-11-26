#  Project Report: Predicting Customer Churn

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)<br>

## What It Does: 
The goal of this project is to build a predictive model to identify customers at risk of churning, i.e., discontinuing their subscription or service. Churn prediction is crucial for businesses to retain customers and maximize revenue. In this report, I'll provide insights into the data exploration, preprocessing steps, feature engineering, and the evaluation of the predictive models.<br>


1️⃣ Data Collection <br>
2️⃣ Data Preprocessing <br>
3️⃣ Exploratory Data Analysis <br>
4️⃣ Dataset Balancing & Scaling <br>
5️⃣ Machine Learning Models Training & Evaluation

## Prerequisites:
I would highly recommend that before the hack night, you should have some kind of toolchain and development environment already installed and ready. If you have no idea where to start with this, try a combination like: <br>


1️⃣ `Python`<br>
2️⃣ `scikit-learn` / `sklearn`<br>
3️⃣ `Pandas`<br>
4️⃣ `NumPy`<br>
5️⃣ `Swaborn`<br>
6️⃣ An environment to work in - something like `Jupyter` or `colab`<br>


For Linux people, your package manager should be able to handle all of this. If it somehow can't, see if you can at least install Python and pip and then use pip to install the above packages.

## Dataset:
The dataset used for this project contains information about customers, including demographic details, services subscribed, and whether they churned or not. Key points about the dataset:

- **Features:** Various customer attributes such as gender, contract type, monthly charges, and others.
- **Target Variable:** 'Churn' indicating whether a customer has churned or not.

> You can collect raw dataset from [here](dataset.csv).

### Data Preprocessing

1️⃣ `Label Encoding:` Categorical variables were encoded using the Label Encoder to convert them into numerical form, making them suitable for modeling.

2️⃣ `Handling Missing Values:` Missing values in the 'TotalCharges' column were replaced with the mean of the column.

EDA was performed to gain insights into the dataset:

1️⃣ `Churn Distribution:` Visualized the distribution of churn to understand the class balance.

2️⃣ `Correlation Matrix:` Explored correlations between variables using a heatmap. This helped identify potential relationships and multicollinearity.

## Model Building

Two models were trained and evaluated:

1️⃣ **`Random Forest Classifier:`**
   - Used 100 trees in the forest.
   - Achieved an accuracy of 79.34%, precision of 65.29%, recall of 46.91%, and F1 score of 54.60%.
2️⃣ **`Logistic Regression:`**
   - Achieved an accuracy of 81.61%, precision of 67.81%, recall of 58.17%, and F1 score of 62.62%.

## Model Evaluation

Both models were evaluated using standard classification metrics:

**`Accuracy:`** Percentage of correctly classified instances.<br>
**`Precision:`** Proportion of true positives among instances predicted as positive.<br>
**`Recall (Sensitivity):`** Proportion of true positives among actual positives.<br>
**`F1 Score:`** Harmonic mean of precision and recall.<br>

### Challenges Faced

**`Imbalanced Classes:`** The dataset showed some imbalance in the distribution of churn and non-churn instances, which can impact model performance. This was addressed by using appropriate metrics and potentially exploring techniques like oversampling or undersampling.

## Conclusion

In this project, I successfully built and evaluated models for predicting customer churn. The Logistic Regression demonstrated reasonable performance, but there is room for improvement, particularly in handling imbalanced classes and further optimizing the chosen models. The insights gained from EDA and the created features contribute to a better understanding of the factors influencing customer churn. Continued refinement and tuning of models may enhance predictive accuracy and provide more actionable insights for business decision-making.
#
