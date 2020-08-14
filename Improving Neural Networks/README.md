## Improving Neural Networks 

<p>There are many ways to improve the working of neural network and make it more efficient by reducing problems like overfitting and underfitting.</p>

<p>Some of the common techniques used are:</p>

  * **Hyperparameter Tuning**
        <p>This includes tuning the values of parameters like learning rate(alpha), number of iterations, number of hidden layers(L) and hidden units(n), choice of activation functions(sigmoid, tanh, ReLU, Leaky ReLU) and so on.Small changes in these paramters can have great effect on a neural network.The most important hyperparameter to tune is learning rate and the appropraite scale to choose for it is 0.0001 to 1. Similarly for beta, which is also a hyperparameter, the scale is 0.9 to 0.999.</p>
        <p>There are some tips for organizing hyperparameter search.</p>
           **i) Babysitting One Model(also called Panda approach)**
                     <p>This approach involves watching performance of the model and patiently nudging the learning rate up and down. Such approach is used if there is no enough computational capacity to train a lot of models at the same time.</p>
           **ii) Training Many Models in Parallel(also called Caviar Approach)**
                     <p>This involves training different models with different hyperparameter values at the same time and choosing the best one from them. It is used if there is enough computers with computational capacity to train a lot of models in parallel.</p>
         <p>Another key concept in hyperparameter tuning is **Batch Normalization** which is used in normalizing actvations in a network. This enables us train very deep neural network much more easily. In deep neural network, we implement normalizations on 'z' instead of 'a' of hidden layers. Batch Norm is applied with mini-batches of the training set where it processes the data one mini-batch at a time during the training process.</p>
         
  * **Regularization** 
        <p>Regularization is mainly used to reduce overfitting(high variance) of the data. It is used so that the neural network will compute/produce simpler linear functions rather than very complex non-linear functions. *L2 Regularization* and *Dropout Regularization* are the most common techniques. </p>
  * **Optimization**
         <p>Optimization allows the neural network to learn faster and achieve better performance. To optimize, we can normalize the inputs that makes the cost function look more symmetric.By initializing weights appropriately and checking gradients can help in optimization as well.</p>
         <p>Some of the widely used Optimization algorithms are:</p>
         **1. Mini-Batch Gradient Descent**
                 <p>It involves division of a large training dataset into small training set. For example: if there are 5000000 training examples, we can divide those examples into mini-batches of 1000 examples each. This makes 5000 mini-batches. Typical practice for choosing mini-batch size is power of 2 rule i.e sizes 64(2^6), 128(2^7), 256(2^8) and 512(2^9), {1024(2^10) is rarely used}. Mini-Batch size is also a hyperparameter for a neural network.</p>
         **2. Gradient Descent with Momentum**
                 <p>It uses exponentially weighted averages to smooth out the steps/path of gradient descent to reach minimum. It uses value from past gardient(dW and db) and a hyperparamter beta which can be set with default 0.9 value.</p>
         **3. RMSprop (Root Mean Square prop)**
                 <p>It is similar to the Gradient Descent with Momentum but it uses the square of the value from past gradient(dW^2 and db^2).</p>
         **4. Adam Optimization Algorithm**
                 <p>This is widely used optimization algorithm which uses both Gradient Descent with Momentum and RMSprop.</p>


            
