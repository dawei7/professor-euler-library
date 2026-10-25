# 07 Linear Algebra Done Right

License: CC BY-NC 4.0 · Source: <https://linear.axler.net/> · 404 pages, 732 exercises in the prepared bundle

*Sheldon Axler*

## What this book trains

Sheldon Axler’s Linear Algebra Done Right is the second linear algebra course, and it starts from the linear map rather than from the matrix. A vector space is the object. A linear map is a structure-preserving function. A matrix appears only after bases are chosen, as a way to compute. Eigenvalues, inner products and the spectral theorem are the summit: a self-adjoint operator is diagonal in some orthonormal basis.

Determinants are postponed until the last chapter, after bilinear forms, alternating multilinear forms, and the trace. The book can reach diagonalization, the minimal polynomial, upper-triangular forms, positive operators, isometries, the singular value decomposition and the generalized eigenspace decomposition without making a determinant the definition of anything. Polynomials get a chapter of their own, because the minimal polynomial and the characteristic polynomial are polynomials in the operator.

## Why it is worth knowing

The spectral theorem is why principal axes exist. A quadratic form, a covariance, a Hessian at a critical point: each is a self-adjoint operator in disguise, and the theorem says there is an orthonormal basis of eigenvectors. The singular value decomposition does the analogous job for a map between two different inner product spaces. It says which directions are stretched, and by how much. That is the linear version of “which features survive”.

The pleasure of this book is the order. Hefferon showed you the computations, including Jordan form and determinants in the middle of the story. Axler asks you to forget the formula and watch the operator. Duality, quotients, and the vector space of all linear maps are the abstract rooms that make later functional analysis feel like the same subject in infinite dimensions. The trace, appearing as a connection between matrices and operators, is independent of the basis. That invariance is the sort of fact the book is built to reveal.

## What it asks of the other books

Hefferon (03) first. Row reduction, bases, and the concrete meaning of a matrix should already be in your hands. This book will not drill Gaussian elimination, and it will feel unmotivated if a linear system is still new. Calculus Volume 3 (06) is the other predecessor the paths use: once the derivative in several variables has been a matrix, an operator is the right next noun. Polynomials from the entry algebra, and the complex numbers, matter because the deepest decomposition theorems prefer an algebraically closed scalar field.

Rodríguez’s functional analysis (20) is the infinite-dimensional sequel. Suh (24) and Prince (28) use the spectral theorem and the singular value decomposition as working tools. You can read Axler before those books and after Hefferon. Measure theory is not required.

## A walk through the chapters

### 1. Vector Spaces

Vector Spaces. ℝⁿ and ℂⁿ, the definition of a vector space, and subspaces. The familiar coordinate spaces are examples, not the definition. A subspace is a subset that is itself a vector space under the same operations.

### 2. Finite-Dimensional Vector Spaces

Finite-Dimensional Vector Spaces. Span and linear independence, bases, and dimension. Every basis has the same number of vectors. That number is the dimension. The proofs are the ones Hefferon also owns. Meeting them a second time, with less matrix arithmetic in the way, is the point.

### 3. Linear Maps

Linear Maps. The vector space of linear maps, null spaces and ranges, matrices, invertibility and isomorphisms, products and quotients of vector spaces, and duality. The rank–nullity theorem lives here. A quotient space collapses a subspace to zero. The dual space is the space of linear functionals. Both constructions return in manifold theory and in functional analysis, and both are already finite-dimensional here.

### 4. Polynomials

Polynomials is a short, necessary pause. An operator applied to a polynomial in itself is the language of the next chapter. The algebra of polynomials, roots and factorization, is what the minimal polynomial will use.

### 5. Eigenvalues and Eigenvectors

Eigenvalues and Eigenvectors. Invariant subspaces, the minimal polynomial, upper-triangular matrices, diagonalizable operators, and commuting operators. An invariant subspace is one the operator maps into itself. Over the complex numbers, an operator has an upper-triangular matrix in some basis. Diagonalizable operators are the ones with a basis of eigenvectors. Commuting operators can be triangularized together, which is the linear-algebraic form of “simultaneously measurable”.

### 6. Inner Product Spaces

Inner Product Spaces. Inner products and norms, orthonormal bases, and orthogonal complements and minimization problems. An inner product is what makes length and angle legal. An orthonormal basis makes the coordinates the inner products against the basis vectors. The minimization problem is projection: the nearest point in a subspace is the orthogonal projection. Least squares is this theorem.

### 7. Operators on Inner Product Spaces

Operators on Inner Product Spaces. Self-adjoint and normal operators, the spectral theorem, positive operators, isometries and unitary operators and matrix factorization, the singular value decomposition, and its consequences. The spectral theorem is the chapter’s prize. A positive operator has nonnegative eigenvalues and a square root. An isometry preserves norms. The singular value decomposition factors a general linear map into a rotation, a stretch along axes, and another rotation.

### 8. Operators on Complex Vector Spaces

Operators on Complex Vector Spaces. Generalized eigenvectors and nilpotent operators, the generalized eigenspace decomposition, its consequences, and the trace. This is Axler’s replacement for a early Jordan-form chapter. A nilpotent operator is one some power of which is zero. The generalized eigenspaces put the operator into a block form even when there are too few genuine eigenvectors. Hefferon’s Jordan chapter and this one describe the same phenomenon. Axler reaches it from the minimal polynomial.

### 9. Multilinear Algebra and Determinants

Multilinear Algebra and Determinants. Bilinear forms and quadratic forms, alternating multilinear forms, determinants, and tensor products. A determinant is the alternating multilinear form that is 1 on the identity, and it is zero exactly when the operator is not invertible. Quadratic forms are the functions whose polarization is a bilinear form, and the spectral theorem says they have principal axes. Tensor products are the construction that makes a space of two-variable objects out of two spaces. They arrive last, when the rest of the language can carry them.
