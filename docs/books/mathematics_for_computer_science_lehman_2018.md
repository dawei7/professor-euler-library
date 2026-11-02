# CS.01 Mathematics for Computer Science

License: CC BY-SA 3.0 · Source: <https://courses.csail.mit.edu/6.042/spring18/mcs.pdf> · 1048 pages, 819 exercises in the prepared bundle

*Eric Lehman, F. Thomson Leighton and Albert R. Meyer*

## What this book trains

Eric Lehman, F. Thomson Leighton and Albert R. Meyer’s Mathematics for Computer Science is the text of MIT’s course 6.042, in its revision of 6 June 2018. It teaches the mathematics a computer scientist reasons with, and it teaches it through proof. The book’s own definition sets the tone: a mathematical proof of a proposition is a chain of logical deductions leading to the proposition from a base set of axioms. Five parts follow: Proofs, Structures, Counting, Probability and Recurrences.

Each chapter ends with problems grouped by section and sorted into practice, class, homework and exam problems, 819 in all. The book opens the Computer science & AI shelf.

## Why it is worth knowing

The examples are computations, and the proofs are about them. A state machine is a set of states and transitions, and the invariant principle says that a property preserved by every transition holds in every reachable state. That one principle shows that a robot stepping diagonally on the integer grid never reaches (1, 0), settles the water jugs of Die Hard, and proves fast exponentiation correct, with termination coming from well ordering. The stable marriage chapter proves that its mating ritual ends with no rogue couple. Games of perfect information are a recursive data type, so structural induction proves that one player has a winning strategy. A diagonal argument shows that no program can decide whether an arbitrary program halts.

Number theory leads to RSA, with a section on why an efficient test for satisfiability would factor numbers and so break it. Probability is taught with the warning that intuition fails. A four-step method is applied to the Monty Hall problem and to dice that beat each other in a circle, and a section separates the confidence one has in a test from the probability of the disease it tests for. Linearity of expectation, the bounds of Markov, Chebyshev and Chernoff, gambler’s ruin and the stationary distribution behind page rank are tools the field uses every day.

## What it asks of the other books

Little beyond school algebra. The first axioms are, in the authors’ words, all familiar facts from high school math, and the opening chapters assume only a first acquaintance with sets and functions, which chapter 4 then makes careful. Calculus appears in a few places: integrals bound sums, Stirling’s formula estimates n!, power series are differentiated in the generating-function chapter, and the Akra–Bazzi formula contains an integral. Generating functions are formal power series, so convergence is not needed. Wallace (S.01) and Stitz and Zeager (S.04) cover the algebra.

On the Computer Science & AI path this is the first book, before Calculus Volume 1 (02), Hefferon (03), Calculus Volume 2 (04) and Calculus Volume 3 (06). The path does not include Hammack (01) or Levin (05); this book covers their logic, proofs, sets, relations, induction, cardinality, graphs and counting. Raji (12) continues the number theory, Grinstead and Snell (08) the probability, and Gallager (27) the random walks. On the same shelf, Ben-Ari and Mondada (CS.03) use finite state machines and paths on graphs, and Sutton and Barto (CS.05) work with expectation and Markov chains.

The license recorded in the catalog is CC BY-SA 3.0.

## A walk through the chapters

### Chapters 1–5. Proofs, logic and induction

Chapter 1 asks what a proof is, from propositions and axioms to implications, cases and contradiction. Chapter 2 is the well ordering principle and factoring into primes. Chapter 3 is logical formulas: connectives, equivalence and validity, the SAT problem, and quantifiers. Chapter 4 is sets, sequences, functions, binary relations and finite cardinality. Chapter 5 is ordinary and strong induction, compared with well ordering.

### Chapters 6–8. State machines, recursive data and infinite sets

Chapter 6 is state machines, partial correctness and termination, and stable marriage. Chapter 7 is recursive data types: structural induction, matched brackets, arithmetic expressions, games, and search trees up to AVL trees. Chapter 8 is infinite sets: countability, the diagonal argument, the halting problem, Russell’s paradox and the ZFC axioms, and a closing section on the continuum hypothesis and Gödel’s incompleteness.

### Chapters 9–13. Structures

Chapter 9 is number theory: divisibility, the greatest common divisor, primes, an encryption scheme Turing proposed in 1937, broken in two versions, modular arithmetic, inverses, Euler’s theorem and RSA. Chapter 10 is directed graphs: walks, adjacency matrices, scheduling with Dilworth’s lemma, partial orders and equivalence relations. Chapter 11 compares routing networks by diameter, switch count, latency and congestion, from the complete binary tree to the butterfly and the Beneš network. Chapter 12 is simple graphs: degrees, isomorphism, bipartite matching, coloring, connectivity, Euler tours, and trees with minimum-weight spanning trees. Chapter 13 is planar graphs: Euler’s formula, why K5 and K3,3 are not planar, five-coloring, the regular polyhedra, and Kuratowski’s theorem, stated without proof.

### Chapters 14–16. Counting

Chapter 14 is sums: annuities, bounds by integrals, the book-stacking problem and harmonic numbers, and asymptotic notation with its pitfalls. Chapter 15 is the cardinality rules, poker hands, the pigeonhole principle with a card trick, inclusion–exclusion and combinatorial proofs. Chapter 16 is generating functions: the convolution rule, partial fractions, linear recurrences, and formal power series.

### Chapters 17–21. Probability

Chapter 17 is probability spaces, strange dice and the birthday principle. Chapter 18 is conditional probability: tree diagrams, medical testing, Simpson’s paradox, independence, and probability versus confidence. Chapter 19 is random variables, their distributions and expectation, with the coupon collector. Chapter 20 is deviation from the mean: variance, estimation by sampling, and the Chernoff bound with randomized load balancing. Chapter 21 is gambler’s ruin and random walks on graphs.

### Chapter 22. Recurrences

Part V is one chapter: the Towers of Hanoi, merge sort, linear recurrences, divide-and-conquer recurrences with the Akra–Bazzi formula and the master theorem, and rules of thumb for judging a recurrence without calculation. A bibliography, a glossary of symbols and the index close the book.
