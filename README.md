# Numerical Practicum 2022 - Current Overview

Course description follows.

## Section 1/: List of Current Assignments

1. HW1: Recap/Intro of Prerequisites;
2. HW2: Solving Reaction-Diffusion Systems in Pursuit of Turing Patterns (with Bijoy Bera in PDC Course) 
3. HW3: Solving the Poisson-Boltzmann Equation  (with Valeria Gabin and Pouyan Boukany in MTP Course)
4. HW4: Assignment on Applied Transport Phenomena (Tom and Alina)
5. HW5: Assignment on Reactors and Kinectics (Ruud van Ommen)
6. HW6: Assignment on Engineering Thermodynamics (Anna Smith)
7. HW7: Assignment on  Colloids and Interfaces (Laura and Monique)
8. HW8: Assignment on Organic Materials Engineering (Eduardo and Pouyan) 
9. HW9: Assignment on Inorganic Materials Engineering (Laurens Sibelles and Ferdinand Grozema) 
10. HW10: Assignment on Machine Learning by Artur

## Section 2/: Course Overview 

### In general 

- formative assessment during the course: to be defined; 
- summative assessment: via 6 homework assignments - no written exam any more - how to define retake? 

### Common to all Homework Assignments 

- Six assignments in total - 1 ECTS per assignment - 28 hours of work for students  
- in Q1: three compulsory assignments (no freedom of choice)
- in Q2: possibly elective assignments (choice assignment corresponding to course)

### Software installation for the course

- how to ensure that students do not encounter issues with software installation?  
- python and object oriented programming;
- python and the two language problem; 

### Other arrangements to be made

- establish house rules for the course;
- establish Q&A for the course;

## Section 3/: HW1: Recap/Intro of Prerequisites in Various Parts

Our goal: Recap of prerequisites. Prepare for forthcoming assignments. In particular 
1. spatial discretization of first and second order derivatives in space and time using the finite difference method: used in solving Poisson-Boltzmann equation and reaction-diffusion systems; 
2. time-integration methods using explicit and implicit time-integration methods: used in solving reaction-diffusion problems and chemical reactors; 
3. non-linear system solvers using derivative-based methods including techniques to compute the Jacobian: used in Poisson-Boltzmann equation; 
4. solving linear systems solvers using direct solution methods: used in data handling methods and large scale partial differential equation problems; 

### HW1: Part 1/4: Linear Boundary Value Problems on the Interval

Assignment in various sections on solving boundary value problem numerically.
1. Intro into this assignment - explain what the goals are; 
2. State problem to solve. Boundary value problem for the Poisson equation (diffusion with constant coefficient only) on the unit interval with Dirichlet and Neumann boundary conditions;
3. Generate analytical reference solution. Use either by pen-and-paper or using symbolic computations;
4. Generate numerical solution using built-in numerical method (e.g. solve-bvp) 
5. Discretize the problem in space. Introduce into finite difference method for the boundary value problem. Treatment of interior and boundary nodes. Linear system formulation: matrix and right-hand side vector. Make sure to provide sufficient references; 
6. Solve linear system using LU decomposition of the coefficient matrix; compare LU with explicit matrix inverse; 
7. Give physical interpretation of solution obtained (steady state of diffusion of drop of dye in water);  
8. Add linear reaction term. Revisit all previous steps;

References:  
1. [One-Dimensional Finite Difference Method for BVP in Python](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter23.03-Finite-Difference-Method.html)

### HW1: Part 2/4: Extension to Non-Linear Boundary Value Problems on the Interval

1. Add non-linear reaction term. Revisit previous steps. Recognize the problem this time to be non-linear. Identify problem as a root-finding problem in N dimensions. Compute the Jacobian. Solve non-linear system using Newton-Raphson method. Compare with reference solution. Give physical interpretation; 

