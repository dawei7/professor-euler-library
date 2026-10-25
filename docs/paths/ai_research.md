# AI Research — Probability, Statistics & Machine Learning

Understand how learning systems are built, why they can generalize, and how to investigate when they fail. A fit on the data you trained on is not yet a claim about data you have not seen. The mathematics is what makes that distinction precise.

**What you will learn**

The objects of learning are mathematical before they are computational. A dataset is a sample from a distribution. A model is a family of functions, often a composition of linear maps and simple nonlinearities. A loss sends parameters to a real number, and training tries to make that number small. Generalization is the separate question: why a minimum on the sample should say anything about a fresh draw from the same distribution. A fit on the training data is a fact about the sample. A claim about unseen data needs a theorem, or an experiment that can fail.

Linear algebra is the geometry of the data. A batch is a matrix, and a layer is a linear map plus a nonlinearity. The column space says which outputs a linear layer can reach. A covariance is positive semidefinite, so it has a square root and a set of principal axes. Singular values say which directions a linear map stretches, which is the linear version of “which features survive”. A gradient lives in the same space as the parameters. Hefferon makes the computations yours. Axler’s spectral theorem says why those principal axes exist: a self-adjoint operator is diagonal in an orthonormal basis.

Calculus and analysis are why a training step can be a proof rather than a hope. A gradient step is Euler’s method on the gradient flow of the loss. Taylor’s theorem with remainder is the honest form of “the loss is locally a parabola”: the linear term picks the direction, the quadratic term warns you about the curvature, and the remainder says how far that picture holds. Convexity is the geometric fact that a local minimum is a global one, and duality turns a constraint into a price. A deep network is usually not convex. The same one-step theorems still describe the step. They stop promising that the valley you found is the only one. Metric spaces and a little functional analysis are the language those sentences are written in.

Probability, inference and dependence are three views of the same uncertainty. Probability says what a random draw is, and once the integral has grown up, expectation is an integral of a measurable function. Inference says what an estimator is entitled to claim: bias, variance, a confidence set, a test, and the difference between a procedure and a proof that the procedure works. A stochastic process puts the draw in time. A Poisson process counts events with no memory of when the last one happened. A Markov chain has a short memory: given the present, the future forgets the past. Renewal theory sits between them, when what repeats is a gap rather than a state.

The last four books separate four different reasons a method can fail. Optimization can fail because the landscape has the wrong shape, or the step size ignores the smoothness. Approximation can fail because the family of functions cannot get close to the target, however long you train. Statistics can fail because the sample was too small, or the dimension was large enough that intuition from the plane quietly died: distances concentrate, and a covariance estimated entrywise needs a model of sparsity or low rank. A paper that reports a number is mixing these reasons. The path trains you to take the mixture apart.

### Foundation

Develop proof, calculus, linear algebra, discrete reasoning, introductory probability/statistics and reliable numerical computation.

1. **01 — Book of Proof** — Richard Hammack
2. **02 — Calculus, Volume 1** — OpenStax
3. **03 — Linear Algebra** — Jim Hefferon
4. **04 — Calculus, Volume 2** — OpenStax
5. **05 — Discrete Mathematics: An Open Introduction** — Oscar Levin
6. **06 — Calculus, Volume 3** — OpenStax
7. **08 — Introduction to Probability** — Charles Grinstead and J. Laurie Snell
8. **09 — Introduction to Modern Statistics** — Mine Çetinkaya-Rundel and Johanna Hardin
9. **10 — Basic Analysis I: Introduction to Real Analysis, Volume I** — Jiří Lebl
10. **07 — Linear Algebra Done Right** — Sheldon Axler
11. **15 — Basic Analysis II: Introduction to Real Analysis, Volume II** — Jiří Lebl
12. **14 — Tea Time Numerical Analysis** — Leon Q. Brin
13. **22 — Introduction to Numerical Methods** — Steven G. Johnson

### Probability and statistics

Move from measure and integration to rigorous probability, estimation and testing, then dependence and stochastic processes.

1. **19 — Measure, Integration & Real Analysis** — Sheldon Axler
2. **25 — Fundamentals of Probability** — Yury Polyanskiy; retain John Tsitsiklis and other contributor credits on individual notes
3. **26 — Statistical Inference** — Eduardo García-Portugués and Isabel Molina
4. **27 — Discrete Stochastic Processes** — Robert G. Gallager

### Machine learning

Move from optimization to deep-learning architectures, then learning theory and modern statistical guarantees. The purpose is understanding and investigating models, not only running them.

1. **24 — Convex Optimization for Machine Learning** — Changho Suh
2. **28 — Understanding Deep Learning** — Simon J. D. Prince
3. **29 — Learning Theory from First Principles** — Francis Bach
4. **30 — Modern Statistical Methods and Theory: An Introduction to Nonparametric and High-Dimensional Statistics** — Richard J. Samworth and Rajen D. Shah

**Why this order works**

Hammack, the calculus volumes and Hefferon are the grammar. Every generalization bound is a sentence with quantifiers, so ∀ and ∃ come before the bound. A gradient is a derivative, and a Jacobian is the derivative of a vector-valued map, so one-variable and several-variable calculus come before any training algorithm. A layer is a matrix and a batch of data is one too, so row reduction, bases and linear maps come before the layer. Calculus Volume 2 sits before discrete mathematics so that series and the Taylor remainder exist before you start counting.

