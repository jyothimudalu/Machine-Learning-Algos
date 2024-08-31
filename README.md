**[Predictive Modeling for Heart Disease: An Evaluation of Decision
Tree, XGBoost, and Random Forest Classifiers]{.underline}**

**[Project Overview]{.underline}**

This project involves analyzing and predicting heart disease using a
dataset of various patient features. The aim is to build and evaluate
several machine learning models to classify patients as either having
heart disease (target = 1) or not (target = 0). The dataset includes 303
entries with 14 features, such as age, blood pressure, cholesterol
levels, and exerciseinduced angina.

**[Key Metrics]{.underline}**

Accuracy: The proportion of correctly predicted classifications out of
all predictions made.

Confusion Matrix: A table used to describe the performance of
classification models by showing the true positives, true negatives,
false positives, and false negatives.

Classification Report: Provides precision, recall, and F1score for each
class, giving a detailed breakdown of the model\'s performance.

**[Dataset]{.underline}**

[Link for dataset](https://www.kaggle.com/datasets/arezaei81/heartcsv)

The dataset used is \`heart.csv\`, which consists of 303 entries and 14
columns, including:

-   age: Age of the patient

-   sex: Gender of the patient (1 = male, 0 = female)

-   cp: Chest pain type

-   trestbps: Resting blood pressure

-   chol: Serum cholesterol level

-   fbs: Fasting blood sugar

-   restecg: Resting electrocardiographic results

-   thalach: Maximum heart rate achieved

-   exang: Exercise induced angina

-   oldpeak: Depression induced by exercise relative to rest

-   slope: Slope of the peak exercise ST segment

-   ca: Number of major vessels colored by fluoroscopy

-   thal: Thalassemia

-   target: Presence or absence of heart disease (1 = presence, 0 =
    absence)

**[Methodology]{.underline}**

1\. Data Cleaning and Preprocessing:

Removed duplicate entries.

Identified and handled outliers for columns \`trestbps\`, \`chol\`, and
\`thalach\` using the Interquartile Range (IQR) method.

Dropped unnecessary columns and converted categorical variables to dummy
variables.

2\. Exploratory Data Analysis (EDA):

Visualized distributions of numerical features using histograms.

Analyzed correlations among features using a heatmap.

3\. Model Building and Evaluation:

Split the data into training and testing sets (80% training, 20%
testing).

Built and evaluated three classification models:

Decision Tree Classifier

XGBoost Classifier

Random Forest Classifier

Used accuracy, confusion matrix, and classification reports to assess
model performance.

4\. Hyperparameter Tuning:

Performed hyperparameter tuning for the Random Forest Classifier using
RandomizedSearchCV to find the best model parameters.

**[Results]{.underline}**

[Decision Tree Classifier:]{.underline}

Accuracy: 83.61%

![](./image1.png){width="6.268055555555556in"
height="2.779861111111111in"}

[XGBoost Classifier:]{.underline}

Accuracy: 85.25%

![](./image2.png){width="6.268055555555556in"
height="3.2979166666666666in"}

[Random Forest Classifier (with Hyperparameter Tuning):]{.underline}

Accuracy: 85.25%

![](./image3.png){width="5.948746719160105in"
height="2.527435476815398in"}

The Random Forest and XGBoost classifiers achieved the highest accuracy
of 85.25%, showing better performance compared to the Decision Tree
classifier.
