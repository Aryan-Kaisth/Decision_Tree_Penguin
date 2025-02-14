# Decision Tree Penguin 
Project Workflow
1. Data Preprocessing
Handling Missing Values: Filled missing values using the mean for numerical columns.
Outlier Detection & Treatment: Used boxplots to visualize outliers and made necessary adjustments.
Encoding Categorical Variables: Applied one-hot encoding for categorical features using pd.get_dummies().
Feature Scaling: Used StandardScaler to standardize numerical features for better model performance.
2. Feature Selection
Implemented Recursive Feature Elimination (RFE) to select the most important features.
Experimented with different numbers of features (2 to 6) to find the optimal subset.
3. Model Training & Optimization
Pipeline Integration: Combined feature selection and model training into a single pipeline for efficiency.
Hyperparameter Tuning: Used GridSearchCV to optimize key Decision Tree parameters:
max_depth (controls tree depth)
min_samples_split (minimum samples required to split a node)
n_features_to_select (optimal number of features)
Achieved a final accuracy of 0.94 on the test data.
4. Model Evaluation & Interpretation
Accuracy Measurement: Evaluated the best model using cross-validation accuracy.
Decision Tree Visualization: Plotted the final optimized Decision Tree to interpret decision boundaries.
5. Model Deployment
Saving the Best Model: Used joblib.dump() to save the trained model for future predictions.
The saved model can be loaded and used directly for inference without retraining.
