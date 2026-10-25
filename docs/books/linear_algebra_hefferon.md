# 03 Linear Algebra

License: CC BY-SA 3.0 US · Source: <https://hefferon.net/linearalgebra/> · 929 pages, 1026 exercises in the prepared bundle

*Jim Hefferon*

## What this book trains

Jim Hefferon’s Linear Algebra is the concrete theory of linear systems, vector spaces and linear maps. A system of equations becomes a set of solutions with a shape: a particular solution plus the solutions of the homogeneous system. A vector space is any set with addition and scalar multiplication obeying the familiar rules. A linear map is a function that respects those operations. A matrix is the table of a linear map after bases have been chosen.

You compute, and the computation is the point of this first course. Gaussian elimination, Gauss–Jordan reduction, bases, dimension, matrix multiplication, inverses, change of basis, Gram–Schmidt orthogonalization, projections, determinants, eigenvalues, diagonalizability, and the Jordan canonical form. Topics scattered through the chapters show the same tools at work: input–output analysis, networks, the line of best fit, Markov chains, page ranking, coupled oscillators.

Determinants are size functions, built from their properties and from the permutation expansion, not a mysterious formula. Eigenvalues are the scalars for which a map sends some nonzero vector to a multiple of itself. When a basis of such vectors exists, the matrix becomes diagonal and the powers of the matrix become easy. That is the computational heart of recurrence, of a Markov chain’s long run, and of a system of linear differential equations.

## Why it is worth knowing

Linear algebra is the language of every discrete model and of every linear approximation. A finite-difference scheme is a matrix. A data matrix has a column space. A covariance is a matrix. Hefferon is where those sentences become operations you can carry out by hand and then trust a computer to repeat.

The joy is structural. Dimension is a well-defined number: every basis of a space has the same length. The rank–nullity idea, range and null space, says what a map preserves and what it kills. Gram–Schmidt turns any basis of an inner-product space into an orthogonal one, which is why projections and least squares have formulas. Jordan form says that even a matrix which cannot be diagonalized has a nearly diagonal shape, built from blocks. Axler’s second course will tell this story again from the operator’s point of view and will postpone determinants. Hefferon tells it with the computations visible.

## What it asks of the other books

Algebra from Wallace (S.01) and the linear systems, matrices and vectors in Stitz–Zeager (S.04). Those sections are a preview. This book is the course. Calculus Volume 1 (02) is the curriculum’s neighbor, not a logical prerequisite for Gaussian elimination. Reading it first helps, because linear approximation and rates make the question “why a linear map?” feel earned. Geometry (S.02) helps length and angle feel familiar.

Axler’s Linear Algebra Done Right (07) is the second course, best after this one and after several-variable calculus. Calculus Volume 3 (06) uses vectors, dot products and cross products in its own way. Differential equations (13) use the fact that the solution set of a linear equation is a vector space. Suh’s optimization (24) uses positive semidefinite matrices and projections. The topic Line of Best Fit is the first least squares.

## A walk through the chapters

### 1. Linear Systems

Linear Systems. Gauss’s method, describing the solution set, the decomposition general = particular + homogeneous, vectors in space, length and angle, Gauss–Jordan reduction, and the linear combination lemma. The topic sections on computer algebra, input–output analysis, accuracy of computations, and networks are worth reading as applications, not as optional decoration. Accuracy of computations is the first hint of conditioning: a computed answer can be the right answer to a slightly wrong question.

### 2. Vector Spaces

Vector Spaces. The definition and examples, subspaces and spanning sets, linear independence, basis, dimension, the relationship with linear systems, and combining subspaces. The topics on fields, crystals, voting paradoxes and dimensional analysis show how far the axioms reach. A field is the scalar system. The real numbers are the usual choice. The complex numbers are the other one this book prepares, because eigenvalues would rather live there.

### 3. Maps Between Spaces

Maps Between Spaces. Isomorphisms, the fact that dimension characterizes isomorphism for finite-dimensional spaces, homomorphisms, range and null space, representing maps by matrices and conversely, matrix arithmetic and multiplication, inverses, changing the representation of a vector and of a map, orthogonal projection onto a line, Gram–Schmidt, and projection onto a subspace. The topics include the line of best fit, the geometry of linear maps, magic squares, Markov chains, and orthonormal matrices. Change of basis is the idea that will not go away: the map is the object, the matrix is a photograph of it in a chosen frame.

### 4. Determinants

Determinants. Exploration and definition, properties, the permutation expansion, existence, determinants as size functions, and Laplace’s expansion. Topics: Cramer’s rule, the speed of calculation, Chiò’s method, projective geometry, and computer graphics. A determinant is zero exactly when the map is not invertible, and its absolute value scales volume. Cramer’s rule is a beautiful formula and a poor algorithm. The section on speed says so.

### 5. Similarity and Eigenvalues

Similarity and Eigenvalues. Complex vector spaces, similarity, diagonalizability, eigenvalues and eigenvectors, nilpotence as self-composition and as strings, polynomials of maps and matrices, and the Jordan canonical form. Topics: the method of powers, stable populations, page ranking, linear recurrences, and coupled oscillators. Similarity means two matrices represent the same map in different bases. A diagonal form is the best photograph. Jordan form is the next best, and nilpotent blocks are why it sometimes cannot be diagonal. Page ranking and population models are powers of a matrix, which is why a good basis is worth the search.
