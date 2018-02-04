# TelstraNetwork
#### Data preparation:
-	Dealing with missing data
-	Visualizing features
For example, to find the relative amount the training data accounts for in each feature, and the popular labels within a feature (major votes)
-	Dealing with outlier value
For example, we did data visualization using pivot_table and then log-transfer some outlier data with large value 
-	Hot-encoding categorical features:
For example, when we are analyzing log features during data preparation, we found that log_feature from the original data is categorical. Then we used hot-encodings to represent log features for each id 
-	Grouping continuous features:
For example, when dealing with locations we first interpret them via value_counts, then set the grouping threshold value according to the number of each location. 

#### Xgboost tuning:
- The first note here is that we also plot the feature importance during each round of parameter gridsearch for future feature engineering work, where the n most important features would be considered.
- After 3 rounds of parameter tuning for max_depth and min_child_weight, we got the final submission score 0.50949 
