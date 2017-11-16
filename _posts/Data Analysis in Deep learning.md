### Preprocessing Data
* create Validation, Sample, train, test, 4 types of data set  
* make data is under the folder named by their own class(except test), we could use flow from dirctory to get data 
* test data batches fetcher to see if it works  
### Start trainning network  
* build up the architecture of the network  
* choose the layers that are trainable  
* load weights
* fine tune the model on sample dataset to figure out some questions(what kind of questions)
* introduce data augmentation(there are some methods that can't get from sample dataset) and find the best super_parameter based on sample dataset
* make sure the model get the best performance on the sample dataset
* then move to full dataset
### Evaluate the trained model
* Generate the prediction of validation set and analyse the correct example and false prediction
* plot confusion matrix
* analyse recall / accuracy / 


### How to use Sample Data
* find best set of hyper-parameters
* test the effect of data augmentation
* 