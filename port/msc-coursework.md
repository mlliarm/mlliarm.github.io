# MSc coursework

## MSc thesis

My thesis was in Active Machine Learning using JCLAL to run the experiments. In this 
project I did an empirical study of the Active Learning framework, using 16 datasets from the
UCI repository, 5 learning algorithms (Naive Bayes, Support Vector Machines, Random Forest, Decision Tree,
k-NN) and 5 active learning strategies (Random sampling, Least Confident Sampling, Margin Sampling, Entropy Sampling, Query by Commitee with Vote Entropy,
Query by Commitee with Kullback-Leibler, Passive learning).

Apart from presenting the active learning framework and the library JCLAL, we had three questions that we attempted to answer empirically. The first question was if active learning was better than passive learning (i.e. the usual supervised methods where the learner uses the whole training dataset). The second question was if the strategies that are in the core of the active learning framework performed better than the Random sampling Strategy. The third question was to find which combination of strategy and learning algorithm gave the best results in the given datasets.

After doing a statistical analysis (Friedman) of the scores we saw that in three out of five learning algorithms the strategy of Entropy Sampling was the best, whereas in the other two, the strategy of the Least Confident Sampling. Also, in all five cases of learning algorithms, we've shown that at least one active learning strategy performed better than Random Sampling. Finally, we've shown that all active learning strategies did better than passive learning.

You can find the thesis (in Greek) [here](https://drive.google.com/open?id=1B5tJi_w1PEKgAVI8IJjTBpvtqOOt_rvU) and the code needed to run the experiments [here](https://bitbucket.org/milia/thesis-experiments/).

## Numerical Optimization with SciPy

Me and my collaborator did a benchmark on some of the algorithms of unconstrained optimization included in SciPy. Namely, BFGS, Powell, Newton-CG, CG (Conjugate Gradient), Nelder-Mead and Basin-hopping. Our main conclusion was that derivative free methods (as BFGS or basinhopping) are more reliable, in contrast to Newton and Quasi-Newton methods. Link to project [here](https://github.com/mlliarm/numerical-optimization) and link to the report [here](https://drive.google.com/file/d/0B4ai-gEVsMLlYThlMWVUYjROajA/view?usp=drive_link&resourcekey=0-PslTmDWDkF6s4MQ8pdg8dw) (in Greek).

## The Interval Slope method

In this project me and my collaborator translated and presented an important paper of D. Ratz, "A Nonsmooth Global Optimization Technique Using Slopes: The One-Dimensional Case" ([DOI](https://link.springer.com/article/10.1023/A:1008391326993)). The key idea of the paper was that it presented an interval analysis algorithm for the optimization of smooth and non-smooth function. The paper was improved so that all equations were aligned with the interval analysis formulation. That is, if we found an inequality of the form ```a < x < c```, we'd write it as ```x ∈ [a,c]```, where by ```[a,c]``` we meant the interval ```X``` with ```Xmin = a``` and ```Xmax = c```. Besides presenting the paper in Greek, simple algorithms of Interval Analysis such as the Interval Bisection method were implemented in Matlab (IntLab) and Mathematica (Intervalica). Link to the report [here](https://drive.google.com/file/d/0B4ai-gEVsMLleVRfdjU3ZExrR2s/view?usp=sharing&resourcekey=0-gL6T347Dzm5PGYWLgtaCyA) (pdf, in Greek).

## Intervalica

An Interval Analysis library in Mathematica. A basic library for Interval Analysis, by extending the interval capabilities provided by Mathematica. It already contains the Interval Bisection method.  What is left is to implement the Interval Newton method and the methods presented in Ratz's paper. [Here](https://drive.google.com/open?id=1Q9T3IQlI2rl88NcREeYyQRXz8zQa6OUY) you can find the User manual pdf and some examples of how the library works within Mathematica. Developmenet in pause.
