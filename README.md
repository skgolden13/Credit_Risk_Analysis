# Credit Risk Analysis

## Project Overview

This project uses Python to develop and evaluate machine learning models to predict credit risk. Credit risk data is from quarter 1 of 2019. The following methods were used:
- Oversampling using RandomOverSampler
- Oversampling using SMOTE
- Undersampling using ClusterCentroids
- Combination using SMOTEENN
- Bias reduction using BalancedRandomForestClassifier
- Bias reduction using EasyEnsembleClassifier

Performance for these models will be evaluated using balanced accuracy scores, confusion matrices, and imbalanced classification reports.

## Results

### RandomOverSampler

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/OS_BAS.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/OS_CM.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/OS_ICR.PNG"><br/>
</p>

<p align="center">
	Figure 1: RandomOverSampler Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report. <br/>
</p>

The balanced accuracy score is 64.1%.
The high risk precision is 1% with a recall score of 60%.
The low risk precision is 100% with a recall score of 68%.

### SMOTE

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/SMOTE_BAS.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/SMOTE_CM.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/SMOTE_ICR.PNG"><br/>
</p>

<p align="center">
	Figure 2: SMOTE Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report. <br/>
</p>

The balanced accuracy score is 63.7%.
The high risk precision is 1% with a recall score of 60%.
The low risk precision is 100% with a recall score of 68%.

### ClusterCentroids

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/CC_BAS.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/CC_CM.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/CC_ICR.PNG"><br/>
</p>

<p align="center">
	Figure 3: ClusterCentroids Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report. <br/>
</p>

The balanced accuracy score is 51.2%.
The high risk precision is 1% with a recall score of 59%.
The low risk precision is 100% with a recall score of 44%.

### SMOTEENN

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/SMOTEENN_BAS.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/SMOTEENN_CM.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/SMOTEENN_ICR.PNG"><br/>
</p>

<p align="center">
	Figure 4: SMOTEENN Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report. <br/>
</p>

The balanced accuracy score is 62.4%.
The high risk precision is 1% with a recall score of 70%.
The low risk precision is 100% with a recall score of 55%.

### BalancedRandomForestClassifier

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/BRFC_BAS.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/BRFC_CM.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/BRFC_ICR.PNG"><br/>
</p>

<p align="center">
	Figure 5: BalancedRandomForestClassifier Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report. <br/>
</p>

The balanced accuracy score is 78.8%.
The high risk precision is 4% with a recall score of 67%.
The low risk precision is 100% with a recall score of 91%.

### EasyEnsembleClassifier

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/EEC_BAS.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/EEC_CM.PNG"><br/>
</p>

<p align="center">
	<img width="450" src="https://github.com/skgolden13/Credit_Risk_Analysis/blob/main/Images/EEC_ICR.PNG"><br/>
</p>

<p align="center">
	Figure 6: EasyEnsembleClassifier Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report. <br/>
</p>

The balanced accuracy score is 92.5%.
The high risk precision is 7% with a recall score of 91%.
The low risk precision is 100% with a recall score of 94%.

## Summary

All models tested showed low precision in determining high credit risk, with no models showing a precision score above 10%. The EasyEnsembleClassifier shows an inprovement on the recall score for high credit risk at 91%. The precision of 7% for the EasyEnsembleClassifier shows that the model still predicts a large number of low credit risks as high. I would not recommend that any of these models are used to predict credit risk.