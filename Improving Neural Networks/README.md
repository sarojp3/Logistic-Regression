## Improving Neural Networks 

<p>There are many ways to improve the working of neural network and make it more efficient by reducing problems like overfitting and underfitting.</p>

<p>Some of the common techniques used are:</p>

  * **Hyperparameter Tuning**
        <p>This includes tuning the values of parameters like learning rate, number of iterations, number of hidden layers and hidden units, choice of activation function and so on.Small changes in these paramters can have great effect on a neural network.</p>
  * **Regularization** 
        <p>Regularization is mainly used to reduce overfitting(high variance) of the data. It is used so that the neural network will compute/produce simpler linear functions rather than very complex non-linear functions. *L2 Regularization* and *Dropout Regularization* are the most common techniques.</p>
  * **Optimization**
         <p>Optimization allows the neural network to learn faster and achieve better performance. To optimize, we can normalize the inputs that makes the cost function look more symmetric.By initializing weights appropriately and checking gradients can help in optimization as well.</p>
         <p>Some of the widely used Optimization algorithms are:</p>
         **1. Mini-Batch Gradient Descent**
                 <p>It involves division of a large training dataset into small training set. For example: if there are 5000000 training examples, we can divide those examples into mini-batches of 1000 examples each. This makes 5000 mini-batches. Typical practice for choosing mini-batch size is power of 2 rule i.e sizes 64(2^6), 128(2^7), 256(2^8) and 512(2^9), {1024(2^10) is rarely used}. Mini-Batch size is also a hyperparameter for a neural network.</p>
         **2. Gradient Descent with Momentum**
                 <p>It uses exponentially weighted averages to smooth out the steps/path of gradient descent to reach minimum. It uses value from past gardient and a hyperparamter beta which can be set with default 0.9 value.</p>
         **3. RMSprop (Root Mean Square prop)**
                 <p>It is similar to the Gradient Descent with Momentum but it uses the square of the value from past gradient.</p>
         **4. Adam Optimization Algorithm**
                 <p>This is widely used optimization algorithm which uses both Gradient Descent with Momentum and RMSprop.</p>
            
