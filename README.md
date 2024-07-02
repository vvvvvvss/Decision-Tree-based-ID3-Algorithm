# Decision-Tree
Decision trees are both a clssification and regression supervised machine learning model. The model is visual represent as tree. 
Each node is a yes/no question. Based on the anwser, the tree splits in branches different branches. One representing yes and the other no. 
Each of these branch again ends with a decision node. This recursive process continues and finally reaches a decision leave which makes the prediction  
![image](https://github.com/vvvvvvss/Decision-Tree-based-ID3-Algorithm/assets/148562671/44d3995f-b6e3-44fa-ba33-9dbaf95cad59)
Clearly Decision trees make only binary splits.  
Decison trees assume that the features in the dataset are independant, but in practice they work well even if the features are corelated. 
Decision trees are sensitive to outliers. Extreme values may influence their construction. Also be aware of overfitting, small datsets may lead to oiverfitting

## Decision trees for numerics
 
## Information Gain
The Information Gain measures the expected reduction in entropy. It is used to determine the root node.
`Information Gain = Entropy(Parent) − Weighted Average Entropy(Children)`
The feature which has minimum impurity will be considered as the root node.
Information Gain calculates the reduction in the entropy and measures how well a given feature separates or classifies the target classes. The feature with the highest Information Gain is selected as the best one.

## Gini impurity
## Entropy
Entropy is a measure of randomness or disorder. It shows the uncertainity in the dataset. Shannon's entropy model uses logarithm of function P(x) to the base 2 to measure the entropy. Once a dataset contains more than one "type" of elements specifically more than one target feature value, the impurity will be greater than zero, which means entropy is alos greater than zero.  
![image](https://github.com/vvvvvvss/Decision-Tree-based-ID3-Algorithm/assets/148562671/f46e0e2e-0b63-43b8-8e57-d6a88ce8d5a2)  
where,  
p+ is the probability of positive class  
p– is the probability of negative class  
S is the subset of the training example  
Higher the entropy, lower the purity of the dataset. 

# ID3
ID3 stands for Iterative Dichotomiser 3 and is named such because the algorithm iteratively (repeatedly) dichotomizes(divides) features into two or more groups at each step.
ID3 uses a **top-down greedy approach**. Top-down approach simply means aproaching the top most node first and gradually moving downwards. While greedy approach means at each iteration the model picks the best feature. ID3 is usually used with nominal features only. We know that ID3 selects the best features only. For this ID3 uses Information gain.

# Calculation
`
