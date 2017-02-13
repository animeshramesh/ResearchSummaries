## Tinkering Under the Hood: Interactive Zero-Shot Learning with Net Surgery

### Author background
* Vivek Krishnan, Deva Ramanan

### Motivation
* Zero shot learning
* Network activation Visualization



### Solution 
* Pictorial Language Classifier - Deformable Parts model
* Interactive zero-shot learning - relies on human to provide semantics. (spatial logic and combination of parts logic)
* Retinotopic embeddings - Embeddings of conv features.



### Experiments/Evaluation
* Trained on AlexNet.



### My analysis
* The paper is haphazardly structured. It's problem statement remains mysterious. It is highly incoherent.
* Aren't linguistic queries easier? PLC looks cool. But why PLC?
* The proposed PLC doesn't seem to be backed by any reliable structure. 
* There is no single strong contribution. There's PLC, visualization, zero-shot learning, object detection. What are they trying to achieve?




### Future work


### Open questions
* Why PLC?
* Why are embeddings 2304 dimensional?
* Why represent an activation as a line?
* I think the approach is more relevant to image retrieval, rather than zero-shot learning.


### Take away 
* PLC to implement interactive human learning.

