# Disease-Analytics-with-GBM
___
## Description:
This project uses a multi-class **Gradient-Boosted Machine (GBM) supervised classification** model (implemented from scratch) to diagnostically predict a patient’s medical condition by using a combination of demographic, behavioral, and physiological health indicators. 

* chronic_diseases.zip and chronic_diseases.csv are the zipped and unzipped CSV "Healthcare Risk Factors" dataset found on Kaggle, which contain nearly 30,000 anonymized patient records.
* HealthcareAnalytics.ipynb implements the multi-class GBM model to **identify which health metric features most strongly predict diabetes, hypertension, asthma, arthritis, cancer, and obesity** in medical patients prior to their hospital stay. This work:
  * Builds a statistically robust model using only the top features that carry the greatest predictive power using Recursive Feature Elimination (RFE).
  * Accurately distinguishes between these medical condition categories uses a **One vs. Rest (OvR)** boosting strategy.
  * Trains the GBM model using **stratified $k$-fold** cross-validation ($k$ = 5) since some diseases occur less frequently than others and maintaining the relative frequencies of medical conditions in each fold supports more accurate model training.
  * Evaluates model performance using **ROC curves**, classification indicators (**precision, recall, F1 scores, accuracy**), and **confusion matrices** as quantitative performance markers and visualizations.
