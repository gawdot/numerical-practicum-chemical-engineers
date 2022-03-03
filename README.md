# Numerical Practicum 2022 - Current Overview

## Section 1/: Common to all Homework Assignments

- Six assignments in total - 1 ECTS per assignment - 28 hours of work for students  
- in Q1: three compulsory assignments (no freedom of choice)
- in Q2: possibly elective assignments (choice assignment corresponding to course)

## Section 2/: HW1: Recap/Intro of Prerequisites in Various Parts

Our goal: Recap of prerequisites; 

Assignment in various sections on solving boundary value problem numerically.  
1. Intro into this assignment - explain what the goals are; 
2. State problem to solve. Boundary value problem for the Poisson equation (diffusion with constant coefficient only) on the unit interval with Dirichlet and Neumann boundary conditions;
3. Generate analytical reference solution. Use either by pen-and-paper or using symbolic computations;
4. Generate numerical solution using built-in numerical method (e.g. solve-bvp) 
5. Discretize the problem in space. Introduce into finite difference method for the boundary value problem. Treatment of interior and boundary nodes. Linear system formulation: matrix and right-hand side vector. Make sure to provide sufficient references; 
6. Solve linear system using LU decomposition of the coefficient matrix; compare LU with explicit matrix inverse; 
7. Give physical interpretation of solution obtained (steady state of diffusion of drop of dye in water);  
8. Add linear reaction term. Revisit all previous steps; 
9. Add non-linear reaction term. Revisit previous steps. Recognize the problem this time to be non-linear. Identify problem as a root-finding problem in N dimensions. Compute the Jacobian. Solve non-linear system using Newton-Raphson method. Compare with reference solution. Give physical interpretation. Solving non-linear model will prepare for HW3; 
10. Extend to partial differential and add transient term. Perform spatial discretization as above. Solve system of ordinary differential equation using a built-in time-stepping method; 
11. Compute average,  derivative and frequency content of the computed solution; 
12. Extend from 1D space (x) to 2D space (x,y) using finite difference method for the Poisson equation. In first step, use manufactured solutions as a reference. Use pulses a point sources or sinks in a subsequent step. The extension to 2D is required for HW2 and HW3. TU Delft bachelor students have no previous experience in solving partial differential equations numerically;   
13. Change problem set-up to meet predefined target using non-linear optimization method. Compute cost function gradient and Hessian. Solve optimization problem using built-in method; 
14. List here possibly other extensions and implementation specific issues; 

Out-of-scope: to be defined; 

References:  
1. [Finite Difference Method in Python](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter23.03-Finite-Difference-Method.html)  

Tentative deadline for students to hand-in their assignment: September 30th; 

Formative assessment: Discussion of how assignment went after grading of assignments;

## Section 3/: HW2: Solving Reaction-Diffusion Systems in Pursuit of Turing Patterns (with Dr. Bera in PDC Course)

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


## Section 4/: HW3: Solving the Poisson-Boltzmann Equation  (with Dr. Gabin and Dr. Boukany in MTP Course)

Our goals:
1. Solve the Poisson-Boltzmann Equation numerically using central second order finite difference in space and Newton iteration to treat the non-linearity; 

References: 
1. [Poisson-Boltzmann Equation](https://en.wikipedia.org/wiki/Poisson–Boltzmann_equation)
2. [Implementation of a Non-Linear Diffusion Equation Ready to Roll](https://rveltz.github.io/BifurcationKit.jl/dev/tutorials/Swift-Hohenberg1d/#d-Swift-Hohenberg-equation-(Automatic)) Possibly better examples do exist

Help in developing this assignment: Abhimanyu Bharade (TA financed by EEMCS Faculty)

Tentative deadline for students to hand-in their assignment: November 30th; 


## Section 5/: HW4: Assignment on Applied Transport Phenomena (Tom and Alina)

References: 
1. [CFD in Python](https://lorenabarba.com/blog/cfd-python-12-steps-to-navier-stokes/)
2. [Hyperbolic Convervation Lwas on Adaptive Grids - TRIXIE](https://github.com/trixi-framework/Trixi.jl) 
3. [Immersed Boundary Method - Waterlily](https://github.com/weymouth/WaterLily.jl)

## Section 6/: HW5: Assignment on Reactors and Kinectics (van Ommen) 

Our goals: 
1. the goal of this assignment is to show examples of non-linear least squares optimization in chemical engineering. The identification of reaction rates in a chemical reaction mechanism from measured concentration data will be used as an example. Given their featuring in the ANM-2021 exam, the reactions of auto-catalysis will be used as a first example. The term forward model refers to solving the set of ordinary differential equations given the reaction rates as input. The term inverse model refers to estimating the reaction rates given measured data and the forward model. The project will target gradient-based optimization methods to minize the model misfit. We will look into gradient-descent, quasi-Newton and Newton methods. The gradient-descent and quasi-Newton require first order sensitivity information. The Newton method requires second order sensitivity information. We will employ ModelingToolkit.jl to represent the system of ordinary differential equations that depend on the parameters (the reaction rates). More details will be given later. 

References:
1. [Autocatalysis](https://en.wikipedia.org/wiki/Autocatalysis) 
2. [Levenberg-Marquard](https://en.wikipedia.org/wiki/Levenberg–Marquardt_algorithm) 
3. [Flux for Differential Equations](https://julialang.org/blog/2019/01/fluxdiffeq/) 
4. [Example of a non-linear least squares problem ready to roll](https://julialang.org/blog/2019/01/fluxdiffeq/) Non-Linear least-squares problem using a neural network problem.|

Help in developing this assignment: Marc Caballero Megia (TA financed by EEMCS Faculty)


## Section 7/: HW6: Assignment on Engineering Thermodynamics (Anna Smith)

See slides for request to Anna to provide more input. 

References:

## Section 8/: HW7: Assignment on  Colloids and Interfaces (Laura and Monique)

More later: 

References:

## Section 9/: HW8: Assignment on Organic Materials Engineering (Eduardo and Pouyan) 

Polymer physics, random walk, stochastic differential equations

References:

## Section 10/: HW9: Assignment on Inorganic Materials Engineering (Laurens Sibelles and Ferdinand Grozema) 

References:
1. [Molecular Dynamics](https://juliamolsim.github.io/Molly.jl/stable/)
2. [Quantum Thermodynamics](https://github.com/FermiQC/Fermi.jl)

## Section 11/: HW10: Assignment on Machine Learning by Artur 

Assignment by Artur on machine learning. To be detailed later. 


```julia

```


```julia

```
