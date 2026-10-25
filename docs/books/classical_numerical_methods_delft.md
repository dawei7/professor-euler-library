# C.03 Classical Numerical Methods in Scientific Computing

License: CC BY 4.0 · Source: <https://books.open.tudelft.nl/home/catalog/book/168> · 322 pages, 150 exercises in the prepared bundle

*Jos van Kan, Guus Segal, Fred Vermolen and Hans Kraaijevanger*

## What this book trains

Classical Numerical Methods in Scientific Computing, by Jos van Kan, Guus Segal, Fred Vermolen and Hans Kraaijevanger, is the optional connected treatment of finite differences, finite volumes, and the time-dependent heat and wave equations. A review of the mathematics, including the Poincaré inequality, a short course in partial differential equations, finite differences, finite volumes, nonlinear equations, the heat or diffusion equation, and the wave equation. The method of lines discretizes space and leaves a large system of ordinary differential equations in time. Consistency, stability and the CFL criterion are the tests a scheme has to pass.

The catalog is explicit that the body does not cover finite elements, and that a promotional description is not an inventory of the chapters. This companion follows the chapters that are there. It is optional. Speck (21) remains the analytic partial-differential-equations book, and the numerical-methods course (22) remains the numerical linear algebra.

## Why it is worth knowing

A scheme can approach the equation on paper as the mesh shrinks and still be useless, because a high-frequency mode of the discrete operator grows at every time step. The heat-equation chapter separates consistency of the spatial discretization from stability of the time integration. The wave-equation chapter adds dissipation, dispersion, and the CFL criterion: a time step that is too large relative to the mesh is a different problem, not a small error.

Finite volumes are built around a cell and a flux, which is why a conservation law sits naturally there. The chapter reaches the Stokes equations for incompressible flow. Finite differences are the stencil view, from a cable equation through a singularly perturbed problem to Poisson’s equation on a rectangle. Nonlinear equations are solved by Picard iteration and by Newton’s method in more than one variable. The Poincaré inequality in the review is the analytic fact that controls a function by its derivative under a boundary condition, and energy estimates in the later chapters depend on having such a fact available.

## What it asks of the other books

Lebl’s differential-equations book (13) for the ordinary theory, and Speck (21) for classification, boundary conditions, and the classical equations. Calculus in several variables (06). The numerical-methods course (22) for conditioning and for Newton’s method as a numerical idea. The numerical-PDE course (23) is the lecture-slide neighbor. This companion is the textbook-shaped version of that computational habit, and the learning-path guide shelves it beside book 23.

The license recorded in the catalog is CC BY 4.0. The companion is not required for any path.

## A walk through the chapters

### Chapters 1–2

The front matter is the title, copyright and contents. Chapter 1 reviews basic mathematical concepts: preliminaries, a statement of the book’s contents, building blocks for mathematical modeling, preliminaries from linear algebra, and the Poincaré inequality. Chapter 2 is a crash course in partial differential equations: classification, boundary and initial conditions, existence and uniqueness, and examples.

### Chapter 3. Finite difference methods

Chapter 3, Finite difference methods. The cable equation and simple extensions, singularly perturbed problems, Poisson’s equation on a rectangle, extended boundary conditions, a global error estimate, and boundary-fitted coordinates. Chapter 4, Finite volume methods. Heat transfer with a varying coefficient, the stationary diffusion equation in two dimensions, the Laplacian in general coordinates, two-component fields, and the Stokes equations for incompressible flow.

### Chapter 5. Non-linear equations

Chapter 5, Non-linear equations. Picard iteration, and Newton’s method in more dimensions. Chapter 6, The heat- or diffusion equation. A fundamental inequality, the method of lines, consistency of the spatial discretization, time integration, stability of the numerical integration, the accuracy of the time integration, and special difference methods for the heat equation. Chapter 7, The wave equation. A fundamental equality, the method of lines, numerical time integration, stability, total dissipation and dispersion, direct time integration of the second-order system, and the CFL criterion. The bibliography closes the book.
