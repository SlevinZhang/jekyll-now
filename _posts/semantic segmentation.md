### Semantic segmentation
it provides region segmentation like mean-shift algorithm  
### 3 methods  
1. Fully convolutional Networks
	1. output is a heatmap for each class, and to know where is the object is.
	2. it can accommodate images of any size
	3. 
	2. Question
		1. how to generate the ground truth
			1. after the deconvolution, the ouput will be the same size as the input
		2. the problem of size of heatmap (which is dependent on the image size)
			1. Solution: backproject heatmap to image pixel through deconvolution
		2. The depth 
		3. pool <-> upsample?
1. Learning Deconvolution Network for semantic segmentation  
	1. idea
		1. do the stride of 1/s(original stride)  
		2. spread it in length S and fill 0 between the 
2. Mask R-CNN(build a segmentor on top of Faster R-CNN) 
	1. instance segmentation
	2. Mask layer(pixel level classifier)
	3. apply mask prediction to highest scoring 100 boxes
	3. 
3. SegNet
4. U-Net
5. Fully Convolutional DenseNet
6. E-net and Link-net
7. PSPnet
8. RefineNet
9. G-FRNet

### Semi-supervised Semantic segmentation
1. DecoupleNet
2. GAN Based Approaches
