# CS.03 Elements of Robotics

License: CC BY 4.0 · Source: <https://doi.org/10.1007/978-3-319-62533-1> · 311 pages, 104 exercises in the prepared bundle

*Mordechai Ben-Ari and Francesco Mondada*

## What this book trains

Mordechai Ben-Ari and Francesco Mondada’s Elements of Robotics teaches the algorithms of autonomous mobile robots and the mathematical and physical principles behind them. It is written for secondary school and the first years of university, and it is not tied to one machine. Chapter 1 defines a generic robot with differential drive, proximity sensors that report the direction and distance of an object, ground sensors, and an embedded computer. Algorithms are written in pseudocode, not in a programming language.

The first six chapters are the core, four chapters on navigation follow, and the last six are advanced topics that the authors say can be read in any order. The exercises are the book’s 104 activities. Most ask you to implement an algorithm on a robot and watch what it does. Some start at a desk: applying Dijkstra’s algorithm to a grid map, or turning three pencils through a sequence of Euler angles. The material grew out of the Thymio educational robot; the preface invites you to adapt the activities to yours.

## Why it is worth knowing

A robot that sets equal power on both wheels does not drive straight. Small differences between motors and wheels, friction and an uneven floor turn it aside, so it has to sense and correct itself. A Braitenberg vehicle couples sensors directly to motors and already looks timid, paranoid or insecure. A finite state machine adds memory. Odometry computes position from speed and time, and its errors are not equal: a heading error of 2 % puts the robot 1.25 m off after 10 m, a distance error of 2 % only 0.2 m. A closed loop corrects an error as it measures it, and the PID controller keeps its integral as a running sum of errors and its derivative as a difference.

Probability enters where certainty runs out. One-dimensional Markov localization keeps a belief array over positions along a wall with doors, sharpens it each time the sensors see a door, and allows for a move that goes zero, one or two positions. A simplified algorithm for simultaneous localization and mapping is computed on a numerical example before it is formalized. The learning chapters train artificial neurons with the Hebbian rule, separate two shades of gray by linear discriminant analysis, and teach a perceptron to tell a safe slope from a dangerous one, the last two on real data from a Thymio. Swarm robotics shows clustering and collective pushing emerge from local rules.

## What it asks of the other books

The preface asks for programming, and for school or first-year university mathematics and physics: algebra, trigonometry, calculus, matrices and probability, and velocity, acceleration, force and friction. Each is used locally. Trigonometry carries odometry with turns, triangulation and the kinematics of the arm. Calculus is the derivative and integral of motion and the PID formula. Probability is Bayes’ rule for localization and mapping, and means, variances and covariance for the discriminants. Matrices are the image filters and the rotations and homogeneous transforms. Appendix B reviews the probability, the statistics and the products of vectors and matrices.

On the Computer Science & AI path the book is in the second stage, Systems and robotics, beside Marwedel’s Eingebettete Systeme (CS.02). The foundations before it, Lehman (CS.01), Calculus Volumes 1–3 (02, 04, 06) and Hefferon (03), cover more than it needs. Corral (S.03) is enough trigonometry, and Lehman’s probability part or Grinstead and Snell (08) give the conditional probability. Lehman’s state machines and graphs return here as robot behaviors and path planning. The learning chapters are a first look at what Thimm (CS.04) and Prince (28) take up in the next stage. The book calls its Hebbian learning a form of reinforcement learning because the feedback says only good or bad; Sutton and Barto (CS.05) develop reinforcement learning as a subject of its own.

The license recorded in the catalog is CC BY 4.0.

## A walk through the chapters

### Chapters 1–6. The core

Chapter 1 classifies robots, specifies the generic robot and sets out the pseudocode. Chapter 2 is sensors: distance sensors of several kinds, cameras, and range, resolution, precision, accuracy and nonlinearity. Chapter 3 is reactive behavior: Braitenberg vehicles and line following. Chapter 4 is finite state machines. Chapter 5 is motion: odometry and its errors, wheel encoders, inertial navigation, degrees of freedom, and holonomic motion. Chapter 6 is control: open and closed loops and the on-off, P, PI and PID controllers.

### Chapters 7–10. Navigation

Chapter 7 is obstacle avoidance: wall following, the Pledge algorithm, reading a code while following a line, and a probabilistic model of ants searching for food. Chapter 8 is localization: landmarks, triangulation, GPS, and probabilistic localization. Chapter 9 is mapping: grid maps with occupancy probabilities, the frontier algorithm, and SLAM. Chapter 10 plans paths with Dijkstra’s algorithm on grid and continuous maps and with A*, then combines path following with obstacle avoidance.

### Chapters 11–14. Fuzzy logic, images and learning

Chapter 11 is fuzzy logic control: fuzzify, apply rules, defuzzify. Chapter 12 is image processing: spatial filters, histograms, edges, corners and blobs, with activities a robot without a camera can perform. Chapter 13 is neural networks: the artificial neuron, a Braitenberg vehicle built from neurons, multilayer networks, memory, and the Hebbian rule. Chapter 14 is machine learning: a discriminant from means and variances, then linear discriminant analysis and perceptrons, both worked numerically.

### Chapters 15–16 and the appendices

Chapter 15 is swarm robotics: communication, the BeeClust algorithm, and robots that combine their forces to pull a stick or push an object. Chapter 16 is the kinematics of a two-link arm: forward and inverse kinematics, rotations and homogeneous transforms in the plane, and a taste of three-dimensional rotations through Euler angles. Appendix A gives units of measurement. Appendix B collects tutorials and derivations, from Bayes’ rule to algebraic formulas for cos 15°. The index closes the book.
