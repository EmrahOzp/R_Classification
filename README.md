# R_Classification
Classification Models built in R

DATA SET 1 + BUSINESS PROBLEM DESCRIPTION
This dataset contains information about the users of a social network; 
“UserID”, “Gender”, “Age”, “Estimated Salary”, and a binary purchased decision “Yes” or “No”. 
Social network has many business clients, and try to implement a classification algorithm when one business client launches 
a new car model, to predict the correct targeted audience who responded positively to the advertisement.

LOGISTIC REGRESSION
Logistic regression will try to understand the correlation between information Age and Salary
and decision of the user whether Yes or No to buy the new product. 

K-NEAREST NEIGHBOR 
Step by step
	Choose the number K of neighbors (default = 5)
	Take the K nearest neighbors of the new data point, according to the Euclidean distance 
	Among these K-neighbors, count the number of data points in each category
	Assign the new data point to the category where you counted the most neighbors.

SUPPORT VECTOR MACHINE 
Objective is the find the best decision boundary which will help to separate classes. 
SVM searches this optimum line through a maximum margin (equal distance between the classes). 
Those vectors are called the support vectors (Positive hyperplane / negative hyperplane) around 
the maximum margin hyperplane (maximum margin classifier). To use this we assume our dataset is linearly separable. 

KERNEL SVM 
We use this if our data is not linearly separable. Kernel SVM helps us to find the decision boundary.
We do it by mapping into a higher dimensional space (using a mapping function) and build a decision boundary and 
project it back to the data set. Setback is mapping to a higher dimensional space can be highly compute-intensive which cause 
a lot of issues. That’s where we apply a Kernel Trick; by adjusting the “sigma” inside the kernel function.
So that, we can build the decision boundary without going to the higher dimensional space and everything will go in the lower dimension.

NAÏVE BAYES CLASSIFICATION
This is a model based on probabilities. 
Posterior Probability = (likelihood * Prior Probability) / Marginal likelihood
It requires independence assumption, it assumes there is no correlation between independent variables. 

DECISION TREE CLASSIFICATION
Decision Tree, slices down the dataset with several iterations. The splits are selected by the algorithm to maximize 
the category it belongs. Splits are try to minimize the information entropy. 

RANDOM FOREST CLASSIFICATION
This is an ensemble learning algorithm which uses many decision tree iterations. 
	Pick at random K data points from the Training set
	Build the decision tree associated to these K data points
	Choose the number Ntree of trees you want to build and repeat the previous steps. 
	For a new data point, make each one of your Ntree trees predict the category to which 
the data points belongs, and assign the new data point to the category that wins the majority vote.

