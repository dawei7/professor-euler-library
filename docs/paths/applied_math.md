# Applied Mathematics

Turn a mathematical model into a calculation you can implement, test and explain. The useful skill is seeing how the error moves when the step size, the noise or the matrix changes.

**What you will learn**

A model is a mathematical sentence with assumptions you can point at. An ordinary differential equation says how a quantity changes with its present value. A partial differential equation says how it changes in space and time. A probabilistic model says which variations you are willing to call noise. You learn to write the sentence, name the hypothesis, and say what would falsify it.

Computation is part of the mathematics. Truncation error is the piece of the Taylor expansion you threw away. Rounding error is what finite precision does to a subtraction of nearly equal numbers. Conditioning is a property of the problem: a small change in the data can force a large change in the answer, and no algorithm escapes that. Stability is a property of the algorithm. Convergence is the theorem that the error goes to zero as the mesh, the step, or the iteration is refined.

Linear algebra is the language of every discrete model. A finite-difference scheme is a matrix. A linear differential equation has a vector space of solutions. A covariance is a positive semidefinite matrix, and a self-adjoint matrix can be diagonalized, which is why principal axes exist. Hefferon makes you compute. Axler tells you why the computation was about an operator.

Analysis is why the numerical story is a theorem. Completeness, continuity and the mean value theorem turn “the error looks smaller” into “the error is smaller”. Several variables and metric spaces make a mesh and a function space into objects you can talk about. Measure and the Lebesgue integral are what you need before an inner product on functions is honest. Functional analysis is linear algebra for those function spaces: norms, completeness, bounded operators.

Optimization and partial differential equations meet at constraints. A convex problem has no spurious local minima, duality explains the constraint, and a numerical method for a PDE asks how a continuous operator becomes a finite matrix you can store. The stochastic extension, if you take it, replaces a fixed equation by a process: probability built on measure, inference as a theorem about estimators, and dependence in time as a stochastic process.

### Foundation

Learn the language of models and data, solve ordinary differential equations, and build a first understanding of numerical error before returning to deeper analysis.

1. **01 — Book of Proof** — Richard Hammack
2. **02 — Calculus, Volume 1** — OpenStax
3. **03 — Linear Algebra** — Jim Hefferon
4. **04 — Calculus, Volume 2** — OpenStax
5. **06 — Calculus, Volume 3** — OpenStax
6. **08 — Introduction to Probability** — Charles Grinstead and J. Laurie Snell
7. **09 — Introduction to Modern Statistics** — Mine Çetinkaya-Rundel and Johanna Hardin
8. **13 — Notes on Diffy Qs: Differential Equations for Engineers** — Jiří Lebl
9. **14 — Tea Time Numerical Analysis** — Leon Q. Brin
10. **10 — Basic Analysis I: Introduction to Real Analysis, Volume I** — Jiří Lebl
11. **07 — Linear Algebra Done Right** — Sheldon Axler
12. **15 — Basic Analysis II: Introduction to Real Analysis, Volume II** — Jiří Lebl

### Advanced core

Connect PDE models, practical numerical computation, measure/integration, function spaces and optimization; then study numerical methods for PDEs.

1. **21 — Introduction to Partial Differential Equations** — Jared Speck
2. **22 — Introduction to Numerical Methods** — Steven G. Johnson
3. **19 — Measure, Integration & Real Analysis** — Sheldon Axler
4. **20 — Introduction to Functional Analysis** — Casey Rodriguez
5. **24 — Convex Optimization for Machine Learning** — Changho Suh
6. **23 — Numerical Methods for Partial Differential Equations** — Khoo, White, Peraire and Patera

### Stochastic modeling — optional

Optional: extend into rigorous probability, statistical inference and stochastic processes for models involving uncertainty over time.

1. **25 — Fundamentals of Probability** — Yury Polyanskiy; retain John Tsitsiklis and other contributor credits on individual notes
2. **26 — Statistical Inference** — Eduardo García-Portugués and Isabel Molina
3. **27 — Discrete Stochastic Processes** — Robert G. Gallager

**Why this order works**

