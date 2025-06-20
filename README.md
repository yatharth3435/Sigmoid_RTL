# Sigmoid_RTL
The Sigmoid activation function is one of the most popular activation functions used in Neural Networks. It is an exponential function which takes an input and outputs in the range (0,1). 
A software implementation of A Neural Network can take a long time, especially for models that involve a lot of computation, since it uses the CPU. Hence, many applications are trying to make these implementations faster.
This project aims to create an optimised Hardware implementation of the piecewise approximated Sigmoid function. Since digital logic components are to be used, An RTL (Register Transfer Level) Verilog implementation is carried out. The inputs and outputs are displayed in the IEEE 753 Floating Point Precision format.
Xilinx Vivado is used to run the simulation on an FPGA board. 

Sigmoid approximation logic:-
If input >= 2; output = 1
If input <= -2; output = 0
If -2 < input < 2; output = (0.25 * input) + 0.5

The aim of the project is to make the implementation as optimised as possible with respect to hardware components, memory and LUTs used and computational complexity. Hence different manipulations and logical tricks are used to reduce comparisions and calculations. 
