# 27 Discrete Stochastic Processes

License: CC BY-NC-SA 4.0 · Source: <https://ocw.mit.edu/courses/6-262-discrete-stochastic-processes-spring-2011/> · 695 pages, 317 exercises in the prepared bundle

*Robert G. Gallager*

## What this book trains

Robert G. Gallager’s Discrete Stochastic Processes is dependence in time, written as a textbook with exercises and with the course’s problem sets, midterms and finals bound in. After a review of probability, axioms, inequalities and the laws of large numbers, the models are Poisson processes, finite-state Markov chains, renewal processes, countable-state Markov chains, Markov processes in continuous time, and random walks with large deviations and martingales.

A Poisson process counts events whose gaps are exponential and memoryless. Combining and splitting, non-homogeneous rates, and the order-statistic property of the arrival times are the chapter’s structure theorems. A renewal process is what you have when the gaps are independent and identically distributed but not necessarily exponential. A Markov chain is what you have when the future depends on the present state. Rewards, decisions and dynamic programming sit inside the finite-state chapter. Jackson networks and semi-Markov processes sit inside the continuous-time chapter.

## Why it is worth knowing

Memory is the subject. A Poisson process has none: the time until the next event does not depend on how long you have waited. A renewal process remembers only the time since the last renewal. A Markov chain remembers only the current state. Being able to say which memory a model has is the difference between a queueing formula and a wish. The M/M/1 chain, birth–death processes and Jackson networks are the queueing theorems. Reversibility is the surprise that a process and its time reversal can share a stationary distribution, which makes those networks computable.

Martingales and Wald’s identity, in the last chapter, control a random walk at a stopping time. Large deviations estimate the probability of a rare path, exponentially small in the length of the path. Detection and hypothesis testing appear here as a threshold crossing of a walk, the same likelihood ratio as in the inference book, now as a process. The strong law is proved in the renewal chapter in the form the renewal theorem needs, convergence with probability one.

## What it asks of the other books

Grinstead and Snell (08) for a first Markov chapter, and Polyanskiy (25) for measure-theoretic probability. Gallager’s first chapter reviews the axioms, inequalities and laws of large numbers, so a reader fresh from Polyanskiy can move quickly and a reader who skipped the measure course will feel the review’s limits. Linear algebra from Hefferon or Axler helps the eigenvalue section of finite-state chains: a stochastic matrix has a spectral theory, and the stationary distribution is an eigenvector.

The AI path shelves this book before Suh and Prince. It is not a ticket that must be punched before a neural network. It is the right book when the object of study has a memory. The problem sets and the 2009–2011 examinations are part of the bundle.

## A walk through the chapters

### Chapter 1. Probability review

Chapter 1, Probability review. The preface and table of contents are in the front matter. The chapter reviews probability models, the axioms, basic inequalities, the laws of large numbers, and the relation of a probability model to the real world. The inequalities, Markov, Chebyshev and their relatives, are the tools every later tail bound sharpens.

### Chapter 2. Poisson processes

Chapter 2, Poisson processes. Definition and properties, combining and splitting, non-homogeneous processes, and conditional arrival densities with the order-statistic property. Merging independent Poisson processes yields a Poisson process whose rate is the sum. Splitting each point independently yields independent Poisson processes. That pair of theorems is why Poisson is the counting process people reach for first.

### Chapter 3. Finite-state Markov chains

Chapter 3, Finite-state Markov chains. Classification of states, the matrix representation, eigenvalues and eigenvectors of stochastic matrices, chains with rewards, and Markov decision theory with dynamic programming. A state is transient or recurrent. Periodicity is the extra label. The decision section chooses an action in each state to maximize a reward. It is optimization on a chain.

### Chapter 4. Renewal processes

Chapter 4, Renewal processes. The strong law, the strong law for renewals, renewal-reward processes as time averages and as ensemble averages, random stopping, the expected number of renewals, and delayed renewals. A delayed renewal lets the first gap have a different law, which is the stationary version of a process you started observing at a random time.

### Chapter 5. Countable-state Markov chains

Chapter 5, Countable-state Markov chains. Classification, birth–death chains, reversibility, the M/M/1 sample-time chain, branching processes, and round-robin and processor sharing. An infinite state space can be transient even when every state can reach every other. Branching processes return from Grinstead’s generating-function chapter with a Markov description.

### Chapter 6. Markov processes with countable state spaces

Chapter 6, Markov processes with countable state spaces. Steady state of an irreducible process, the Kolmogorov differential equations, uniformization, birth–death processes, reversibility, Jackson networks, and semi-Markov processes. Uniformization turns a continuous-time chain into a discrete chain with exponential holding times, which is both a theorem and a way to simulate. A Jackson network is a system of queues whose stationary distribution is a product.

### Chapter 7. Random walks, large deviations, and martingales

Chapter 7, Random walks, large deviations, and martingales. The queueing delay in a G/G/1 queue, detection and hypothesis testing, threshold crossing, Wald’s identity, martingales, submartingales and supermartingales, stopped processes, the Kolmogorov inequalities, and Markov-modulated walks. Twelve problem sets, an appendix and bibliography, and the 2009 and 2011 finals and the 2009–2011 midterms are bound after the chapters.
