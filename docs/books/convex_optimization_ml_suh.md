# 24 Convex Optimization for Machine Learning

License: CC BY-NC 4.0 · Source: <https://www.emerald.com/books/oa-edited-volume/20740/Convex-Optimization-for-Machine-Learning> · 379 pages, 89 exercises in the prepared bundle

*Changho Suh*

## What this book trains

Changho Suh’s Convex Optimization for Machine Learning is a textbook, not a slide deck. A convex optimization problem is one whose objective and constraints bend the right way: a local minimum is a global minimum. The book defines that property, explains why convex problems are tractable, and teaches gradient descent as the basic algorithm. It then builds the standard cones of models. Linear programs, least squares, quadratic programs, second-order cone programs, and semidefinite programs, including relaxations that turn a hard combinatorial problem into a convex one you can actually solve.

Duality is the second chapter. Strong duality, the interior-point method, the proof of strong duality, weak duality, and Lagrange relaxation for Boolean problems and for MAXCUT. The third chapter spends the theory on learning: supervised learning as optimization, logistic regression, deep learning with a TensorFlow implementation, generative modeling, GANs and Wasserstein GANs, and fair classification, including a fair classifier whose formulation is connected to a GAN. Appendices teach the Python, CVXPY and TensorFlow used in the implementations.

## Why it is worth knowing

Convexity is a geometric gift. If the set of feasible points is convex and the objective is convex, you cannot get stuck in a bad valley that is only bad locally. Gradient descent, which in a deep network is only a local method, is a global method on the problems in the first two chapters. Duality turns a constraint into a price. The dual problem is often smaller, and a zero gap between primal and dual values is a certificate that you have the optimum. Weak duality always gives a bound. Strong duality is the theorem that says the bound is tight, and the book proves it rather than quoting a solver.

MAXCUT is the delightful example. Cutting a graph to maximize the weight of severed edges is hard. A semidefinite relaxation is convex, solvable, and famous for how close it gets. Least squares appears again, now with test error, regularization, and a computed-tomography application. Fairness appears as an optimization constraint, not as a slogan. The Wasserstein GAN lectures are the point where a distance between probability distributions becomes the loss.

## What it asks of the other books

Calculus Volume 3 (06) for gradients and Lagrange multipliers in the classical setting. Hefferon (03) and Axler (07) for positive semidefinite matrices, eigenvalues and projections. Probability (08) helps the learning chapter’s losses. Analysis is what makes a convergence proof feel like a proof. The applied path places this book after functional analysis and immediately before the numerical PDE course. The AI path places it after Gallager and immediately before Prince, so that gradient descent and duality are already mathematics when a network appears.

Boyd and Vandenberghe’s Convex Optimization, named in the path’s personal-download notes, is the fuller reference beside this book. Suh remains the curriculum’s optimization book. Prince (28) uses the deep-learning sections as a preview and then studies architectures. Bach (29) studies the optimization–approximation–generalization split that a solver cannot see by itself.

## A walk through the chapters

### Chapter 1. Convex Optimization Basics

Chapter 1, Convex Optimization Basics. An overview, the definition, tractability and gradient descent, then linear programs: examples, relaxation, algorithms, and a CVXPY implementation. Least squares: test error, regularization, CVXPY, and computed tomography. Quadratic programs, second-order cone programs, semidefinite programs and semidefinite relaxation. Problem sets sit inside the chapter, after the blocks of sections. A linear program has a linear objective and linear constraints. A semidefinite program has a matrix unknown that must stay positive semidefinite. The relaxation is how a 0–1 choice becomes a matrix constraint you can hand to a solver.

### Chapter 2. Duality

Chapter 2, Duality. Strong duality and the interior-point method, the proof of strong duality in two sections, weak duality, and Lagrange relaxation for Boolean problems and for MAXCUT. Interior-point methods walk through the interior of the feasible set rather than along the vertices the simplex method prefers. The proof sections are the reason this is a mathematics book. MAXCUT is the section where the relaxation of Chapter 1 meets a famous graph problem.

### Chapter 3. Machine Learning Applications

Chapter 3, Machine Learning Applications. Supervised learning as optimization, logistic regression, three sections of deep learning including a TensorFlow implementation, unsupervised generative modeling, GANs and their implementation, two sections of Wasserstein GAN and an implementation, and fair machine learning: a fair classifier, its connection to GANs, and an implementation. Logistic regression is the convex classification model. A deep network in this chapter is a composition whose training is the optimization you already defined, demonstrated in code. The Wasserstein distance is a cost of moving probability mass. Fairness is written as a constraint the dual can price.

### 4. Chapter A, Python and Jupyter, Chapter B, CVXPY, and Chapter C, TensorFlow and Keras

Chapter A, Python and Jupyter, Chapter B, CVXPY, and Chapter C, TensorFlow and Keras, are manuals for the implementations, not a second theory. References, the index and a note about the author close the book.
