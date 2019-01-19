## Week 3 Quiz - Shallow neural networks

1) Which of the following are true? (Check all that apply.)

    -[x] X is a matrix in which each column is one training example.

    -[x] a<sup>[2]</sup> denotes the activation vector of the 2nd layer.

    -[ ] a<sup>[2]</sup><sub>4</sub> is the activation output of the 2nd layer for the 4th training example

    -[x] a<sup>[2](12)</sup> denotes the activation vector of the 2nd layer for the 12th training example.

    -[x] a<sup>2</sup><sub>4</sub> is the activation output by the 4th neuron of the 2nd layer.

    -[ ] X is a matrix in which each row is one training example.

    -[ ] a<sup>[2](12)</sup> denotes activation vector of the 12th layer on the 2nd training example.


2) The tanh activation usually works better than sigmoid activation function for hidden units because the mean of its output is closer to zero, and so it centers the data better for the next layer. True/False?

    -[x] True

    -[ ] False

3) Which of these is a correct vectorized implementation of forward propagation for layer ll, where 1 < = l < = L?

    [x] Z<sup>[l]</sup> = W<sup>[1]</sup>A<sup>[l-1]</sup> + b<sup>[l]</sup>
        A<sup>[l]</sup> = g<sup>[l]</sup>(Z<sup>[l]</sup>)
    
4) You are building a binary classifier for recognizing cucumbers (y=1) vs. watermelons (y=0). Which one of these activation functions would you recommend using for the output layer?

    sigmoid

5) Consider the following code:
A = np.random.randn(4,3)
B = np.sum(A, axis = 1, keepdims = True)

    (4, 1)

6) Suppose you have built a neural network. You decide to initialize the weights and biases to be zero. Which of the following statements is true?

    -[X] Each neuron in the first hidden layer will perform the same computation. So even after multiple iterations of  gradient descent each neuron in the layer will be computing the same thing as other neurons.

    -[ ] Each neuron in the first hidden layer will perform the same computation in the first iteration. But after one iteration of gradient descent they will learn to compute different things because we have “broken symmetry”.

    -[ ] Each neuron in the first hidden layer will compute the same thing, but neurons in different layers will compute different things, thus we have accomplished “symmetry breaking” as described in lecture.

    -[ ] The first hidden layer’s neurons will perform different computations from each other even in the first iteration; their parameters will thus keep evolving in their own way.

7) Logistic regression’s weights w should be initialized randomly rather than to all zeros, because if you initialize to all zeros, then logistic regression will fail to learn a useful decision boundary because it will fail to “break symmetry”, True/False?

    -[x] True
    -[ ] False

8) You have built a network using the tanh activation for all the hidden units. You initialize the weights to relative large values, using np.random.randn(..,..)*1000. What will happen?

    -[x] This will cause the inputs of the tanh to also be very large, thus causing gradients to be close to zero. The optimization algorithm will thus become slow.

    -[ ] This will cause the inputs of the tanh to also be very large, thus causing gradients to also become large. You therefore have to set \alphaα to be very small to prevent divergence; this will slow down learning.

    -[ ] It doesn’t matter. So long as you initialize the weights randomly gradient descent is not affected by whether the weights are large or small.

    -[ ] This will cause the inputs of the tanh to also be very large, causing the units to be “highly activated” and thus speed up learning compared to if the weights had to start from small values.