References:  
1. [Newton's Method in Python](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter19.04-Newton-Raphson-Method.html)
2. [Newton's Method on wiki](https://en.wikipedia.org/wiki/Newton%27s_method)
3. [Jacobian on wiki](https://en.wikipedia.org/wiki/Jacobian_matrix_and_determinant)

### HW1: Part 3/4: Extension to time-dependent and two-dimensional probems 

1. Extend to partial differential and add transient term. State problem to solve. Perform spatial discretization as above. Solve system of ordinary differential equation using a built-in time-stepping method. Give physical interpretation of solution obtained; 
2. Extend to partial differential and add second partial derivastive with respect to space. State problem to solve. Perform spatial discretization as above. Form coefficient matrix as sum of two Kronecker products. Solve linear system of  equations using a built-in time-stepping method. Give physical interpretation of solution obtained;

References 
1. [The Method of Euler in Python](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter22.03-The-Euler-Method.html)
2. [Finite Difference Method for ODE and PDE on wiki](https://en.wikipedia.org/wiki/Finite_difference_method)
3. [2D Discrete Poisson Eqiuation on wiki](https://en.wikipedia.org/wiki/Discrete_Poisson_equation)

### HW1: Part 4/4: Extension to Data Handling and Optimization Methods  

1. Compute average,  derivative and frequency content of the computed solution; 
2. Extend from 1D space (x) to 2D space (x,y) using finite difference method for the Poisson equation. In first step, use manufactured solutions as a reference. Use pulses a point sources or sinks in a subsequent step. The extension to 2D is required for HW2 and HW3. TU Delft bachelor students have no previous experience in solving partial differential equations numerically;   
3. Change problem set-up to meet predefined target using non-linear optimization method. Compute cost function gradient and Hessian. Solve optimization problem using built-in method; 
4. List here possibly other extensions and implementation specific issues; 

Out-of-scope: to be defined; 

References:  
1. to be inserted 

Tentative deadline for students to hand-in their assignment: September 30th; 

Formative assessment: Discussion of how assignment went after grading of assignments;

## Section 4/: HW2: Solving Reaction-Diffusion Systems in Pursuit of Turing Patterns (with Bijoy Bera in PDC Course)

Our goals: 
1. solve reaction-diffusion systems numerically and find Turing patterns; 
2. gradually introduce more advanced coding techniques; 

Assignment in various sections 
1. Solve system of coupled ODEs for reactive systems for various parameter settings. Perform spectral analysis of the Jacobian. See wiki page for example of spectral analysis. Give physical interpretation of solution obtained; 
2. Introduce diffusion in one (single) spatial dimension. Document analytical solutions for the Fisher equation. Source term $F(u) = u(1-u)$. Very similar to growth model in ANM-2021. Explain solutions. Solve Fisher equation using finite differences in space and implicit time-stepping with variable time step; 
3. Extend the Fisher model to the Kolmogorov-Petrovsky-Piskunov model by extending to more general source terms $F(u)$; 
4. Extend above to the Brusselator, the Oregonator, the and the Schnakenberg and the Gray-Scott models; 

References: 
1. [Reaction-Diffusion Systems and Gray-Scott Model](https://en.wikipedia.org/wiki/Reaction–diffusion_system)
2. [Fisher and KPP Equation](https://en.wikipedia.org/wiki/Fisher%27s_equation)
3. [Brusselator Model](https://en.wikipedia.org/wiki/Brusselator)
4. [Oregonator Model](https://en.wikipedia.org/wiki/Oregonator): model for auto-catalysis, and thus interesting to explore; 
5. [Implementation of Brusselator Model Ready to Roll](https://diffeq.sciml.ai/stable/tutorials/advanced_ode_example/) See Hairer-2 for the definition of the test case;  

Help in developing this assignment: Shruti Shruti (TA financed by EEMCS Faculty) 

Tentative deadline for students to hand-in their assignment: October 30th; 


## Section 5/: HW3: Solving the Poisson-Boltzmann Equation  (with Valeria Gabin and Pouyan Boukany in MTP Course)

Our goals:
1. Solve the Poisson-Boltzmann Equation numerically using central second order finite difference in space and Newton iteration to treat the non-linearity; 

References: 
1. [Poisson-Boltzmann Equation](https://en.wikipedia.org/wiki/Poisson–Boltzmann_equation)
2. [Implementation of a Non-Linear Diffusion Equation Ready to Roll](https://rveltz.github.io/BifurcationKit.jl/dev/tutorials/Swift-Hohenberg1d/#d-Swift-Hohenberg-equation-(Automatic)) Possibly better examples do exist

Help in developing this assignment: Abhimanyu Bharade (TA financed by EEMCS Faculty)

Tentative deadline for students to hand-in their assignment: November 30th; 


## Section 6/: HW4: Assignment on Applied Transport Phenomena (Tom and Alina)

See [notebook](HW4-transport.ipynb). 

## Section 7/: HW5: Assignment on Reactors and Kinectics (van Ommen) 

Our goals: 
1. the goal of this assignment is to show examples of non-linear least squares optimization in chemical engineering. The identification of reaction rates in a chemical reaction mechanism from measured concentration data will be used as an example. Given their featuring in the ANM-2021 exam, the reactions of auto-catalysis will be used as a first example. The term forward model refers to solving the set of ordinary differential equations given the reaction rates as input. The term inverse model refers to estimating the reaction rates given measured data and the forward model. The project will target gradient-based optimization methods to minize the model misfit. We will look into gradient-descent, quasi-Newton and Newton methods. The gradient-descent and quasi-Newton require first order sensitivity information. The Newton method requires second order sensitivity information. We will employ ModelingToolkit.jl to represent the system of ordinary differential equations that depend on the parameters (the reaction rates). More details will be given later. 

References:
1. [Autocatalysis](https://en.wikipedia.org/wiki/Autocatalysis) 
2. [Levenberg-Marquard](https://en.wikipedia.org/wiki/Levenberg–Marquardt_algorithm) 
3. [Flux for Differential Equations](https://julialang.org/blog/2019/01/fluxdiffeq/) 
4. [Example of a non-linear least squares problem ready to roll](https://julialang.org/blog/2019/01/fluxdiffeq/) Non-Linear least-squares problem using a neural network problem.|

Help in developing this assignment: Marc Caballero Megia (TA financed by EEMCS Faculty)


## Section 8/: HW6: Assignment on Engineering Thermodynamics (Anna Smith)

See [notebook](HW6-thermo.ipynb). 

## Section 9/: HW7: Assignment on  Colloids and Interfaces (Laura and Monique)

More later: 

References:
1. [wiki on colloid](https://en.wikipedia.org/wiki/Colloid)

## Sect 10/: HW8: Assignment on Organic Materials Engineering (Eduardo and Pouyan) 

Polymer physics, random walk, stochastic differential equations

References:

## Section 11/: HW9: Assignment on Inorganic Materials Engineering (Laurens Sibelles and Ferdinand Grozema) 

References on molecular dynamics simulations:
1. [Short (4.11 min) video giving overview of molecular dynamics](https://www.youtube.com/watch?v=lLFEqKl3sm4)
 Valuable as introductory material, nice voice, good content; 
2. [wiki page on molecular dynamics containing simulations](https://en.wikipedia.org/wiki/Molecular_dynamics)
3. [Tutorial in implementing MD simulations in Python](https://klyshko.github.io/teaching/2019-03-01-teaching)
4. [Molecular Dynamics using openmm.py](https://openmm.org) good content; 
5. [Molecular Dynamics using Molly.jl](https://juliamolsim.github.io/Molly.jl/stable/)
6. Molecular Dynamics simulations for protein-folding: nice stuff! [ProtoSyn.jl code](https://github.com/sergio-santos-group/ProtoSyn.jl) (the list of 14 examples are potentially interesting to look into) and [Short (3.54 min) ProtoSyn video](https://www.youtube.com/watch?v=Z02zw8H-HQc)
7. [(Advanced) Poster Presentation Julia software development for MD simulation](https://www.youtube.com/watch?v=wPRgd0mfwyM)


References on quantum thermodynamic simulations 
1. [Quantum Thermodynamics using Fermi.jl](https://github.com/FermiQC/Fermi.jl)

## Section 12/: HW10: Assignment on Machine Learning by Artur 

Assignment by Artur on machine learning. To be detailed later. 

References
1. [wiki on neural network with valuable schematic](https://en.wikipedia.org/wiki/Neural_network) 
2. [wiki on artificial neural network with broad overview](https://en.wikipedia.org/wiki/Artificial_neural_network#Practical_counterexamples)
3. [Video with history of neural networks](https://www.youtube.com/watch?v=GVsUOuSjvcg)
4. [Overview Paper on Physics informed Neural Networks](https://arxiv.org/pdf/2201.05624.pdf) The part on ODEs might be valuable to us. 



```julia

```


```julia

```
