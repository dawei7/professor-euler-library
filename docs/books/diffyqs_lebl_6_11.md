# 13 Notes on Diffy Qs: Differential Equations for Engineers

License: CC BY-SA 4.0 · Source: <https://www.jirka.org/diffyqs/diffyqs.pdf> · 709 pages, 747 exercises in the prepared bundle

*Jiří Lebl*

## What this book trains

Jiří Lebl’s Notes on Diffy Qs treats differential equations as calculus plus linear algebra. A first-order equation can be separable, linear, exact, or autonomous. A higher-order linear equation has a vector space of solutions whose dimension equals the order. A system is a vector equation, solved by eigenvalues when the coefficients are constant, and by a matrix exponential in general. Forcing, resonance, and the Laplace transform are ways to handle a nonzero right-hand side.

The book then leaves ordinary equations. Fourier series, separation of variables, the heat equation, the wave equation, D’Alembert’s formula, the Laplacian and the Dirichlet problem on a disk. Sturm–Liouville problems explain why those Fourier expansions exist. Nonlinear systems introduce equilibria, linearization, limit cycles and chaos. A final chapter reviews the linear algebra the course spent.

## Why it is worth knowing

An ordinary differential equation is a model of change that depends on the present state. The logistic equation, mechanical vibrations, and a pendulum are the same grammar with different forces. Resonance is the warning that a forcing term at a natural frequency does not produce a bounded oscillation of the usual kind. The Laplace transform turns a differential equation into algebra, and a convolution turns an impulse response into the response to any input.

Partial differential equations in this book are the first time a function of space and time is the unknown. The heat equation diffuses. The wave equation propagates. The Laplace equation describes a steady state. Separation of variables is the method that turns each of them into ordinary equations and a series. Speck’s course is the deeper study of those equations. This book is where their shapes become familiar. Picard’s existence theorem, if you have met it in Lebl’s analysis, is the reason a respectable equation has a solution even when you cannot write it down. Euler’s method, in the first-order chapter, is what you do instead of a formula.

## What it asks of the other books

Calculus Volumes 1 and 2 (02, 04) for derivatives, integrals, series and the short differential-equations chapter of Volume 2. Volume 3 (06) for partial derivatives and for the second-order equations it already sketched. Hefferon (03) for eigenvalues, determinants and the shape general = particular + homogeneous. The book’s own linear-algebra chapter reviews vectors, matrices, elimination, subspaces, dimension, kernel, inner products, projections and determinants. Use it as a repair, not as a first linear algebra course.

Axler (07) makes the eigenvalue method and the inner-product remarks cleaner, and it can come before or after. Tea Time Numerical Analysis (14) takes Euler’s method and Runge–Kutta seriously. Speck (21) takes the heat, wave and Laplace equations seriously. Fourier series here prepare both.

## A walk through the chapters

### 1. Introduction, and First-order equations

Introduction, and First-order equations. Classification, integrals as solutions, slope fields, separable equations, linear equations and the integrating factor, substitution, autonomous equations, Euler’s method, exact equations, and a first look at first-order linear partial differential equations. An autonomous equation is one in which time does not appear explicitly, so the phase line is a complete picture. Exact equations are those that are the derivative of a hidden function of two variables. Euler’s method steps along the slope field. Its error is the reason a numerical course exists.

### 2. Higher-order linear ODEs

Higher-order linear ODEs. Second-order and higher-order equations, constant coefficients, mechanical vibrations, nonhomogeneous equations, and forced oscillations and resonance. The characteristic polynomial turns a constant-coefficient equation into algebra. A repeated root produces a factor of t in the solution. Resonance is the case in which the forcing solves the homogeneous equation, and the particular solution has to be sought in a larger family.

### 3. Systems of ODEs

Systems of ODEs. Matrices and linear systems, the eigenvalue method, two-dimensional vector fields, second-order systems and applications, repeated eigenvalues, matrix exponentials, and nonhomogeneous systems. A first-order system in several unknowns is the natural home of a higher-order equation: one variable for the quantity, another for its velocity. The matrix exponential solves the constant-coefficient system even when the matrix is not diagonalizable. Repeated eigenvalues are that case.

### 4. Fourier series and PDEs

Fourier series and PDEs. Boundary value problems, trigonometric series, sine and cosine series, the heat equation by separation of variables, the one-dimensional wave equation, D’Alembert’s solution, steady state temperature and the Laplacian, and the Dirichlet problem in the circle with the Poisson kernel. A Fourier series writes a function as a sum of harmonics. The coefficients are inner products against those harmonics, which is why the linear-algebra chapter’s projection section belongs in the same book. The Poisson kernel solves the steady temperature problem on a disk by an integral.

### 5. More on eigenvalue problems

More on eigenvalue problems. Sturm–Liouville problems, higher-order eigenvalue problems, and steady periodic solutions. A Sturm–Liouville problem is the abstract form of the boundary-value problems that produced sines and cosines. Its eigenfunctions are orthogonal. That is the theorem that makes the expansions legitimate.

### 6. The Laplace transform

The Laplace transform. The transform, transforms of derivatives, convolution, the Dirac delta and impulse response, and solving partial differential equations with the transform. Differentiation becomes multiplication by the variable. A convolution becomes a product. The delta is the input whose response is the kernel you convolve with everything else.

### 7. Power-series methods

Power-series methods. Power series, series solutions of linear second-order equations, and singular points with the method of Frobenius. This is Volume 2’s power series used as a solution method, including at points where the coefficients blow up and an ordinary series is not enough.

### 8. Nonlinear systems

Nonlinear systems. Linearization, critical points and equilibria, stability and classification of isolated critical points, applications, limit cycles, and chaos. Linearization replaces a nonlinear field by its derivative at an equilibrium, a matrix, and reads stability from eigenvalues. A limit cycle is a closed orbit that nearby trajectories approach. Chaos is the chapter’s honest announcement that a deterministic equation can be unpredictable in practice. The linear-algebra review closes the book.
