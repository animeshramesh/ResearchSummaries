## Rich feature hierarchies for accurate object detection and semantic segmentation (2014)


### Author/paper background
* Ross Girshick - Currently in FAIR. Berkeley PhD
* CVPR 2014, 2400 citations.

### Motivation
* Object detection on PASCAL VOC dataset has plateaued. 
* No scaleable end-to-end algorithm for object detection.

### Solution 
* Generate category-independent region-proposals using selective search (~2000 proposals/image)
* Warp the proposal to 227x227 for input to CNN
* Use pretrained CNN model (AlexNet) to extract 4096-dim vector for each proposal
* Use class-specific linear SVMs to reject/accept proposals.
* Finally apply greedy non-maximum suppression


### Experiments/Evaluation
* Pretrained on AlexNet using image-level annotations (no bounding boxes)
* 21 way classification layer instead of 1000. (20 + background)
* All region-proposals > 0.5 IoU is positive.
* 53.7% mAP on PASCAL VOC 2010


### My analysis
* Test-time detection of 13s/img on GPU and 53s/img on CPU is very slow.


### Future work
* Fast R-CNNs
* Faster R-CNNs
* More logical region proposals?

### Open questions
* How are region proposals constructed?
* Why can't we detect object first and then label those objects?



### Take away 

