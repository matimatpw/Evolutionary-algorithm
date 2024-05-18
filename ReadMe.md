# Evolutionary Algorithm

This repository contains an implementation of the Evolutionary Algorithm with strategy EE(1+1) using Python. It is designed to optimize functions through evolutionary strategies, adapting step sizes based on the success rate of iterations.

## Usage
* Objective function

The **objective_function** is designed to take a numpy array x and return a scalar value. This function is used to evaluate the performance of the evolutionary algorithm.

* Solver

The **evolution_1p1** function performs the evolutionary optimization. It takes the following parameters:

-f: The objective function to be minimized.

-x0: The initial point as a numpy array.

-o_p: An instance of optim_params containing control rate, step size, maximum iterations, mean,
deviation, and adaptation parameters.

-stepsize_adaptation: A function to adapt the step size based on iteration success rate.

The evolution_1p1 function returns an instance of optim_result containing the history of function values, iterations, and stopping information.

* Comparison Function

The **comparision function** sets up and runs a comparison between different configurations of the optimizer using the cec2017 benchmark functions. It prints the output of the optimization process for review.