Levin is on this path, and absent from the applied path, because learning theory counts. Combinations give a hypothesis class a size. Graphs keep a nearest-neighbor or a message-passing picture exact. Recurrences are how an iteration gets a closed form. Calculus Volume 3 then makes the gradient a vector. Probability and modern statistics come next, still on the calculus integral: expectation, variance, a likelihood, a test. You want those words fluent before analysis rebuilds the foundations under them.

Lebl’s two analysis volumes and Axler’s second linear algebra are the first deepening. Completeness and continuity turn “the step gets smaller” into an argument. Inner products and the spectral theorem turn principal-component analysis from a recipe into a theorem. Numerical analysis, first Brin’s course and then Johnson’s, puts an error bar on the arithmetic. A computed gradient is an approximation. A matrix can be ill-conditioned, which is a property of the problem. An iterative method has a rate, which is a property of the algorithm. Those are different facts, and papers mix them up.

Measure is the point where the integral grows up. Axler’s measure book builds the Lebesgue integral. Polyanskiy then builds probability on it, so a random variable is a measurable function, an expectation is an integral, and the limit theorems have hypotheses you can check. High-dimensional arguments later in the path assume that book even when they do not cite it. The inference book turns estimation and testing into mathematics: a procedure is an object, and a guarantee is a theorem about that object. Gallager adds time. Poisson processes, renewal processes and Markov chains are three different memories: none, a gap that restarts, and a state that is enough. That is dependence as a mathematical object.

Suh is placed before the three learning books, and that placement is the point of the path. Gradient descent, convexity and duality are already mathematical objects when Prince describes a network. Prince’s book is the path’s account of modern neural networks, transformers and generative models, read as compositions of maps whose training is that optimization. Bach then asks what approximation, optimization and generalization each contributed, including the modern regime in which a model has more parameters than samples and the old “it will overfit” slogan is only part of the story. The question is sharper after you have seen a model. Samworth and Shah come last because high-dimensional and nonparametric statistics correct the geometry: finite-sample theory, high-dimensional regression, and methods that do not begin by picking a finite list of parameters.

Gallager sits on the shelf before Prince because information and dependence are part of the probability education, and a network is one of several reasons to learn them. Stochastic processes are the right tool when the object of study has a memory. Read them in that spot, or return to them beside the learning books, whenever that object is yours. The order starts from the mathematics so that a broken formula has a theory waiting for it. If you would rather meet the theory early, read the matching chapters of Bach alongside Prince. The path still wants the models in view while you do it.

**How to study**

Study mathematics and experiments together. Derive a result, implement a small version, reproduce a published baseline, and change one assumption at a time. As you reach the ML stage, read papers and write short critiques of their assumptions, evidence and limitations. Books build research foundations; original research also needs sustained paper reading, programming and experiments.

**Companions**

Use C.01 Dive into Deep Learning alongside Prince (28) for coding. Use C.04 Rigollet alongside Bach (29) for compact theory and matched solved assignments. Read selected C.02 Murphy Advanced chapters after the relevant probability/ML foundations for Bayesian inference, probabilistic models and further research topics. These are optional references, not extra compulsory stages.

**Books you prepare yourself**

Seven further books are widely used and are not part of the curriculum. The app does not include their files. Copyright stays with the publisher. Download a personal copy only from the page named here. Do not share the file. None of these replaces a numbered book on the path.

- Boyd and Vandenberghe, *Introduction to Applied Linear Algebra*. Beside Hefferon (03). Axler (07) remains the proof-based second course. https://web.stanford.edu/~boyd/vmls/
- Deisenroth, Faisal and Ong, *Mathematics for Machine Learning*. After calculus (02, 04, 06), linear algebra (03) and introductory probability (08), and before Prince (28). It does not replace analysis or Polyanskiy (25). https://mml-book.github.io/
- Boyd and Vandenberghe, *Convex Optimization*. Beside Suh (24). Suh is the path's machine-learning course in optimization. Boyd is the fuller reference. https://web.stanford.edu/~boyd/cvxbook/
- MacKay, *Information Theory, Inference, and Learning Algorithms*. After probability (08), and beside Murphy (C.02). It does not replace Gallager (27) or Bach (29). Printing the whole book is not permitted. https://www.inference.org.uk/itila/book.html
- Bishop, *Pattern Recognition and Machine Learning*. Beside Prince (28) and Murphy (C.02). Prince remains the deep-learning book. Bishop is the probabilistic generation: mixtures, EM, graphical models and kernels. Springer holds the copyright; Microsoft Research posts a PDF for personal reading. https://www.microsoft.com/en-us/research/publication/pattern-recognition-machine-learning/
- Shalev-Shwartz and Ben-David, *Understanding Machine Learning*. Beside Bach (29) and Rigollet (C.04). Classical PAC, VC and kernel theory. Bach stays the path book. https://www.cs.huji.ac.il/~shais/UnderstandingMachineLearning/
- Vershynin, *High-Dimensional Probability*. After Polyanskiy (25), and beside Samworth–Shah (30). Personal use only, not for redistribution. https://www.math.uci.edu/~rvershyn/papers/HDP-book/HDP-book.html
