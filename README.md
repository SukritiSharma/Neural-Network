# Neural-Network
This is a simple model with single neuron with three input and single output.

Model will be train the neuron to solve the problem below. The first four examples are called a training set. Test set will be Should the ‘?’ be 0 or 1?


|          | Input | |  | Output |
|----------|---|---|---|--------|
| Example 1| 0 | 0 | 1  | 0      |
| Example 2| 1 | 1 | 1  | 1      |
| Example 3| 1 | 0 | 1  | 1      |
| Example 3| 0 | 1 | 1  | 1      |
| Test     | 0 | 1 | 1  | ?      |


In above example output is always equal to the value of the leftmost input column. Therefore the answer is the ‘?’ should be 1.

First I have set each weight to a random number. Then training process begins as:

* Input is taken from a training set example, adjusted them by the weights, and passed them through a special formula to calculate the neuron’s output.
* Error is calculated, which is the difference between the neuron’s output and the desired output in the training set example.
* Depending on the direction of the error, weights are adjusted slightly.
* Process is 1000 times.

Output of neuron is calculated by taking weighted sum of input and then normalising it so that result is between 0 and 1. 
![alt text](https://github.com/SukritiSharma/Neural-Network/blob/master/img/output.pngg "Output equation")

Weighted sum is calculated as 
![alt text](https://github.com/SukritiSharma/Neural-Network/blob/master/img/weight_sum.png "Weighted sum")

Normalised through sigmoid function
![alt text](https://github.com/SukritiSharma/Neural-Network/blob/master/img/sigmoid_eq.png "Sigmoid eq")

If plotted on a graph, the Sigmoid function draws an S shaped curve.

![alt text](https://github.com/SukritiSharma/Neural-Network/blob/master/img/sigmoid_graph.png "Sigmoid eq")

