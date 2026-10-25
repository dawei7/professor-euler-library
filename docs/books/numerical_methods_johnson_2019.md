# 22 Introduction to Numerical Methods

License: CC BY-NC-SA 4.0 · Source: <https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/> · 368 pages, 45 exercises in the prepared bundle

*Steven G. Johnson*

## What this book trains

Steven G. Johnson’s Introduction to Numerical Methods is the MIT 18.335 bundle: fourteen week summaries, a set of lecture notes, four homework assignments and a run of midterm examinations from several years. The subject is numerical linear algebra and the algorithms around it, with the error kept in view. Floating-point roundoff, backward stability of summation, conditioning, QR factorization instead of the normal equations, cache-aware and cache-oblivious matrix multiplication, eigenvalue algorithms, Krylov subspaces, sparse direct solvers, adjoint methods, optimization, Chebyshev approximation, quadrature and the fast Fourier transform.

A condition number is a property of the problem. A backward-stable algorithm computes the exact answer to a nearby problem. The notes on naive summation and on the equivalence of norms in finite dimension are there so those two sentences have proofs.

## Why it is worth knowing

Forming the normal equations for a least-squares problem squares the condition number. QR factorization, an orthonormal basis for the column space, avoids that squaring. That one comparison is worth the course for anyone who has ever solved a regression by the textbook formula and watched it fall apart. The power method keeps only the latest vector. A Krylov method keeps the whole history and looks for the best answer inside it. Arnoldi and Lanczos are that idea, and the notes include why restarting them is not a trivial change.

The fast Fourier transform is an O(N log N) way to compute a transform that looks like N² work. Gauss, the notes remind you, was already doing trigonometric interpolation of this family. Adjoint methods differentiate a long computation, a PDE solve or a recurrence, at a cost comparable to one extra solve rather than one solve per parameter. Optimization in the later weeks, Lagrange multipliers, derivative-free methods, quasi-Newton and the BFGS update, is the same subject Suh treats from the convex-model side. Johnson treats it as numerical analysis.

## What it asks of the other books

Hefferon (03) for elimination, least squares, orthogonality and eigenvalues. Axler (07) makes the spectral theorem and orthonormal bases the language of the symmetric eigenvalue problem. Brin’s Tea Time Numerical Analysis (14) is the first course in roots, interpolation and Runge–Kutta. This bundle assumes that taste and moves to linear algebra at scale. Calculus and Taylor’s theorem are used in the quadrature and approximation weeks.

The week-3 summary is a guest lecture by Christopher Rackauckas on differential-equation solver software. It sits in the bundle as software context. The analysis of a step method remains Brin’s and Lebl’s job. The numerical PDE course (23) uses the sparse linear algebra and the stability language these weeks practice.

## A walk through the chapters

### 1. The fourteen week summaries

The fourteen week summaries are the spine. Week 1 is the overview: performance, and the concerns that abstract mathematics does not count. Week 2 analyzes accumulated floating-point error. Week 3 is the guest lecture on modern differential-equation software. Week 4 is the normal equations, the squared condition number, and QR. Week 5 is cache-oblivious matrix multiplication. Week 6 begins the eigenproblem, including why a finite LU-style algorithm cannot be the whole story and how a Hessenberg factorization prepares a matrix. Week 7 is the power method and Krylov subspaces. Week 8 is preconditioning, a crude approximate inverse that clusters eigenvalues. Week 9 is sparse-direct factorization that tries to keep the factors sparse. Week 10 is adjoint methods for eigenproblems and recurrences. Week 11 returns to Lagrange multipliers. Week 12 is derivative-free optimization. Week 13 connects Clenshaw–Curtis quadrature and cosine series to Chebyshev polynomials, and the exponential accuracy of polynomial approximation for smooth functions on an interval. Week 14 is the discrete Fourier transform, aliasing, the discrete cosine transform, and spectral methods.

### 2. The separate lecture notes fill those weeks in

The separate lecture notes fill those weeks in. Newton’s method for square roots. The IEEE floating-point standard, and a note dispelling myths about floating-point arithmetic. Naive summation and the backward stability of recursive summation. Equivalence of norms in finite dimension. Gram–Schmidt, Householder reflectors and Givens rotations. Performance experiments with matrix multiplication, including a cache-oblivious experiment. The QR algorithm for real symmetric matrices, in two notes. Why restarting Arnoldi or Lanczos is not trivial. Sparse matrix storage. An overview of optimization, adjoint methods for a discretized PDE, adjoint methods for a recurrence, and the origin of the BFGS update. Numerical integration and the redemption of the trapezoidal rule, Fourier cosine series, the FFT, and a historical note that begins with Gauss in 1805. Four homework sets and midterm examinations from 2008 through 2019, with a gap at 2014 in the bundle’s outline, are the practice.
