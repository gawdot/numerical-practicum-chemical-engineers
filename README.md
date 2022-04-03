# Numerical Practicum 2022 - Current Overview

Course description follows.

## Section 1/: List of Current Assignments

1. HW1: [Recap/Intro of Prerequisites](homework1/notebooks/HW1-intro.ipynb);
2. HW2: [Solving Reaction-Diffusion Systems in Pursuit of Turing Patterns (with Bijoy Bera in PDC Course)](homework2/notebooks/HW2-pde-reaction-diffusion.ipynb) 
3. HW3: [Solving the Poisson-Boltzmann Equation  (with Valeria Gabin and Pouyan Boukany in MTP Course)](homework3/notebooks/HW3-poisson-boltzmann.ipynb)
4. HW4: [Assignment on Applied Transport Phenomena (Tom and Alina)](homework4/notebooks/HW4-applied-transport-phenomena.ipynb)
5. HW5: [Assignment on Reactors and Kinectics (dialogue with Ruud van Ommen)](homework5/notebooks/HW5-ode-reactors.ipynb)
6. HW6: Assignment on Engineering Thermodynamics (Anna Smith)
7. HW7: Assignment on  Colloids and Interfaces (Laura and Monique)
8. HW8: Assignment on Organic Materials Engineering (Eduardo and Pouyan) 
9. HW9: Assignment on Inorganic Materials Engineering (Laurens Sibelles and Ferdinand Grozema) 
10. HW10: Assignment on Machine Learning by Artur

## Section 2/: Course Overview 

### In general 

- formative assessment during the course: to be defined; 
- summative assessment: via 6 homework assignments - no written exam any more - how to define retake? 
- auto-grading of the assignments using nb-grader and unit-tests (give information to the students); 

### Common to all Homework Assignments 

- Six assignments in total - 1 ECTS per assignment - 28 hours of work for students  
- in Q1: three compulsory assignments (no freedom of choice)
- in Q2: possibly elective assignments (choice assignment corresponding to course)

### Software installation for the course

