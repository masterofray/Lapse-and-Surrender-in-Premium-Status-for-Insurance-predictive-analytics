# Instruction
1. Use data vizualization to visualize the data and generate some insight. Make as creative and as presentable as possible.
2. Use this data to create predictive modelling to predict Premium Status (we are interested to find predictive modelling to predice premium status to Lapse and Surrender).

# Summary
1. Our target is to predict value of Lapse and Surrender as in Premium Status Columns.
2. We show the description statistics in this report for every feature and target.
3. We put the graphics as data visualized along the description statistics for every feature.
4. We checked every missing data in every feature and :
	- We dropped some features because of zero value at mean, median, and/or Q75
	- We filled the missing value with its mode
	- We determined the median and fill NULL value with its median.
5. We did feature enginnering for all data type : Categorical, Discrete, Continuous, and Date.
6. 18 Features was included in prediction model calculation.
7. We modelled the prediction by using algorithm of :
	- Logistic Regression
	- k-Nearest Neighbors (KNN)
	- Naive Bayesian
	- Decision Tree
	- Random Forests
	- Support Vector Machines (SVM)

# Model Evaluation Scores
No. Model Score MSE Variance Biased
1. Logistic Regression has score 83.62 and it's MSE is 0.162
2. k-Nearest Neighbors has score 85.00 and it's MSE is 0.182
3. Naive Bayesian has score 81.42 and it's MSE is 0.184
4. Decision Tree has score 88.86 and it's MSE is 0.165
5. Random Forests has score 88.86 and it's MSE is 0.159
6. Support Vector Machines has score 84.68 and it's MSE is 0.153

We evaluated the models using their scores also by Mean Square Error (MSE), variance of prediction result, and the bias.

# Conclussion
We choose prediction from Random forest modelling. While both Decision Tree and Random Forest score likely same, we choose to use Random Forest as they correct for decision tree’s habit of overfitting to their training set. Comparing with Biased value and variance, KNN has lowest biased value. It looks better in accuracy but highest variance. SVM and Logistic Regression are better in focus but lack of accuracy. And the last, we saved the prediction result into CSV file format with the name ’submission.csv’.
