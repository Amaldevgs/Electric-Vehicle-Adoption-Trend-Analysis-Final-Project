#  Analyzing and Predicting Electric Vehicle Adoption Trends Using Machine Learning

This project predicts whether a vehicle falls into a specific EV adoption category using various machine learning algorithms.  
It demonstrates the full ML pipeline: data cleaning, class imbalance handling, feature scaling, training multiple models, and visual performance comparison.

---

##  Project Objective

The goal is to help policymakers, researchers, and EV manufacturers understand which factors influence electric vehicle adoption.  
Accurate classification helps guide infrastructure planning, policy formulation, and targeted EV incentives.

---

##  Dataset

**Source**: :https://catalog.data.gov/dataset/electric-vehicle-population-data 

- Vehicle make/model
- Model year
- Base MSRP
- Electric range
- Clean alternative fuel eligibility  
... and more.

**Target Variable**: EV adoption category (binary classification)

---

##  Workflow

Steps implemented:

###  Exploratory Data Analysis (EDA):

- Removed missing values and duplicates
- Explored feature distributions using histograms, box plots
- Visualized trends by model year, make, range
- Identified skewed features and applied log transformation

###  Feature Engineering & Selection:

- Created new feature: **Vehicle Age**
- Transformed price features (e.g., Base MSRP)
- Selected high-impact features based on correlation and business relevance

###   Data Preprocessing:

- Encoded categorical features
- Scaled numerical values using StandardScaler
- Balanced class distribution using **SMOTE**

###  Model Building:

Trained and evaluated 5 classifiers:

- Logistic Regression  
- Random Forest Classifier  
- Support Vector Classifier (SVM)  
- Gradient Boosting Classifier  
- XGBoost Classifier  

###  Model Evaluation:

- Evaluated models using **accuracy, precision, recall, F1-score**
- Analyzed **confusion matrices** for error patterns
- Compared model accuracy using a bar plot
- Plotted **AUC-ROC curves** to visualize class separability

---

##  Key Results

- **Model Year**, **Electric Range**, and **Vehicle Age** were the strongest predictors of EV adoption.
- **XGBoost** and **Random Forest** achieved perfect or near-perfect accuracy.
- SMOTE significantly improved classification for underrepresented classes.
- AUC-ROC plots confirmed strong separation between classes across models.
- Confusion matrix showed minimal false positives and high precision for top models.

---

##  Conclusion

This project demonstrates a strong application of end-to-end machine learning techniques in analyzing electric vehicle trends. The study confirms that electric vehicle adoption is growing, especially in urban hubs like Seattle, with strong presence from brands like Tesla.

In this project, I built and compared multiple machine learning models to predict electric vehicle adoption categories.  
After thorough preprocessing, feature engineering, and model evaluation, **XGBoost and Random Forest** delivered the most accurate and balanced performance.

This project shows how data science can help stakeholders understand and forecast EV market trends.  

