# Decisiontree

How Do Decision Trees Work?
There are several steps involved in the building of a decision tree.
1)Splitting
The process of partitioning the data set into subsets. Splits are formed on a particular variable
2)Pruning
The shortening of branches of the tree. Pruning is the process of reducing the size of the tree by turning some branch nodes into leaf nodes, and removing the leaf nodes under the original branch. Pruning is useful because classification trees may fit the training data well, but may do a poor job of classifying new values. A simpler tree often avoids over-fitting.
3)Tree Selection
The process of finding the smallest tree that fits the data. Usually this is the tree that yields the lowest cross-validated error.




key factors:
1. Entropy
A decision tree is built top-down from a root node and involves partitioning the data into subsets that contain instances with similar values (homogeneous). ID 3 algorithm uses entropy to calculate the homogeneity of a sample. If the sample is completely homogeneous the entropy is zero and if the sample is an equally divided it has entropy of one.
2. Information Gain
The information gain is based on the decrease in entropy after a dataset is split on an attribute. Constructing a decision tree is all about finding attribute that returns the highest information gain (i.e., the most homogeneous branches).

Step 1:
Calculate entropy of the target.
Step 2:
The dataset is then split on the different attributes. The entropy for each branch is calculated. Then it is added proportionally, to get total entropy for the split. The resulting entropy is subtracted from the entropy before the split. The result is the Information Gain, or decrease in entropy.
Step 3:
Choose attribute with the largest information gain as the decision node, divide the dataset by its branches and repeat the same process on every branch.



These are the basic parameter which are useful when we are doing the decision tree analysis.