Hammack, the calculus volumes and Hefferon are the working language. You cannot read a stability proof if quantifiers are new, and you cannot discretize a derivative you have not earned. Calculus in one variable, then Hefferon, then the second and third calculus volumes: by the time a derivative in several variables is a matrix, row reduction and bases are already in your hands. The fundamental theorem, Taylor’s theorem with remainder, and the vector-calculus integral theorems are the exact identities your later error estimates will approximate.

Probability and modern statistics come before differential equations, which is the opposite of the pure-math order and is deliberate. An applied model is often a deterministic equation plus a noise term. Grinstead and Snell, then Çetinkaya-Rundel and Hardin, give you expectation, variation and the logic of a statistical claim while the integral is still the calculus integral. You do not need Lebesgue theory to model a measurement. You do need to know the difference between a model and a sample.

Lebl’s differential equations and Tea Time Numerical Analysis turn that language into procedures. A linear ordinary differential equation has a vector space of solutions, so the course is linear algebra in disguise. Laplace transforms and a first look at Fourier series are the linear algebra of signals. Numerical analysis then works without a closed form: interpolation, quadrature and a step method for an initial-value problem, each with an error you can name. Conditioning shows up as soon as a matrix is nearly singular.

Only then does the path return to foundations. Lebl’s first analysis volume rebuilds limits and continuity so that “the step size goes to zero” is a proof. Axler’s second linear algebra supplies operators, inner products and the spectral theorem, which numerical linear algebra uses whenever it rotates a matrix into a better basis. Lebl’s second volume does several variables and metric spaces honestly. Speck’s partial differential equations can now be read as equations: the heat equation, the wave equation and Laplace’s equation as objects, before the function-space language gets abstract. Johnson’s numerical methods come next as algorithms with named errors: conditioning, linear systems and iterative methods. The course that turns a partial differential equation into a grid is the last book of the core.

Axler’s measure book and Rodríguez’s functional analysis are the second climb. The Lebesgue integral is what lets you pass a limit inside an integral under a theorem. Function spaces with norms are where a differential operator becomes a linear map between complete spaces. A first finite-difference scheme can be run before this machinery. The machinery is what tells you why the scheme’s matrix is the right shadow of the operator.

Suh’s convex optimization comes after that climb and just before the numerical PDE course. Convexity is the geometric fact that a local minimum is a global one. Duality is how a constraint becomes a price. The path places Suh here as breadth for constrained models, once the linear algebra and the analysis are strong enough for the proofs. Finite-difference schemes in the numerical PDE course have their own prerequisites in calculus, linear algebra and the earlier numerical books. The numerical PDE course then asks the applied question in full: how a continuous equation becomes a grid, and how the grid’s error behaves.

Books 25, 26 and 27 are the optional stochastic extension. Polyanskiy rebuilds probability on measure, so a random variable is a measurable function and an expectation is an integral. The inference book turns estimation and testing into theorems. Gallager treats dependence in time: Markov chains and discrete stochastic processes. Skip them if your models are deterministic. Take them if the interesting object is noise with a memory. They do not count toward finishing the core path.

**How to study**

For each method, derive a small example, implement it, and compare it with an exact or independently computed result. Change the step size, noise or initial conditions and explain what changes. Keep a record of error and assumptions alongside the answer.

**Companions**

Use C.03, Classical Numerical Methods in Scientific Computing, alongside 23 for additional explanations and exercises in finite differences and finite volumes. The stochastic extension 25 → 26 → 27 is optional and does not count toward core-path completion.

**Books you prepare yourself**

Two books sit beside this path and are not part of the curriculum. Cambridge University Press holds the copyright and allows the authors to keep a PDF on the web for personal reading. Professor Euler does not include the files. Download your own copy from the author page. Do not share the file.

- Boyd and Vandenberghe, *Introduction to Applied Linear Algebra*. Read it beside Hefferon (03) when you want vectors, matrices and least squares in the form data and control use. It is a stronger first applied pass than Axler for that purpose. It does not replace Axler (07). https://web.stanford.edu/~boyd/vmls/
- Boyd and Vandenberghe, *Convex Optimization*. Read it beside Suh (24), after multivariable calculus and linear algebra. Suh is this path's optimization book. Boyd is the standard full account of convex sets, duality and algorithms. https://web.stanford.edu/~boyd/cvxbook/
