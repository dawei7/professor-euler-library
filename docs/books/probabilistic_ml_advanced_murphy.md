# C.02 Probabilistic Machine Learning: Advanced Topics

License: CC BY-NC-ND 4.0 · Source: <https://mitpress.mit.edu/9780262048439/probabilistic-machine-learning/> · 1370 pages, 0 exercises in the prepared bundle

*Kevin P. Murphy*

## What this book trains

Kevin P. Murphy’s Probabilistic Machine Learning: Advanced Topics is the optional research companion, not an introductory textbook. It assumes you can already read a likelihood. The early chapters rebuild probability, statistics, graphical models, information theory and optimization at the level the later algorithms need. Inference is then a subject of its own: an overview, Gaussian filtering and smoothing, message passing, variational inference, Monte Carlo, Markov-chain Monte Carlo, and sequential Monte Carlo. Predictive models and generalized linear models lead into deep networks, Bayesian neural networks, and Gaussian processes. The book then leaves the independent-and-identically-distributed assumption and spends a long stretch on generative models: variational autoencoders, autoregressive models, normalizing flows, energy-based models, diffusion, and adversarial networks. Discovery, latent factor models, state-space models, graphs, nonparametric Bayes, representation learning, and interpretability follow. The last movement is decision making, reinforcement learning, and causality.

The catalog places it as an optional reference after the foundations. It supplies a Bayesian and algorithmic depth that book 26 does not attempt. It is not a new compulsory stage, and it does not replace Prince, Bach, or Samworth and Shah.

## Why it is worth knowing

A probabilistic model writes a joint distribution and then computes. Prediction, in this book, is often a distribution, and the hard part is the computation. Variational inference replaces the posterior by a tractable family and optimizes a bound. Markov-chain Monte Carlo builds a chain whose stationary distribution is the posterior: Metropolis–Hastings, Gibbs, Hamiltonian Monte Carlo. Particle filters carry a cloud of samples through a state-space model. These are different answers to one obstacle, and the pleasure is knowing which answer you reached for and what it approximates.

Graphical models make conditional independence a missing edge, directed or undirected, and the chapter includes structural causal models before the dedicated causality chapter returns with randomized trials, confounders, instruments, and the do-calculus. Information theory is entropy, mutual information, compression and channel coding, used as tools. Gaussian processes, diffusion, flows and adversarial networks reappear here as probabilistic objects, so a reader of Prince can see the same architectures attached to a posterior or a score. Causality is kept distinct from prediction. That distinction is the chapter’s point.

## What it asks of the other books

Read it after the inference book (26), or beside it once the likelihood, intervals and tests are familiar. Probability (08, and ideally Polyanskiy, 25) and linear algebra (07) are assumed more than reviewed. Prince (28) makes the deep-network and generative chapters concrete. Suh (24) helps the optimization chapter. Gallager (27) is the right background for the Markov chains inside the probability chapter and for the state-space models later. Samworth and Shah (30) remain the high-dimensional statistics text. This companion does not replace them.

The license recorded in the catalog is CC BY-NC-ND 4.0. The companion is not required for any path. The learning-path guide shelves it beside books 26, 28, 29 and 30.

## A walk through the chapters

### Chapters 1–3

The front matter is the title, copyright, contents and preface. Chapter 1 is the introduction. Chapter 2, Probability, covers common distributions, Gaussian joint distributions, the exponential family, transformations of random variables, Markov chains, and divergence measures. Chapter 3, Statistics, sets Bayesian and frequentist statistics side by side, then conjugate, noninformative and hierarchical priors, empirical Bayes, model selection, model checking, hypothesis testing, and missing data.

### Chapter 4. Graphical models

Chapter 4, Graphical models: directed models, undirected models, conditional random fields, the comparison, extensions, and structural causal models. Chapter 5, Information theory: Kullback–Leibler divergence, entropy, mutual information, source coding, channel coding, the information bottleneck, and algorithmic information theory. Chapter 6, Optimization: automatic differentiation, stochastic optimization, natural gradient descent, bound optimization, Bayesian optimization, derivative-free optimization, optimal transport, and submodular optimization.

### Chapters 7–13

Chapter 7 overviews inference patterns and the exact and approximate algorithms. Chapter 8 is Gaussian filtering and smoothing, including the linear-Gaussian state-space model, local linearization, the unscented transform, and other Kalman variants. Chapter 9 is message passing: belief propagation on chains, trees and loopy graphs, variable elimination, and the junction tree. Chapter 10 is variational inference, from gradient-based and coordinate-ascent methods to expectation propagation. Chapter 11 is Monte Carlo integration, rejection sampling and importance sampling. Chapter 12 is Markov-chain Monte Carlo, including Metropolis–Hastings, Gibbs sampling and Hamiltonian Monte Carlo. Chapter 13 is sequential Monte Carlo and the particle filter.

### Chapters 14–19

Chapter 14 overviews predictive models, including conformal prediction. Chapter 15 is generalized linear models: linear, logistic and probit regression, and multilevel models. Chapter 16 is deep neural networks as differentiable circuits. Chapter 17 is Bayesian neural networks: priors, posteriors, generalization, and online inference. Chapter 18 is Gaussian processes, Mercer kernels, Gaussian and non-Gaussian likelihoods, and the link to deep networks. Chapter 19 is what happens beyond the i.i.d. assumption: distribution shift, robustness, adaptation, continual learning, and adversarial examples.

### Chapters 20–26

Chapter 20 overviews generative models and their training objectives. Chapters 21 through 26 are the families: variational autoencoders, autoregressive models (including transformers and large language models as the chapter’s own sections), normalizing flows, energy-based models and score matching, diffusion models, and generative adversarial networks.

### Chapters 27–36

Chapter 27 opens the discovery part. Chapter 28 is latent factor models: mixtures, factor analysis, topic models, and independent components analysis. Chapter 29 is state-space models: hidden Markov models, linear dynamical systems, switching and nonlinear variants, and deep state-space models. Chapter 30 is graph learning. Chapter 31 is nonparametric Bayesian models. Chapter 32 is representation learning. Chapter 33 is interpretability. Chapter 34 is decision making under uncertainty: statistical decision theory, influence diagrams, contextual bandits, Markov decision problems, and active learning. Chapter 35 is reinforcement learning by value, by policy, and by model. Chapter 36 is causality: the formalism, randomized trials, confounder adjustment, instrumental variables, difference in differences, and the do-calculus. The index and bibliography close the book.
