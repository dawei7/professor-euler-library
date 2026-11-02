# Computer Science & AI

Learn the mathematics computer science runs on, then follow it into machines that sense and act, systems that learn from data, and the language models of today. A program that passes its tests has not yet been shown correct, and a model that fits its data has not yet been shown to work on the next input. This path keeps both questions in view.

**What you will learn**

Discrete mathematics is the language the rest of the path is written in. A loop is correct because an invariant holds before it, after every pass, and at the end, and induction is the proof that it does. A running time is a sum or a recurrence, and asymptotic notation says which term wins. Counting tells you how many cases an algorithm must face; probability tells you how often a random one fails. Number theory turns into public-key cryptography, and a graph is the shape of a network, a schedule or a state machine. Lehman, Leighton and Meyer cover all of it in one book, with the exercises to make it yours.

A computer in a device is a different object from a computer on a desk. It has a deadline, a power budget and sensors that report a noisy version of the world. Marwedel's book follows such a system from its specification and models of computation through its hardware and system software to its evaluation and validation, then maps applications onto processors with real-time scheduling, optimizes them and tests them. Ben-Ari and Mondada then give the system wheels: reactive behaviour and finite state machines, motion and odometry, control, obstacle avoidance, localization and mapping, and at the end neural networks, machine learning and swarms in small robots. A robot that does not know where it is already needs probability, and a control loop is the first place feedback becomes mathematics.

Learning from data has three shapes. Supervised learning fits a function to labelled examples and must be evaluated on examples it has not seen. Unsupervised learning looks for structure without labels: clusters, rules, anomalies, principal components. Reinforcement learning learns from a reward that arrives late, by acting. Thimm's book teaches the classical methods of all three and ends with neural networks. Prince's book is the path's account of deep networks, transformers and generative models. Sutton and Barto build reinforcement learning from the ground up: bandits, Markov decision processes, dynamic programming, Monte Carlo and temporal-difference learning, then function approximation and policy gradients.

The last stage reads the language-model literature. Paaß and Giesselbach survey pre-trained models as they stood in 2023: how BERT and GPT are trained and improved, what knowledge they hold, and how they are used for information extraction, text generation and other media. The two papers are a pair. Both start from reinforcement learning from human feedback. Constitutional AI replaces human labels of harmful answers by AI feedback guided by a written list of principles. Direct Preference Optimization removes the separate reward model and the reinforcement-learning loop and fits the model to preferences directly. Reading them after Sutton and Barto, you can see which parts of each method are reinforcement learning and which are not.

### Foundations

Prove, count and compute: induction, number theory, graphs, sums and asymptotics, counting and probability, with the calculus and linear algebra that learning needs.

1. **CS.01 — Mathematics for Computer Science** — Eric Lehman, F. Thomson Leighton and Albert R. Meyer
2. **02 — Calculus, Volume 1** — OpenStax
3. **03 — Linear Algebra** — Jim Hefferon
4. **04 — Calculus, Volume 2** — OpenStax
5. **06 — Calculus, Volume 3** — OpenStax

### Systems and robotics

See computing inside devices: specification, hardware, system software, real-time scheduling and validation, then robots that sense, move, localize and map.

1. **CS.02 — Eingebettete Systeme: Grundlagen Eingebetteter Systeme in Cyber-Physikalischen Systemen** — Peter Marwedel (in German)
2. **CS.03 — Elements of Robotics** — Mordechai Ben-Ari and Francesco Mondada

### Machine learning

Learn from data: classical supervised and unsupervised methods, deep networks, and reinforcement learning from bandits to policy gradients.

1. **CS.04 — Maschinelles Lernen** — Matthias Thimm (in German)
2. **28 — Understanding Deep Learning** — Simon J. D. Prince
3. **CS.05 — Reinforcement Learning: An Introduction** — Richard S. Sutton and Andrew G. Barto

### Language models and alignment

Read the language-model literature: pre-trained models and their uses, then two papers on fitting a model to feedback.

