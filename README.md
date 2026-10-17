# Data-201-Project-1

**Goal:** Predict whether a patient has heart disease (which is 1) or not(0) using age, cholesterol, maximum heart rate and chest pain type

## Main finding
KNN scored perfectly only because of the duplicate rows: cross-validation chose K = 1, so it memorizes patients that appear in both the training and test sets. I would **deploy LDA**. A missed case of heart disease (a false negative) is the costly error, and LDA caught the most sick patients among the trustworthy models (recall 0.80) with an ROC-AUC of 0.87. A limitation is that 723 rows out of the 1025 are duplicates. 
