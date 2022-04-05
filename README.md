# CH3133: Numerical Practicum 2022 - Current Overview

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

### Section 1.2/: In general 

- formative assessment during the course: to be defined; 
- summative assessment: via 6 homework assignments - no written exam any more - how to define retake? 
- auto-grading of the assignments using nb-grader and unit-tests (give information to the students); 

### Section 2.2/: Common to all Homework Assignments 

- Six assignments in total - 1 ECTS per assignment - 28 hours of work for students  
- in Q1: three compulsory assignments (no freedom of choice); 
- in Q2: possibly elective assignments (choice assignment corresponding to course); 
- foresee model for the grading of the homeworks; 

### Section 3.2/: Other arrangements to be made

- establish house rules for the course;
- establish Q&A for the course;
- Vocareum for auto-grading of the assignments;

### Section 4.2/: Asked Jolanda Quak to arrange 

#### Prior to the summer 2022  
1. notify TG that a book is no longer required; course will link to online resources instead; 
2. notify Osiris of wish to register two grades. The first (to two) grades is an intermediate grade (after 3 assignments at the end of Q1). The second (of two) grades is the final grade (after 6 assignments at the end of Q2). The first grade only serves for teaching staff to keep track of active participation in the course (thanks to Arno Hakket for providing this suggestion); 
3. notify campus-wide BrightSpace support about need for course pages and plug-in for Vocareum (see below);  

#### During summer 2022 
1. notify non-TU-Delft bachelor students about Python introduction to the course (see below); 

#### Introduction Days end of August 2022 
1. notify all students to enroll in course via BrightSpace; 
2. instruct students on how to navigate to Vocareum and Jupiter notebook for Python through Vocareum;  

## Section 3/: Software Instruments (needs revision)  

### Section 1.3/: Python 

#### Students should use Python and Jupyter notebook via Vocareum. 

Divide students in the following three groups: TU bachelor, entirely strange to Python and in between group. Define seperate tasks for the three groups. 

Introduction in Python programming in four parts. Used as reference for future parts of the course. (Encourage TU Delft bachelor students to give Part 4/4 a look?, how to provide opportunity to practice, how do other courses do so?)
1. [Part 1/4](intro-python/notebooks/ANM_2020_PythonIntro1.ipynb): introduction; operations of vectors and matrices; plotting; 
2. [Part 2/4](intro-python/notebooks/ANM_2020_PythonIntro2.ipynb): functions, particular matrices, matrix-vector operations, linear Systems and more plotting;
3. [Part 3/4](intro-python/notebooks/ANM_2020_PythonIntro3.ipynb): conditional statements, loops, vectorization and function handles; 
4. [Part 4/4](intro-python/notebooks/ANM_2020_PythonIntro4.ipynb): non-linear systems, ordinary differential equations, partial differential equations, data and optimization

#### External Courses 
1. [Harvard CS50 Week 6 Python](https://cs50.harvard.edu/college/2022/spring/weeks/6/) Elementary 
2. [Udemy Course](https://www.udemy.com/course/the-python-mega-course/?k_clickid=b80c91fd-6e49-4ad4-a74f-4dad023d04ad_124565424&utm_campaign=NEW-FB-PROS-TECH-ROW-LF-Dev-Python-EN-ALL_._ci_692188_._sl_ALL_._vi_TECH_._sd_All_._la_EN_.&utm_medium=udemyads&utm_source=facebook-row&utm_term=_._ag_NEW-FB-PROS-TECH-ROW-LF-Dev-Python-Affinity-EN-ALL_._ci_692188_._pi_1528203673886358_._gi_all_._ai_18--65_._an_hId26t)
3. Various level courses on Linked-Inn 

#### References: 
1. [Python Tutorials](https://docs.python.org/dev/tutorial/index.html) (need to select appropriate parts)
2. [Numpy Fundamentals](https://numpy.org/doc/stable/user/basics.html) (ask TU Delft students to prepare talks on ndarrays, broadcasting, ufunc?)
3. [Scipy Users Guide](https://scipy.github.io/devdocs/tutorial/index.html#user-guide) (need to select appropriate parts) 
4. [scipy-lectures.org](https://scipy-lectures.org)
5. [Hans Petter Langtangen, A Primer in Scientific Computing Using Python, PDF file, 900+ pages](https://hplgit.github.io/primer.html/doc/pub/half/book.pdf): Can we summarize? Can we find other examples? 

#### Extend with: 
1. NumPy uses C-order indexing. That means that the last index usually represents the most rapidly changing memory location, unlike Fortran, where the first index represents the most rapidly changing location in memory. This difference represents a great potential for confusion.
2. NumPy uses particular rules for broadcasting. Some documentation is [here](https://numpy.org/doc/stable/reference/generated/numpy.broadcast.html?highlight=broadcast#numpy.broadcast); more documentation is required;  
3. more information on what function for (non-)linear systems, ODE and PDE does;

#### Doubts on the use of Python in Computational Practicum for non-math/non-computer science master students 
1. When/how (in case at all) to raise awareness on how to code to obtain computational efficiency? How to discuss avoiding loops? How to vectorize code? What are good examples/practices/tools? What are pitfalls to avoid? 
2. When/how (in case at all) to address the two language problem, i.e., the fact that the bulk of the computations does not happen in Python, but rather in Fortran or C? (Examples are linear algebra, time stepping and FFT among many others). Do we teach Python initially to reveal the need to switch to non-Python later?   
3. When/how (in case at all) to address software development practises? When to introduce object-oriented programming?
4. When/how (in case at all) to address parallel computing architectures and/or large data sets? 

### Section 2.3/: Jupyter Notebook
- How to guide students into the use of [Jupyter notebooks](https://jupyter.org)? 
- How to guide TA in the use of [nb-grader](https://nbgrader.readthedocs.io/en/stable/)? Refer them to instructional videos by Gary Steele? 

### Section 3.3/: Vocareum 
Cloud computing. Support for online distribution notebooks and grade administration using [Vocareum](https://www.vocareum.com).
TEAMS has a Vocareum channel. Gary Steele has instructional videos on the use of Vocareum. 

### Section 4.3/: Not Python 
1. [Parallel Computing and Scientific Machine Learning (SciML): Methods and Applications](https://book.sciml.ai)


```julia

```

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
6. [Introduction to Scientific Programming and Machine Learning with Julia (SPMLJ)](https://github.com/sylvaticus/SPMLJ)
7. [Overview Paper on Physics informed Neural Networks](https://arxiv.org/pdf/2201.05624.pdf) The part on ODEs might be valuable to us. 


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
