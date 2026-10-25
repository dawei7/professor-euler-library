# 29 Learning Theory from First Principles

License: CC BY-NC-ND 4.0 · Source: <https://www.di.ens.fr/~fbach/ltfp/> · 709 pages, 209 exercises in the prepared bundle

*Francis Bach*

## What this book trains

Francis Bach’s Learning Theory from First Principles separates three reasons a learning method can fail. Approximation: the family of functions cannot get close to the target. Optimization: the algorithm did not find a good member of the family. Generalization: a good member on the sample is not good on a fresh draw. The book is the mathematical account of that split, from linear least squares and empirical risk minimization through optimization, local averaging, kernels, sparsity, neural networks, ensembles, online learning and bandits, overparameterized models, structured prediction, probabilistic methods and lower bounds.

Overparameterized models are the chapter where a model has more parameters than samples and the old warning that it must overfit stops being the whole story. Lower bounds say when a method is not merely unlucky but information-theoretically short of data.

## Why it is worth knowing

Empirical risk minimization picks the hypothesis that looks best on the sample. A uniform law of large numbers says the sample risk and the true risk stay close for every hypothesis in a class at once, provided the class is not too large. The size is a combinatorial or analytic measure, the descendant of Levin’s counting. Without that uniform control, a method can look perfect on the data it was scored on and say nothing about the next point.

Kernel methods lift a linear algorithm into a space of functions without writing the features down, using only inner products. Sparse methods bet that most coefficients should be zero. Ensembles average many weak rules. Bandits are the online problem in which you only observe the loss of the action you chose. Each chapter is a different answer to the same three-way split. The pleasure is finishing a chapter and knowing which of the three failures it closed, and which it left open.

## What it asks of the other books

Prince (28), on the AI path, so the neural-network chapter refers to models you have seen. The book allows reading relevant chapters beside Prince if you would rather meet the theory early. Suh (24) for convex optimization. Polyanskiy (25) and the inference book (26) for probability and estimation. Linear algebra (07) for least squares, kernels and the spectral facts inside a kernel matrix. Levin (05) for the counting instinct behind a hypothesis class.

Rigollet (C.04) is the optional compact lecture companion, with solved assignments, beside this book. Shalev-Shwartz and Ben-David, in the personal-download notes, is the classical PAC and VC alternative. Bach remains the path book because it starts from optimization after the models. Samworth and Shah (30) take the statistical side into high dimension and nonparametric estimation.

## A walk through the chapters

### 1. After the preface, Mathematical Preliminaries collect the analysis, linear algebra and probability the arguments quote

After the preface, Mathematical Preliminaries collect the analysis, linear algebra and probability the arguments quote. Introduction to Supervised Learning sets the risk, the sample, and the three-way split. Linear Least-Squares Regression is the model whose optimization is a linear system and whose generalization can be computed. Empirical Risk Minimization is the general principle. Optimization for Machine Learning is how the minimizer is sought: gradients, convexity, and the rates a step size can promise.

### 2. Local Averaging Methods predict by smoothing neighbors

Local Averaging Methods predict by smoothing neighbors. Kernel Methods replace explicit features by a positive definite kernel. Sparse Methods seek solutions with few nonzeros. Neural Networks return to compositions of the kind Prince studied, now with approximation and generalization statements. Ensemble Learning combines predictors. From Online Learning to Bandits drops the assumption that the whole sample is in hand before the first prediction.

### 3. Overparameterized Models treat the regime of more parameters than observations

Overparameterized Models treat the regime of more parameters than observations. Structured Prediction is the case where the output is a sequence, a tree or another object with its own loss. Probabilistic Methods put a distribution on the prediction or on the parameters. Lower Bounds prove that some accuracies are impossible for a given sample size, no matter how clever the algorithm. The conclusion and the references close the book.
