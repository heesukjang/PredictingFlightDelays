# Predicting Flight Delays
###### <i>UC Berkeley MIDS `Machine Learning at Scale` Group Project</i>



The goal of this project was to predict flight departure delays exceeding 15 minutes, 2 hours before takeoff. The detailed business case is available in the [final report](https://github.com/heesukjang/PredictingFlightDelays/blob/main/Final_Report.pdf), with significant potential benefits for airlines and passengers.

In **Phase** I, we focused on project management, setting up the computing environment, planning the data pipeline, and conducting initial exploratory data analysis (EDA) to identify key variables.

In **Phase II**, we joined datasets, performed data cleaning, EDA, and feature engineering. We started with a logistic regression baseline, followed by LASSO regularization, reducing the feature set to 10. This improved logistic regression showed notable performance gains over the baseline.

In **Phase III**, we expanded feature engineering and tested various models, including logistic regression, decision trees, random forests, gradient boosted decision trees, multilayer perceptron, CNNs, and XGBoost. After Bayesian optimization, 5-fold blocking time series cross-validation, and LASSO regularization, XGBoost emerged as the best model with a validation F2 score of 63%, an 18% improvement over the baseline. On the test set, XGBoost achieved an F2 score of 69%, with high precision (90%) but moderate recall (65%). While recall could be improved, the model maintains a good balance, prioritizing the detection of as many actual delays as possible in line with operational goals.

For my **individual contribution**, I led the efforts in EDA, innovating by creating 10 new features for feature engineering, and developed the XGBoost model. I also utilized Bayesian Optimization for hyperparameter tuning, reducing the risks of overfitting and selection bias.
