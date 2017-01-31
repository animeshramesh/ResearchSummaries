## Visualizing and Understanding Convolutional Networks, ECCV 2014 

### Author background
* Matthew D. Zeiler [NYU PhD student] and Rob Fergus 
* Zeiler is the cofounder of Clarifai.

### Motivation
* No clear understanding of why CNNs perform well. Need to dig deep so that we can improve.

### Solution 
* DeconvNets proposed by the author in 2011, which projects feature activations back to input space.
* DeconvNet attached to each of the layers.
* Record location of maxima in each pooling region using *switch variables*.
* Reveal structures in the input which excite the feature map.
* Invariance to input deformations. (due to convolutions)
* Visualizations can be used to debug nets/select good architectures.


### Experiments/Evaluation
* Similar setup as AlexNet.
* Authors visualized AexNet responses, found problems in that and trained a different model which improves accuracy on ImageNet.
* Occluded different portions if input img with a grey square and monitored the output of the classifier -> accuracy drops when 
object is occluded. Which means that the model is actually localizing the object in the img.


### My analysis
* The authors have solved an important challenge by just connecting the dots.
* Paper does not comment on how to debug network by just visualization.


### Future work


### Open questions
* Why is visualization done on the validation set? Why not on the training set?
* Objects in Layer 2 don't make any sense! Wtf? Are these textures? 


### Take away 

