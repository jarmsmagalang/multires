# Multiresolution Algorithm

This package is an implementation of the standard and hybrid multiresolution algorithm as proposed in "Analytic and Monte Carlo Approximations to the Distribution of the First Passage Time of the Drifted Diffusion with Stochastic Resetting and Mixed Boundary Conditions" by J. Magalang, R. Turin, et. al. 

This package contains functions that will either generate a single first passage time or the a single full trajectory for either simulation scheme. 

To run a simulation, begin by first choosing the scheme that you want:
1.  `smra` for the standard MRA
2. `hmra` for the hybrid MRA

Please refer to the function docstring for a detailed list of the arguments required for either function, e.g. use `help(smra)` after importing the package. By default, either simulation scheme will produce a first passage time, rather than a full trajectory.

This package also contains auxiliary functions:
1. `increase_resolution` increases the resolution of a trajectory from level $k-1$ to $k$ given that the input array has length $2^{k-1}+1$, following Equation 4.3 of Magalang, Turin, et. al.
2. `euler` is an implementation of the Euler-Maruyama algorithm which outputs a full trajectory and is required for the HMRA.

# Installation

[will be up once the package is on pypi, conda, and github]

> Written with [StackEdit](https://stackedit.io/).
