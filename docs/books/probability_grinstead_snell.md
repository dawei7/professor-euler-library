# 08 Introduction to Probability

License: GFDL · Source: <https://math.dartmouth.edu/~prob/prob/prob.pdf> · 592 pages, 709 exercises in the prepared bundle

*Charles Grinstead and J. Laurie Snell*

## What this book trains

Introduction to Probability, by Charles M. Grinstead and J. Laurie Snell, is a first course that treats probability as mathematics with simulations beside the theorems. Discrete distributions and continuous densities, combinatorics, conditional probability, the important named distributions, expectation and variance, sums of random variables, the law of large numbers, the central limit theorem, generating functions, Markov chains, and random walks.

Expectation is a weighted average, and it is linear even when the variables are dependent. The law of large numbers says the sample average settles on the expectation. The central limit theorem says the fluctuations around that average, scaled properly, look Gaussian. Markov chains are dependence with a short memory: the next state depends on the present state and not on the path that led there.

## Why it is worth knowing

Almost every later claim about data is a sentence in this language. A statistical test is a probability computed under a model. A loss on a random sample has an expectation. A training run is a random walk of a particular kind. The book earns those sentences before anyone asks you to trust a p-value.

The joy is in the paradoxes and the exact models. Conditional probability produces situations where an intuitively obvious answer is wrong, and the book has a section of paradoxes so you can enjoy being corrected by a computation. Card shuffling, gambler’s ruin, branching processes and the arc sine laws are theorems about familiar pictures. Generating functions, already met in Levin, return as a way to study a distribution by a series. Simulation is not a substitute for the proof. It is a way to see the theorem before you prove it, and a way to check the proof after.

## What it asks of the other books

Counting from Hammack (01) or Levin (05). The book contains its own combinatorics chapter, permutations, combinations and card shuffling, so a gap can be repaired in place. Calculus Volumes 1 and 2 (02, 04) for the integral, because a continuous density is integrated, and an expectation of a continuous random variable is an integral. Improper integrals from Volume 2 are the reason a density on the whole line can integrate to 1.

Modern statistics (09) uses this language on data. Polyanskiy (25) rebuilds it on measure theory after Axler’s measure book (19). Gallager (27) continues the Markov chains and adds Poisson processes and renewal theory. The curriculum places this book before the measure-theoretic return, on purpose. You do not need Lebesgue theory to model a measurement.

## A walk through the chapters

### 1. Discrete Probability Distributions

Discrete Probability Distributions. Simulation of discrete probabilities, and the distributions themselves. A probability is a number assigned to outcomes so that disjoint outcomes add and the whole space adds to 1. Simulation makes the definition feel like a repeated experiment.

### 2. Continuous Probability Densities

Continuous Probability Densities. Simulation again, then density functions. A density is not a probability. The probability of a region is the integral of the density. A single point gets probability zero. That distinction matters the moment someone asks for the probability of an exact real number.

### 3. Combinatorics

Combinatorics. Permutations, combinations, and card shuffling. This is the counting the discrete models need. Shuffling is a serious example, not a pastime: a shuffle is a random permutation, and the distribution of a shuffle is something you can compute.

### 4. Conditional Probability

Conditional Probability. The discrete and continuous theories, and paradoxes. Conditioning restricts the sample space. The continuous case needs care because you are conditioning on events of probability zero when you condition on an exact value. The paradoxes are there to make the formalism feel necessary.

### 5. Important Distributions and Densities, then Expected Value and Variance

Important Distributions and Densities, then Expected Value and Variance. The named families, Bernoulli, binomial, Poisson, geometric, normal, exponential and their relatives, then expectation and variance in the discrete case and the continuous case. Linearity of expectation is the tool that makes many hard counts easy. Variance adds when the variables are uncorrelated, and not in general.

### 6. Sums of Random Variables

Sums of Random Variables. Discrete and continuous. The distribution of a sum is a convolution. This is why generating functions and, later, characteristic functions exist: they turn convolution into multiplication.

### 7. Law of Large Numbers, and the Central Limit Theorem

Law of Large Numbers, and the Central Limit Theorem. Discrete and continuous versions of the law. The central limit theorem for Bernoulli trials, for discrete independent trials, and for continuous independent trials. The law says the average converges to the mean. The central limit theorem says the shape of the error is approximately normal, with a width that shrinks like one over the square root of the number of trials. Statistics lives on that width.

### 8. Generating Functions

Generating Functions. Discrete distributions, branching processes, and continuous densities. A branching process is a population in which each individual independently produces offspring. Extinction probabilities fall out of a functional equation. It is one of the cleanest applications of generating functions in the book.

### 9. Markov Chains

Markov Chains. Introduction, absorbing chains, ergodic chains, the fundamental limit theorem, and mean first passage time. An absorbing chain ends in a state it cannot leave. An ergodic chain keeps mixing, and the fundamental limit theorem says the probability of being in each state forgets the start. Mean first passage time is how long that takes. Gallager’s book is the graduate continuation of this chapter.

### 10. Random Walks

Random Walks. Walks in Euclidean space, gambler’s ruin, and the arc sine laws. Gambler’s ruin is a walk on the integers with two absorbing ends. The arc sine laws are the surprising theorems about how a random walk spends its time positive or negative. They are a reward for readers who reached the last chapter: exact, counterintuitive, and proved.
