---
layout: post
title: Classifying plankton with deep neural networks
---

### Pre-processing and Data augmentation  
**Pre-processing**  
1. Recaling the images to the normalized size   
2. perform global zero mean unit variance  
  
**Data Augmentation**  

* use various affine transforms  

	* rotation
	* translation  
	* rescaling  
	* flipping  
	* shearing  
	* stretching   
  
* gradually increase the intensity of the augmentation as the model overfit more  

**Network architecture**

* convolutional layer with 3 * 3 filters  
* Cyclic pooling  
	* apply several rotated and flipped versions of the same input image  
	* concatenated the extracted features
	* feed this into a stack of dense layers  
	* further step: pool the features before concatenation
![](http://benanne.github.io/images/cyclicpool.png)
	*  Advantages:
		*  reduce the batch size
	*  Best Pooling Method: root-mean-square
*  Rolling feature maps(a step further of Cyclic pooling)
	* combine the stacks of feature maps from the different orientations into a big stack and then learn features based on this combined input
![](http://benanne.github.io/images/cyclicroll.png) 

* Activations
	* ReLU
	* Maxout
	* parameterized ReLU
	* Leaky ReLU

* Multiscale architectures 
	* because the input has different size, and some species are larger than others. So if we rescale the image into the same size, we will lose the information about this.
	* use combinations of different rescaling strategies within the same network.
	* The best combination: combine a network with inputs rescaled based on the input size with a network rescaled by a fixed factor.

* Additional image features(hand-made features)

![_config.yml]({{ site.baseurl }}/images/config.png)
