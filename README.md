## Intro to Deep Learning and Neural Network
 
Concepts used: 
 <ul>
  <li>Logistic Regression,</li>
  <li>Activation Functions,</li>
  <li>Forward Propagation,</li>
  <li>Backward Propagation,</li>
  <li>Vectorization,</li>
  <li>Gradient Descent(Optimization),</li>
  <li>Parameters and Hyperparameters</li>
 </ul>
 <p>These concepts are used completely from scratch without using any deep learning frameworks except in Tensorflow Basics.</p>
 
 #### Softmax Regression
 <p> Softmax regression is used for multi-class classification. For instance, if we have to detect cats, dogs and bird from a single dataset. It is similar to Logistic Regression but it use softmax activation function to compute the cost function. It can be mostly used in Convolutional Neural Network for Object Detections.</p> 

<h4>Main Steps for Building a Neural Network</h4>

 1. Define the model structure such as number of input features.</ul>
 2. Initialize the model's parameters</ul>
 3. Loop:
        <ul>
        <li>Calculate current cost (Forward Propagation)</li>
        <li>Calculate curren gradient (Backward Propagation)</li>
        <li>Update parameters to minimize the cost(Gradient Descent)</li>
        </ul>

<h4>Deep Learning Notations</h4>

<img src="images/notation1.jpg">
<img src = "images/notation2.jpg">
