The given data contains unknown and masked columns, which are analyzed to identify variables and datatypes. 
Basic metrics are calculated, and non-graphical and visual analysis techniques are applied. 
The data has numerous missing values in several columns, which are handled by dropping columns with missingness exceeding 80%.
These columns do not contribute significantly to the analysis. For the remaining missing values that are mild to moderate, multivariate KNN imputation is used to remove them.

The data is divided into train_set, validation_set, and test_set to prevent data leakage. Outliers are addressed by replacing extreme values.
Feature scaling, feature selection, and dimension reduction techniques, such as L1 Regression, are applied.
Feature creation is also attempted as a trial and test method. 
Finally, an optimized algorithm is selected, prioritizing the positive class based on precision, recall, true positive rate, and false positive rate. 
Ensemble techniques are utilized for the best model selection. ROC AUC curve and ROC AUC metrics are used for evaluation on the required data.
Ultimately, predictions are made on the X_test dataset and saved in the Predictions.csv file.