1. **CS.06 — Foundation Models for Natural Language Processing: Pre-trained Language Models Integrating Media** — Gerhard Paaß and Sven Giesselbach
2. **CS.07 — Constitutional AI: Harmlessness from AI Feedback** — Yuntao Bai and others (Anthropic), paper
3. **CS.08 — Direct Preference Optimization: Your Language Model is Secretly a Reward Model** — Rafael Rafailov and others, paper

**Why this order works**

Lehman, Leighton and Meyer come first because every later book assumes their sentences. An algorithm's correctness is an induction, its cost is a sum, and a learning method's guarantee is a statement about probability. The calculus volumes and Hefferon follow on the same stage, and they are there for one reason each: a gradient is a derivative of a function of many variables, and a layer of a network is a matrix. Calculus Volume 2 stands between the two others because series and the Taylor remainder come before several variables. Thimm's first chapter reviews linear algebra, analysis, optimization and probability, but a review is not a course.

Systems and robotics come before learning on purpose. A learning algorithm runs on a machine, and Marwedel's book says what that machine is: a specification, hardware with timing and energy limits, system software, scheduling that meets deadlines, and validation that has to happen before the device ships. Ben-Ari and Mondada then put the computation into a robot. Localization and mapping need probability that CS.01 has just provided, and the book's last chapters already teach neural networks and machine learning on small robots, a first look at the next stage. Marwedel's book is in German. A reader without German can go straight to Ben-Ari and Mondada; an English open-access edition of Marwedel's book exists separately and is not part of this library.

Thimm comes before Prince because the classical methods give the vocabulary: a loss, a training and a test set, overfitting and regularization, a kernel, a cluster and how to evaluate one. His chapters on reinforcement learning and deep learning are a preview of the two books that follow. Prince's networks are then compositions of maps whose training is optimization, and Sutton and Barto need both what came before: value functions are expectations, and the later chapters approximate them with parameterized functions and learn policies by gradients. Thimm's book is in German. A reader without German loses the classical methods but can read Prince and Sutton and Barto without it.

The language-model stage is last because each of its works assumes the books before it. Paaß and Giesselbach assume the transformer, which Prince explains. The two papers assume a policy, a reward and a penalty that keeps the trained model close to where it started, which is reinforcement learning in Sutton and Barto's terms. Constitutional AI comes before Direct Preference Optimization because it keeps the reinforcement-learning stage and changes where the feedback comes from; Direct Preference Optimization then changes the training itself. Its appendix derives the new objective from the old one, and that derivation is the mathematics this stage asks you to reproduce.

**How to study**

Write proofs by hand before you read the book's solution, and turn every algorithm into a small program you can run. In the systems and robotics books, sketch the timing or the sensor readings before you trust a design. From the learning stage on, implement a small version of each method, change one assumption at a time, and keep a short log of what changed. Read the two papers as arguments: write down the objective, the assumptions and the experiments that support each claim.

**Companions**

Use C.01 Dive into Deep Learning alongside Thimm (CS.04) and Prince (28) for code. Grinstead and Snell (08) takes probability further than CS.01, and Suh (24) is the optimization book behind the training chapters. The AI Research path continues into learning theory and statistics. CS.02 and CS.04 are in German.

## Optional companions

These enrich the main paths; they are not extra compulsory stages.

- **C.01 — Dive into Deep Learning** — Aston Zhang, Zachary C. Lipton, Mu Li and Alexander J. Smola. Read alongside **28**.
- **C.02 — Probabilistic Machine Learning: Advanced Topics** — Kevin P. Murphy. Read alongside **26, 28, 29, 30**.
- **C.03 — Classical Numerical Methods in Scientific Computing** — Jos van Kan, Guus Segal, Fred Vermolen and Hans Kraaijevanger. Read alongside **23**.
- **C.04 — Mathematics of Machine Learning** — Philippe Rigollet. Read alongside **29**.

Path order comes from [catalog.json](catalog.json). This file is the path guide and is kept in step with the study-direction text in the app. The chapter-by-chapter essays for all 58 books and papers are on their own pages in [docs/books](books/).
