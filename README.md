# Predicting Flight Delays
###### <i>UC Berkeley MIDS `Machine Learning at Scale` Group Project</i>



The goal of this project was to predict flight departure delays exceeding 15 minutes, 2 hours before takeoff. The detailed business case is available in the [final report](https://github.com/heesukjang/PredictingFlightDelays/blob/main/Final_Report.pdf), with significant potential benefits for airlines and passengers.

In **Phase** I, we established project management, set up the computing environment, planned the data pipeline, and conducted initial EDA to identify key variables.

In **Phase II**, we merged 60M+ flight and weather records, performed data cleaning, deeper EDA, and feature engineering. Starting with a logistic regression baseline, we applied LASSO regularization to reduce features to 10, significantly boosting model performance.

In **Phase III**, we expanded feature engineering and tested various models, including logistic regression, decision trees, random forests, gradient boosted decision trees, multilayer perceptron, CNNs, and XGBoost. After Bayesian optimization, 5-fold blocking time series cross-validation, and LASSO regularization, XGBoost emerged as the best model with a validation F2 score of 63%, an 18% improvement over the baseline. On the test set, XGBoost achieved an F2 score of 69%, with high precision (90%) but moderate recall (65%). While recall could be improved, the model maintains a good balance, prioritizing the detection of as many actual delays as possible in line with operational goals.

For my **individual contribution**, I led the efforts in exploratory data analysis (EDA), creating all 10 new features for feature engineering, and developed the XGBoost model. I applied Bayesian Optimization for hyperparameter tuning, reducing the risks of overfitting and selection bias to achieve the best performance among all the models tested.

<h3>Tehnologies Used:</h3>
<p>PySpark (MLflow, SQL), Python (Matplotlib, Pandas, NumPy, Seaborn, Datetime), DataBricks on GCP, MapReduce</p>

<h3>Models Utilized</h3>
<p>Logistic Regression (Baseline), <strong>XGBoost (Top Performer)</strong>, Decision Tree, Gradient Boosting, Random Forest, Mulitilayer Perception Classifier, and CNNs.</p>
