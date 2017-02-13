## Low-shot Visual Recognition by Shrinking and Hallucinating Features

### Author background


### Motivation
* Low-shot learning is something humans perform intuitively. However, exisitng ML algos do not generalize well.


### Solution
* Two training phases - Representation learning and Low-shot learning.
* Accuracy gain in low-shot setting must not come at the expense of reduced accuracy of base classes?
* Squared Gradient Magnitude - Encode end-goal of low-shot training during training. 
* Loss function which penalizes the difference between classifiers learnt on large and small datasets.
* "Hallucinate" additional examples for novel classes by transferring modes of variation from base classes. (category independent transformations)
* The second phase enables us to add additional categories. Dataset used in second phase also has base classes. (1-20 instances per class max) 



### Experiments/Evaluation
* 5 trials over set of base + novel classes.
* MLP with 3 FC layers to hallucinate features - supervised regression.



### My analysis



### Future work


### Open questions
* They use separate, independent training phases. What if they merge these two?



### Take away 

