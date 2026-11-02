# CS.05 Reinforcement Learning: An Introduction

License: CC BY-NC-ND 2.0 · Source: <http://incompleteideas.net/book/the-book-2nd.html> · 548 pages, 144 exercises in the prepared bundle

*Richard S. Sutton and Andrew G. Barto*

## What this book trains

Richard S. Sutton and Andrew G. Barto’s Reinforcement Learning: An Introduction is the standard account of learning from interaction. An agent acts, the environment answers with a state and a reward, and the agent must learn to make the long-run sum of rewards large without being told which action was right. Part I of the second edition treats what can be done while the values fit in a table. Part II carries the same ideas to function approximation and ends with policy gradient methods. Part III looks outward, to psychology, neuroscience, case studies and the frontiers of the field.

The library’s copy marks 144 exercises, twenty-nine of them in Chapter 3, where they make the Bellman equations routine. Some are short calculations, some ask for a derivation, a proof or pseudocode, and twelve are programming exercises, among them the racetrack, the windy gridworld and Baird’s counterexample. Chapters 14 to 16 have none.

## Why it is worth knowing

The central object is the value function: the expected return from a state, or from a state and an action, under a policy. The Bellman equation says a value is the expected immediate reward plus the discounted value of where you land. Dynamic programming solves it when the dynamics are known, and Monte Carlo methods average complete returns. Temporal-difference learning updates a guess from a later guess before the episode ends; the authors call it the idea most central and novel to reinforcement learning. Part I ends by laying the methods out along dimensions, with generalized policy iteration as their shared pattern.

Approximation is where the guarantees thin out, and the book says so. Function approximation, bootstrapping and off-policy training together form what the authors call the deadly triad, and Baird’s counterexample makes the weights of a linear model diverge. The Bellman error, a natural objective, is not learnable from any amount of data. Policy gradient methods learn the policy itself, and the policy gradient theorem gives the gradient of performance without the derivative of the state distribution. The frontiers chapter warns that an agent can find unintended ways to collect reward, and designing reward signals gets a section of its own.

## What it asks of the other books

The authors chose not to write a rigorous formal treatment. The more mathematical passages sit in shaded boxes a reader may skip, and starred sections and exercises can wait. Part I needs conditional probabilities and expectations, which Grinstead and Snell (08) supply, and the geometric series behind a discounted return, from Calculus Volume 2 (04). The book defines Markov decision processes itself, so Gallager (27) is not required. Part II takes gradients from Calculus Volume 3 (06), and inner products, projections and matrix equations from Hefferon (03). Thimm (CS.04) and Prince (28) give the supervised background the preface suggests, and each has a short treatment of reinforcement learning: Thimm’s reaches Q-learning, and Prince’s goes on to policy gradients.

On the Computer Science & AI path the book closes the machine learning stage, after Thimm and Prince. The preface recommends the first ten chapters, in order, for a one-semester course, and names Chapter 6 the most important for the subject. Foundation Models (CS.06) and the papers Constitutional AI (CS.07) and Direct Preference Optimization (CS.08) follow; for the reinforcement learning from human or AI feedback they discuss, the policy gradient chapter is the background. Dive into Deep Learning (C.01) has a short reinforcement-learning chapter to code beside Chapters 3, 4 and 6. The license recorded in the catalog is CC BY-NC-ND 2.0.

## A walk through the chapters

### Chapter 1

Chapter 1 sets reinforcement learning apart from supervised and unsupervised learning, names its elements (policy, reward signal, value function and, optionally, a model), and builds a tic-tac-toe player that learns the values of positions. A history follows three threads, trial and error, optimal control and temporal differences, to their meeting in the late 1980s.

### Chapters 2–4

Chapter 2 is the k-armed bandit: action-value methods, the 10-armed testbed, incremental and nonstationary estimates, optimistic initial values, upper-confidence-bound selection, gradient bandits and associative search. Chapter 3 is the finite Markov decision process: the agent–environment interface, returns and episodes, policies and value functions, and optimality. Chapter 4 is dynamic programming: policy evaluation, improvement and iteration, value iteration, asynchronous updates and generalized policy iteration, with the gambler’s problem.

### Chapters 5–8

Chapter 5 is Monte Carlo prediction and control, with and without exploring starts, and off-policy prediction by ordinary and weighted importance sampling. Chapter 6 is temporal-difference learning: TD(0), Sarsa, Q-learning, Expected Sarsa, double learning and afterstates. Chapter 7 is n-step bootstrapping, with tree backup and n-step Q(σ). Chapter 8 joins planning and learning: Dyna, prioritized sweeping, expected and sample updates, trajectory sampling, real-time dynamic programming, rollouts and Monte Carlo tree search, and a summary of Part I.

### Chapters 9–13

Chapter 9 is on-policy prediction with approximation: the mean squared value error, semi-gradient methods, linear features from polynomials to tile coding, neural networks, least-squares TD, and kernel-based methods. Chapter 10 is control, from the mountain car to the average-reward setting. Chapter 11, starred, is off-policy learning with approximation: divergence, the deadly triad, the Bellman error, and Gradient-TD and Emphatic-TD methods. Chapter 12 is eligibility traces, from the λ-return to true online TD(λ) and off-policy traces. Chapter 13 is policy gradient methods: the theorem, REINFORCE with and without a baseline, actor–critic methods, and continuous actions.

### Chapters 14–17

Chapter 14 sets the algorithms beside animal learning: classical and instrumental conditioning, the Rescorla–Wagner and TD models, cognitive maps, and habitual against goal-directed behavior. Chapter 15 is neuroscience: dopamine, the reward prediction error hypothesis, a neural actor–critic, and addiction. Chapter 16 is case studies, from TD-Gammon and Samuel’s checkers player to Atari games, Go and thermal soaring. Chapter 17 is frontiers: general value functions, options, observations and state, reward design, and the future of artificial intelligence, including its safety. The references and the index close the book.
