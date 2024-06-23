# Decision-Tree-based-ID3-Algorithm
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


## Gini impurity
## Entropy
Entropy is a measure of randomness or disorder. It shows the uncertainity in the dataset.  
![image](https://github.com/vvvvvvss/Decision-Tree-based-ID3-Algorithm/assets/148562671/f46e0e2e-0b63-43b8-8e57-d6a88ce8d5a2)
where,  
p+ is the probability of positive class  
p– is the probability of negative class  
S is the subset of the training example  
Higher the entropy, lower the purity of the dataset. 
