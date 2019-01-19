1. Which of the following are true? (Check all that apply.)

[X] X is a matrix in which each column is one training example.

[x] a<sup>[2]</sup> denotes the activation vector of the 2nd layer.

[ ] a<sup>[2]</sup><sub>4</sub> is the activation output of the 2nd layer for the 4th training example

[x] a<sup>[2](12)</sup> denotes the activation vector of the 2nd layer for the 12th training example.

[x] a<sup>2</sup><sub>4</sub> is the activation output by the 4th neuron of the 2nd layer.

[ ] X is a matrix in which each row is one training example.

[ ] a<sup>[2](12)</sup> denotes activation vector of the 12th layer on the 2nd training example.


2. The tanh activation usually works better than sigmoid activation function for hidden units because the mean of its output is closer to zero, and so it centers the data better for the next layer. True/False?

[x] True

[ ] False

3. Which of these is a correct vectorized implementation of forward propagation for layer ll, where 1 < = l < = L?

[x] Z<sup>[l]</sup> = W<sup>[1]</sup>A<sup>[l-1]</sup> + b<sup>[l]</sup>
    A<sup>[l]</sup> = g<sup>[l]</sup>(Z<sup>[l]</sup>)
