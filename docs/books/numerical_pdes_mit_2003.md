# 23 Numerical Methods for Partial Differential Equations

License: CC BY-NC-SA 4.0 · Source: <https://ocw.mit.edu/courses/16-920j-numerical-methods-for-partial-differential-equations-sma-5212-spring-2003/> · 1352 pages, 10 exercises in the prepared bundle

*Khoo, White, Peraire and Patera*

## What this book trains

Numerical Methods for Partial Differential Equations, the MIT notes associated with Khoo, White, Peraire and Patera, is a long bundle of lecture slides and four problem sets. Much of the slide text is stored as images, so the outline’s lecture numbers are the reliable table of contents, and only some title slides yield their words to a text search. What those readable pages actually teach is finite-difference discretization and its stability, and integral-equation methods.

The finite-difference lectures analyze a parabolic problem. A PDE is reduced to coupled ordinary differential equations, then to uncoupled modal equations by replacing the spatial operator with an eigenvalue. Absolute stability diagrams are drawn for leapfrog and for forward Euler. Backward Euler is the implicit march that stays stable for the parabolic sign. A problem set treats traffic flow as a nonlinear hyperbolic conservation law. The later readable block is integral equations: discretization of boundary integral equations, first-kind and second-kind Fredholm equations, Dirichlet and Neumann problems, the self-term in a singular integral, and the Stokes equations with a Krylov method modified to stay out of a null space.

## Why it is worth knowing

Stability is the new word, beside consistency. A consistent scheme can still blow up if the time step and the spatial step sit outside the region the stability diagram allows. Drawing that region for forward Euler on the heat equation, and seeing backward Euler remain stable because the eigenvalues of the spatial operator are real and negative, is the practical form of thirty pages of analysis. The traffic problem is the hyperbolic cousin: a density of cars obeying a nonlinear conservation law, the sort of shock Speck’s Burgers equation prepared.

Integral equations are the other joy. Instead of filling the volume with a grid, a boundary-integral method places the unknown on the surface. A second-kind equation has the unknown both under the integral and outside it, and the Fredholm alternative describes its null space. The Stokes system in the notes has a null space the Krylov iteration must be taught to ignore. Delft’s companion (C.03) teaches finite differences and finite volumes as a connected textbook. This bundle is the MIT lecture sequence, including the examinations’ style of problem set.

## What it asks of the other books

Speck (21) for the heat, Laplace and wave equations as continuous objects. Johnson (22) for conditioning, sparse linear algebra and Krylov subspaces. Hefferon (03) for eigenvalues of a discrete operator. Calculus Volume 3 (06) for the divergence theorem that boundary integrals restate. The curriculum places Suh’s convex optimization (24) just before this course on the applied path as breadth for constrained models. The finite-difference stability diagrams do not require duality. They require the PDE and the numerical linear algebra.

C.03 is the optional companion for additional finite-difference and finite-volume explanations. It does not replace these lectures, and these lectures do not replace its finite-volume chapter.

## A walk through the chapters

### Lectures 1–26

The outline runs from Lecture 1 through Lecture 26, with some meetings bound together and with Lecture 13–14 appearing twice, then four homework sets. Treat the lecture numbers as the contents list the bundle actually stores.

### 2. The readable finite-difference block, including the title slide of the lecture labeled Finite Differences: Parabolic Problems

The readable finite-difference block, including the title slide of the lecture labeled Finite Differences: Parabolic Problems, works through discretization, reduction of a one-dimensional PDE to coupled and then uncoupled ordinary differential equations, modal stability, leapfrog, forward Euler and backward Euler, and the absolute-stability regions in the complex plane. The same ideas reappear in the SMA-HPC slide sequence and in the 16.920J lecture numbering. Problem Set 1 is finite differences. A later problem poses traffic flow as a nonlinear hyperbolic equation for a density.

### 3. The readable integral-equation block

The readable integral-equation block begins with the title slide Discretization of Boundary Integral Equations. The notes construct potentials that satisfy Laplace’s equation, discuss first-kind and second-kind equations, the Fredholm alternative, Dirichlet and Neumann boundary conditions, the singular self-term, and a Krylov-subspace treatment of the Stokes null space. Problem Set 4 is integral equation methods.

### 4. Where a slide page does not yield a title as text, the honest guide

Where a slide page does not yield a title as text, the honest guide is the lecture number in the outline rather than a guessed topic. The homework is part of the course.
