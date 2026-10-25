# 14 Tea Time Numerical Analysis

License: CC BY-SA 4.0 · Source: <https://raw.githubusercontent.com/lqbrin/tea-time-numerical/master/TeaTimeNumericalAnalysis.pdf> · 523 pages, 527 exercises in the prepared bundle

*Leon Q. Brin*

## What this book trains

Leon Q. Brin’s Tea Time Numerical Analysis, third edition, is what you do when a theorem guarantees a number you cannot write in closed form. Accuracy, Taylor polynomials, and the speed of a recursive procedure come first. Then root finding: bisection, fixed-point iteration, its order of convergence, Newton’s method, and roots of polynomials. Interpolation by Lagrange polynomials, Newton polynomials, osculating polynomials and splines. Numerical differentiation and integration, with undetermined coefficients, error analysis, composite rules and extrapolation. Ordinary differential equations by Taylor methods and Runge–Kutta methods, including adaptive step size.

The book is written to be computed. Octave and the accompanying code are part of the preface. The mathematics is the error, not the printout. Truncation error is the piece of the Taylor expansion you discarded. The order of a method is the power of the step size in that piece.

## Why it is worth knowing

A numerical method is a theorem about an approximation. Bisection is slow and almost unreasonably reliable, because the intermediate value theorem keeps a root inside the bracket. Newton’s method is fast when the derivative is nonzero and the start is close, and it can fail when those hypotheses fail. Knowing which fact you are using is the whole subject.

Interpolation is how a function known at finitely many points becomes a function you can evaluate. A spline is a piecewise polynomial that does not oscillate the way one global polynomial of high degree can. Composite integration and extrapolation, Richardson’s idea in this chapter, squeeze more accuracy out of a basic rule by combining step sizes. Adaptive Runge–Kutta spends small steps where the solution bends and large steps where it does not. That is the practical form of an error estimate. Johnson’s numerical methods (22) take the linear-algebra side of this craft further. This book is the first course, and it includes the differential equations.

## What it asks of the other books

Calculus Volumes 1 and 2 (02, 04), especially Taylor’s theorem, the intermediate value theorem, and integrals. Newton’s method already appeared in Volume 1. This book analyzes it. Lebl’s differential equations (13) supply the equations the last chapter discretizes, including the pendulum. Linear algebra from Hefferon (03) helps undetermined coefficients and the linear systems inside splines, and the book does not require Axler.

Analysis (10) turns “the error looks smaller” into a proved limit. You can compute before that course. You should read it before you trust an error bound’s hypotheses. The pure and applied paths both include this book. The AI path includes it because a computed gradient and a computed root are approximations with rates.

## A walk through the chapters

### 1. The front matter explains the course and how to obtain Octave and the code

The front matter explains the course and how to obtain Octave and the code. Preliminaries then set the language: accuracy, Taylor polynomials, speed, and recursive procedures. A Taylor polynomial is the approximation. The next term is the shape of the error. Speed, here, is how the work grows with the number of steps, the same growth-rate idea as in Levin, applied to a numerical process.

### 2. Root Finding

Root Finding. A root-finding challenge appears again at the start of interpolation, as motivation. Bisection, fixed-point iteration, the order of convergence of a fixed-point iteration, Newton’s method, more convergence diagrams, roots of polynomials, and bracketing. A fixed-point iteration rewrites an equation as x = g(x) and hopes the map g pulls points closer. The order says how fast. Newton’s method is the fixed-point iteration built from the tangent line, and its order is typically two, which is why the number of correct digits can double. Bracketing methods keep a sign change in hand so a root cannot slip out.

### 3. Interpolation, and More Interpolation

Interpolation, and More Interpolation. Lagrange polynomials, Newton polynomials, then osculating polynomials and splines. A Lagrange polynomial matches values. A Newton form makes adding a node cheap. An osculating polynomial also matches derivatives. A spline matches values and a chosen amount of smoothness with low-degree pieces. The challenge that opens the interpolation chapter is there to show why a root finder and an interpolant can serve each other.

### 4. Numerical Calculus

Numerical Calculus. Rudiments, undetermined coefficients, error analysis, composite integration, and extrapolation. Undetermined coefficients derive a differentiation or integration rule by asking a formula to be exact on polynomials up to a certain degree. The error analysis then uses the next Taylor term. A composite rule applies a basic rule on many small intervals. Extrapolation combines results at different step sizes to cancel the leading error.

### 5. Ordinary Differential Equations

Ordinary Differential Equations. The motion of a pendulum, Taylor methods, the foundations of Runge–Kutta methods, error analysis, and adaptive Runge–Kutta methods. A Taylor method differentiates the equation to get higher derivatives and steps with a Taylor polynomial. A Runge–Kutta method samples the slope several times inside one step and never forms those higher derivatives explicitly. The adaptive method uses the error estimate to choose the next step. The pendulum is the running example because its nonlinearity is honest and its small-angle version is the linear oscillator from the differential-equations course. Solutions and answers to selected exercises, the bibliography and the index close the book.
