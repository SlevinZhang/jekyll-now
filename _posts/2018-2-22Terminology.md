---
layout: post
titile: Terminology for machine learning
---

### Neural Network
1.Bias and Variance  
2.Early Stopping  
3.multi-task learning  
4.manual error analysis  
5.Artificial data sythesis  
6.overfitting & underfitting  
  * overfitting  
    * regularization  
    * dropout | batchnormalization  
    * data augmentation  
    * better neural network  
    * more diverse dataset  
  * Underfitting  
    * better neural network  
    * better training dataset  
    * better optimization algorithm  
    * run more longer | use more complicate neural network
    
7.train set | dev set | test set  
8.Transfer learning & fine-tuning  
9.The distribution of dataset  
  * train set vs dev-set and test-set  
  * data mismatch  
  * train-dev dataset  
  
10.Metric
  * precision  
  * recall | sensitivity  
  * specificity
  * F1 score  
  * False positive rate(how bad)  
  
11.Loss function  
  * cross-entropy  
  * Mean squared error
  * Maximum Likehood    
  * Logistic Loss  
  
12.activation function  
  * Sigmoid  
    * Saturate and kill gradients  
    * output is not zero-mean  
  * Relu  
    * non-saturating  
    * converge more faster  
    * easy to die with large learning rate( output is zero)
  * Leaky-ReLU
    * Solve dying ReLU  
  * Parametric ReLU  
  * Randomized ReLU
  * Maxout  
    * better than ReLU
    * double the parameter  
    * compute two and find the max one
  * ELU  
    * exponential relu  

14.Gradient boosting  
  * produces a prediction model in form of a ensemble of weak prediction models  
  * as a plugging in in the different loss and its gradient  
  
15.Vanishing gradient  
  * Residual networks  
  * Choose a better activation function  
16.Softmax
  * represent a categroical distribution  
  * How to calculate the softmax function for the input  
  * Used in Naive Bayes  
17.Optimization Algorithm  
  * SGD  
  * mini-batch SGD  
  * Momentum( SGD + previous step)  
   * Don't know to slow down
  * Nesterov( SGD + consider about all the history gradient)
   * need to slow down   
  * Adagrad
   * change the learning rate as well
  * Adam
   * Adagrad + Momentum
   
