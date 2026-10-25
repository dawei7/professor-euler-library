# C.04 Mathematics of Machine Learning

License: CC BY-NC-SA 4.0 · Source: <https://ocw.mit.edu/courses/18-657-mathematics-of-machine-learning-fall-2015/> · 248 pages, 12 exercises in the prepared bundle

*Philippe Rigollet*

## What this book trains

Philippe Rigollet’s Mathematics of Machine Learning is the MIT 18.657 lecture course from fall 2015, with three problem sets bound after the lectures. The notes are a statistical-learning course. They begin by saying what the course means by machine learning: how much data a given accuracy demands. Binary classification, a finite dictionary of rules, the effect of noise on excess risk, empirical risk minimization through VC dimension and Rademacher complexity, a general loss, and covering numbers with chaining occupy the first part. Convex relaxation, positive definite kernels, convex optimization, projected gradient descent and its convergence, and stochastic optimization occupy the second. Online learning, prediction with expert advice, a guest-style set of notes by Gábor Lugosi on structured experts, stochastic bandits, a lecture by Alexander Rakhlin on prediction of individual sequences, adversarial bandits, linear bandits, Blackwell approachability, and potential-based approachability occupy the third.

The course is optional and compact. Bach (29) is the longer path book. These lectures are the place to watch the same ideas arrive one meeting at a time.

## Why it is worth knowing

Excess risk splits the error of a learned rule into the error of the best rule in the class and the error of not having found it. Noise, in the binary model of these notes, is how close the regression function sits to one half. A finite dictionary makes the argument a union bound. VC dimension and Rademacher complexity are two ways to measure a class that is infinite. Covering numbers measure it by how many balls you need, and the chaining lecture turns those numbers into a bound. The lectures are short enough that you can see the measuring instrument change while the theorem’s shape stays put.

Projected gradient descent returns to a closed convex set after each step. One lecture proves a rate for a convex Lipschitz function on a set of bounded diameter. Stochastic optimization replaces the full gradient by a noisy one. Bandits are the problem in which you see only the loss of the action you chose. Approachability, Blackwell’s notion, extends a zero-sum game to vector payoffs: a convex set you can force the average payoff to approach. The notes record who Blackwell was, inside the mathematics rather than instead of it. The three problem sets ask you to do discriminant analysis, Rademacher complexity, and the algebra of positive definite kernels. They are problem sheets. The bundle’s outline does not present them as a solution manual.

## What it asks of the other books

Probability (08 or 25), linear algebra (07), and enough analysis to read a Lipschitz constant and a diameter. Suh (24) is the convex-optimization book in the curriculum. These lectures teach a slice of that subject themselves and name Boyd and Vandenberghe as further reading. Bach (29) is the systematic text. Prince (28) supplies models whose risk this course bounds. The learning-path guide shelves the course beside Bach.

Lecture 17 is Lugosi’s notes on online learning with structured experts. Lecture 19 is given by Alexander Rakhlin. The catalog records the course under CC BY-NC-SA 4.0. It is not required for any path.

## A walk through the chapters

### Lectures 1–7

The bundle lists the meetings as lectures, so the walk follows the notes’ own openings. Lecture 1 asks what machine learning means in this course and separates that question from a general tour of the field. Lecture 2 begins the statistical-learning part with binary classification. Lecture 3 learns with a finite dictionary and asks how the sample size must grow with the number of rules. Lecture 4 studies noise and the excess risk of the empirical risk minimizer. Lecture 5 finishes that analysis under a VC-dimension constraint and controls Rademacher complexity by shatter coefficients. Lecture 6 moves to a general loss function. Lecture 7 continues covering numbers, bounds conditional Rademacher averages, and brings in chaining.

### Lectures 8–14

Lecture 8 opens the convexity part: a convex relaxation of empirical risk minimization, because the original 0–1 objective is not convex. Lecture 9 continues with soft classifiers and convex surrogate losses, naming the hinge, exponential and logistic losses. Lecture 10 defines a positive definite kernel by symmetry and by positive definite Gram matrices. Lecture 11 is convex optimization for machine learning. Lecture 12 is projected gradient descent and projection onto a closed convex set. Lecture 13 proves a convergence rate. Lecture 14 is stochastic optimization.

### Lectures 15–23

Lecture 15 opens online learning: a sequence of predictions rather than one batch. Lecture 16 continues prediction with expert advice. Lecture 17 is Lugosi’s survey of online learning with structured experts. Lecture 18 is the stochastic multi-armed bandit. Lecture 19, by Alexander Rakhlin, is prediction of individual sequences. Lecture 20 is the adversarial bandit under limited feedback. Lecture 21 is linear bandits, the case where the loss is a linear function of the action. Lecture 22 is Blackwell’s approachability for vector losses. Lecture 23 is potential-based approachability, using a separating hyperplane to force the average payoff toward a convex set. Three problem sets follow, dated through that fall: discriminant analysis, Rademacher complexity, and kernels.