- how to ensure that students do not encounter issues with software installation?  
- python and object oriented programming;
- python and the two language problem; 
- [Hans Petter Langtangen, A Primer in Scientific Computing Using Python, PDF file, 900+ pages](https://hplgit.github.io/primer.html/doc/pub/half/book.pdf): Can we summarize? Can we find other examples? 

### Other arrangements to be made

- establish house rules for the course;
- establish Q&A for the course;
- Vocareum for auto-grading of the assignments;

## Section 3/: Python, Jupyter and Vocareum Introduction (needs revision)  

Divide students in the following three groups: TU bachelor, entirely strange to Python and in between group. Define seperate tasks for the three groups. 

Introduction in Python programming in four parts. Used as reference for future parts of the course. (Encourage TU Delft bachelor students to give Part 4/4 a look?, how to provide opportunity to practice, how do other courses do so?)
1. [Part 1/4](intro-python/notebooks/ANM_2020_PythonIntro1.ipynb): introduction; operations of vectors and matrices; plotting; 
2. [Part 2/4](intro-python/notebooks/ANM_2020_PythonIntro2.ipynb): functions, particular matrices, matrix-vector operations, linear Systems and more plotting;
3. [Part 3/4](intro-python/notebooks/ANM_2020_PythonIntro3.ipynb): conditional statements, loops, vectorization and function handles; 
4. [Part 4/4](intro-python/notebooks/ANM_2020_PythonIntro4.ipynb): non-linear systems, ordinary differential equations, partial differential equations, data and optimization

References: 
1. [Python Tutorials](https://docs.python.org/dev/tutorial/index.html) (need to select appropriate parts)
2. [Numpy Fundamentals](https://numpy.org/doc/stable/user/basics.html) (ask TU Delft students to prepare talks on ndarrays, broadcasting, ufunc?)
3. [Scipy Users Guide](https://scipy.github.io/devdocs/tutorial/index.html#user-guide) (need to select appropriate parts) 
4. [scipy-lectures.org](https://scipy-lectures.org)

Extend with: 
1. NumPy uses C-order indexing. That means that the last index usually represents the most rapidly changing memory location, unlike Fortran, where the first index represents the most rapidly changing location in memory. This difference represents a great potential for confusion.
2. NumPy uses particular rules for broadcasting. Some documentation is [here](https://numpy.org/doc/stable/reference/generated/numpy.broadcast.html?highlight=broadcast#numpy.broadcast); more documentation is required;  
3. more information on what function for (non-)linear systems, ODE and PDE does;

## Section 4/: HW1: Recap/Intro of Prerequisites in Various Parts

See notebook [Recap/Intro of Prerequisites](homework1/notebooks/HW1-intro.ipynb). 

## Section 5/: HW2: Solving Reaction-Diffusion Systems in Pursuit of Turing Patterns (with Bijoy Bera in PDC Course)

See notebook [HW2-pde-reaction-diffusion](homework2/notebooks/HW2-pde-reaction-diffusion.ipynb). 

Help in developing this assignment: Shruti Shruti (TA financed by EEMCS Faculty) 

Tentative deadline for students to hand-in their assignment: October 30th; 

## Section 6/: HW3: Solving the Poisson-Boltzmann Equation  (with Valeria Gabin and Pouyan Boukany in MTP Course)

See notebook [HW3-Poisson-Boltzmann Equation  (with Valeria Gabin and Pouyan Boukany in MTP Course)](homework3/notebooks/HW3-poisson-boltzmann.ipynb)

Help in developing this assignment: Abhimanyu Bharade (TA financed by EEMCS Faculty)

Tentative deadline for students to hand-in their assignment: November 30th; 

## Section 7/: HW4: Assignment on Applied Transport Phenomena (Tom and Alina)

See [notebook](homework4/notebooks/HW4-applied-transport-phenomena.ipynb). 

## Section 8/: HW5: Assignment on Reactors and Kinectics (van Ommen) 

See notebook [Assignment on Reactors and Kinectics (dialogue with Ruud van Ommen)](homework5/notebooks/HW5-ode-reactors.ipynb)

Help in developing this assignment: Marc Caballero Megia (TA financed by EEMCS Faculty)


## Section 9/: HW6: Assignment on Engineering Thermodynamics (Anna Smith)

See [notebook](homework6/notebooks/HW6-engineering-thermodynamics.ipynb).

## Section 10/: HW7: Assignment on  Colloids and Interfaces (Laura and Monique)

More later: 

References:
1. [wiki on colloid](https://en.wikipedia.org/wiki/Colloid)

## Sect 11/: HW8: Assignment on Organic Materials Engineering (Eduardo and Pouyan) 

Polymer physics, random walk, stochastic differential equations

References:

## Section 12/: HW9: Assignment on Inorganic Materials Engineering (Laurens Sibelles and Ferdinand Grozema) 

References on molecular dynamics simulations:
1. [Short (4.11 min) video giving overview of molecular dynamics](https://www.youtube.com/watch?v=lLFEqKl3sm4)
 Valuable as introductory material, nice voice, good content; 
2. [wiki page on molecular dynamics containing simulations](https://en.wikipedia.org/wiki/Molecular_dynamics)
3. [Tutorial in implementing MD simulations in Python](https://klyshko.github.io/teaching/2019-03-01-teaching)
4. [Molecular Dynamics using openmm.py](https://openmm.org) good content; 
5. [mdanalysis](https://www.mdanalysis.org)
6. [Molecular Dynamics using Molly.jl](https://juliamolsim.github.io/Molly.jl/stable/)
7. Molecular Dynamics simulations for protein-folding: nice stuff! [ProtoSyn.jl code](https://github.com/sergio-santos-group/ProtoSyn.jl) (the list of 14 examples are potentially interesting to look into) and [Short (3.54 min) ProtoSyn video](https://www.youtube.com/watch?v=Z02zw8H-HQc)
8. [(Advanced) Poster Presentation Julia software development for MD simulation](https://www.youtube.com/watch?v=wPRgd0mfwyM)


References on quantum thermodynamic simulations 
1. [Quantum Thermodynamics using Fermi.jl](https://github.com/FermiQC/Fermi.jl)

## Section 13/: HW10: Assignment on Machine Learning by Artur 

Assignment by Artur on machine learning. To be detailed later. 

References
1. [Chapter Introduction to Machine Learning](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter25.00-Introduction-to-Machine-Learning.html)
2. [wiki on neural network with valuable schematic](https://en.wikipedia.org/wiki/Neural_network) 
3. [wiki on artificial neural network with broad overview](https://en.wikipedia.org/wiki/Artificial_neural_network#Practical_counterexamples)
4. [Video with history of neural networks](https://www.youtube.com/watch?v=GVsUOuSjvcg)
5. [RDKit is a collection of cheminformatics and machine-learning software written in C++ and Python](https://github.com/rdkit/rdkit)
6. [Overview Paper on Physics informed Neural Networks](https://arxiv.org/pdf/2201.05624.pdf) The part on ODEs might be valuable to us. 


## Section 14/: Our Favorites 
1. Linear solvers and sparse matrices;
2. FFT of Heart Rate Signals; 
3. Growth Model;
4. SVD decomposition applied to images [tutorial](https://numpy.org/numpy-tutorials/content/tutorial-svd.html); 
5. Matrix-Free implementation of the Laplacian for use inside non-linear iteration [tutorial](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.root.html);  


```julia

```


```julia

```


```julia

```
