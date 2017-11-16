### Functional Model Method
1. Creating Model
	1. model.compile()
	2. 
2. Training model
	1. model.fit(x,y,batch_size=None,epochs = , verbose = 1, ...)
	2. model.train\_on\_batch() Run the model on the single batch and we could monitor the change of loss
	3. model.fit_generator(): fits the model on data yielded batch-by-batch by a python generator
3. Prediction
	1. model.predict(): used to deploy to predict the new case
	2. model.predict\_on\_batch(x)
	3. model.predict_generator()
4. Evaluation
	1. model.evaluate(): return the loss value & metrics values for the model
	3. model.test\_on\_batch():test the model on the single batch
	4. model.evaluate_generator(): evaluate the model on a data generator
5. Visualiztion
	1. model.get_layer(name=None,index=None): retrieve a layer based on its name or index


### Loss Function
from keras import losses  
### hot code the ground truth
from keras.utils.np_utils import to_categorical

### Measure the performance
from keras import metrics  

### usage of optimizers
from keras import optimizers

### Usage of activations
from keras import backend as K  
`k.tanh`  
`softmax`
`elu`
`selu`

### usage of callback

### Applications
The deep learning model we usually use in daily life  
`from keras.applications.resnet50 import ResNet50`  
read image with keras  
`from keras.preprocessing import image`  

