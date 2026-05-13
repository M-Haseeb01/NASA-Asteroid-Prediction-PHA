# NASA-Asteroid-Prediction-PHA

To build and evaluate a machine learning binary classification model that 
predicts whether an asteroid is potentially hazardous (PHA = 1) or not (PHA = 0), based 
on its physical and orbital characteristics as recorded in the NASA Asteroid Dataset.

This project successfully demonstrates the application of machine learning to the 
planetary defense problem of identifying Potentially Hazardous Asteroids. The key 
findings are: 
1. Random Forest is the best model, achieving near-perfect recall (0.9855) and 
F1-score (0.9887) on the held-out test set, making it the recommended classifier 
for this task. 
2. MOID and absolute magnitude (H) are the most discriminating features, 
consistent with the physical definitions used by NASA for PHA classification. 
3. Class imbalance requires careful metric selection. Accuracy alone is 
misleading; recall and AUC are the appropriate measures for hazard detection. 
4. Logistic Regression provides a strong, interpretable baseline with 
near-perfect AUC (0.9992), suitable when model transparency is prioritized. 
5. SVM and KNN underperform primarily due to training on a 50k-row subsample; 
they remain viable candidates with full-dataset training or threshold optimization.
