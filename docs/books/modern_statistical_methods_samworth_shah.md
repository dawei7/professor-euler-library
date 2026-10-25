# 30 Modern Statistical Methods and Theory: An Introduction to Nonparametric and High-Dimensional Statistics

License: CC BY-NC-ND 4.0 · Source: <https://www.cambridge.org/core/books/modern-statistical-methods-and-theory/C172B2647EFDE563204D208B939D6E39> · 458 pages, 265 exercises in the prepared bundle

*Richard J. Samworth and Rajen D. Shah*

## What this book trains

Richard J. Samworth and Rajen D. Shah’s Modern Statistical Methods and Theory is an introduction to nonparametric and high-dimensional statistics. Ordinary least squares is the baseline. High-dimensional linear regression is what happens when the number of predictors is large enough that the baseline’s geometry fails. Kernel density estimation and nonparametric regression estimate a curve without naming a finite list of parameters. Reproducing kernel Hilbert spaces connect that estimation to the kernel machines of learning theory. Conditional independence, graphical models and causality ask which variables still speak to each other after the others are accounted for. Minimax lower bounds say how hard a problem is. Shape-constrained estimation uses a hypothesis such as monotonicity or convexity in place of a parametric formula.

The appendix collects mathematical background. The book is a recent treatment of finite-sample and high-dimensional theory, not a second copy of the classical inference text.

## Why it is worth knowing

In a thousand dimensions, distances concentrate and a covariance estimated entry by entry is a noisy object. A method that was honest in the plane can be false here unless it assumes sparsity, low rank, or some other structure that reduces the effective dimension. High-dimensional regression is that correction. The Lasso and its relatives, in spirit the sparse methods Bach also studies, are the procedures. This book’s job is the statistical guarantee: for whom, under what assumption, at what rate.

A kernel density estimator is a smoothed histogram whose bandwidth is a theorem as much as a knob. Too small, and the estimate follows noise. Too large, and it erases the shape. Minimax lower bounds certify that a rate is not an accident of one algorithm. Shape constraints are the cheerful alternative to kernels: if you know a density is decreasing, or a regression is convex, the constraint itself regularizes. Graphical models draw conditional independence as a missing edge. Causality is treated as a claim beyond conditional independence, with assumptions the chapter is responsible for stating.

## What it asks of the other books

The inference book (26) for estimation, testing and the low-dimensional baseline. Polyanskiy (25) for measure-theoretic probability. Axler (07) and the measure book’s Hilbert-space chapters (19) for the reproducing-kernel geometry. Modern statistics (09) for the pictures of regression this book complicates. Bach (29) for the learning-theoretic side of kernels, sparsity and lower bounds. The two books meet. They are not duplicates.

Vershynin’s High-Dimensional Probability, in the personal-download notes, is the concentration toolkit beside this book. It does not replace it. The AI path places Samworth and Shah last.

## A walk through the chapters

### Chapters 1–2

The front matter is the cover, half-title, endorsements, series page, title, copyright, contents and acknowledgements. Chapter 1 is the introduction. Chapter 2, Linear models and ordinary least squares, is the review of the estimator you already know, so the later chapters can say exactly what fails when the design is no longer a comfortable rectangle.

### Chapter 3. High-dimensional linear regression

Chapter 3, High-dimensional linear regression, is the sparse and regularized theory. Chapter 4, Kernel density estimation, and Chapter 5, Nonparametric regression, are estimation of functions. Chapter 6, Reproducing kernel Hilbert spaces and kernel machines, is the Hilbert space in which a kernel method is a linear method. The representer theorem, in this circle of ideas, says the solution lives in the span of the kernel sections at the sample points. The chapter is where that geometry is earned.

### Chapter 7. Conditional independence, graphical models and causality

Chapter 7, Conditional independence, graphical models and causality. An edge means a dependence that survives conditioning. A causal claim is a further sentence, and the chapter’s value is the distinction. Chapter 8, Minimax lower bounds, is the information-theoretic floor. Chapter 9, Shape-constrained estimation, uses monotonicity, convexity and their relatives as the model. The appendix is mathematical background. References and the index close the book.
