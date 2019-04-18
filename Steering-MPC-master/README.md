# Steering-MPC

...

% Readme
% This file contains brief information about the code.
%
% Author : Shawn Daniel


About the Project -
The following code directories are the simulations of the steering car problem using MPC to track a trajectory. 
In Simulation I we have the simulation of a Holonomic car model, meaning the states areonly inertial frame longitudinal, 
lateral positions, and heading.The vehicle is assumed to have body frame longitudinal velocity which can be generated by breaks,
 or acceleration(gas).
 In Simulation II we have simulation of a simple full dynamic model of a car, and the states are body frame longitudinal  and lateral velocity, inertial frame "X and Y", heading, heading rate of change. The longitudinal velocity o the vehicle is assumed constant and the only control herer is the front wheel turning angle. This code involves a nonlinear equation model of a pneumatic tire, using Pacejka Magic Tire formula. The equation of motion is nonlinear, so  Linear time invariant LTV MPC was used with MPC to track reference trajectory in discrete time. Additionally, obstacle avoidance is also experimented and played with.


The papers referenced for these two codes are:
F. Borrelli, P. Falcone, T. Keviczky, J. Asgari, and D. Hrovat,
“MPC-based approach to active steering for autonomous vehicle
systems,” Int. J. Vehicle Autonomous Systems, vol. 3, no. 2/3/4,
pp. 265–291, 2005.

Bakker, E., Nyborg, L., Pacejka, H. B., 1987. "Tyre modeling for use in vehicle dynamics studies". SAE paper # 870421.
Please check the report for other references.

System Requirements -
You need to have the MATLAB Optimization Toolbox installed in order to run this program.


Extra Files -
There are a few auxiliary files which haven't been activated by default in the main code, but might provide valuable insight in some cases. These are -

Fun Notes: In locations where the script "O PLAY" is seen, this notes where a user can change parameters to see the convergence nature of MPC




