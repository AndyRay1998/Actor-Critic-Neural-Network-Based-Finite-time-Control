# AC-FTC
Implementation of actor-critic based finite time control.  
Terminal sliding mode is utilized to ensure finite settling time, and actor-critic network is to ensure robustness.  
We use RBF network for actor and critic approximator, and continuous sigmoid function for reward calculation.  
The critic is updated based on Recursive Least Square, and actor is based on TD(0) standard policy gradient.  
The algorithm is tested on a 2-DOF manipulator basic tracking task with perturbance.  
The result shows better accuracy near equilibrium and less settling time, but with the cost of enlarged control input.  
https://doi.org/10.1145/3471287.3471288  
