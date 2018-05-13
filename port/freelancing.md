# Freelancing

## Continuous optimization and solution of a system of 36 ODEs

This one was one of the first projects I took as a freelancer. The problem was to solve a system of 36 ODES 
and minimize a determinant composed of some of the solutions ```y_i(x)```. I used the odeint() python algorithm to solve the system and
minimize() to find the minimum of the determinant. Both functions were from the SciPy library. Because the function to be minimized ended up
to be a function of six variables (s, a, R, n, m, T), we used a bisection method for the temperature T to simplify the problem. See the project [here](https://github.com/mlliarm/pythonscience).

## End of the World Population

In this project we were asked to plot various data on Mathematica that show the projection of the world population in the many years to come. See the project [here](https://bitbucket.org/bit_from_it/theendoftheworldpop/)

