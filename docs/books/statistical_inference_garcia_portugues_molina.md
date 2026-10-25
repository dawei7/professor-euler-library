# 26 Statistical Inference

License: CC BY-NC-ND 4.0 · Source: <https://egarpor.github.io/SI-UC3M/> · 182 pages, 166 exercises in the prepared bundle

*Eduardo García-Portugués and Isabel Molina*

## What this book trains

Statistical Inference, by Eduardo García-Portugués and Isabel Molina, turns estimation and testing into a course with definitions, theorems and exercises. A point estimator is a function of the sample. Unbiased, invariant, consistent, sufficient, minimal sufficient, efficient and robust are different compliments, and they are not interchangeable. The method of moments and maximum likelihood are two ways to build an estimator. Confidence intervals are built from pivotal quantities, from normal sampling, from asymptotics, and from the bootstrap. Tests are built for normal populations, for two samples, for asymptotic regimes, and by the likelihood-ratio principle. Neyman–Pearson’s lemma is the optimality theorem for a simple hypothesis against a simple alternative.

The preliminaries review probability, random variables and random vectors, and transformations. The introduction fixes the vocabulary of a sample and recalls normal sampling distributions and the central limit theorem. Software and a license note sit in the welcome pages. The book is the classical-inference stage. It says so, and it is not an encyclopedia of every modern method.

## Why it is worth knowing

A sufficient statistic is a compression of the sample that loses nothing the model could have used. The factorization theorem tells you when you have found one. An efficient estimator meets the variance bound. A robust estimator does not collapse when the model is slightly wrong. Wanting all three at once is usually wanting too much, and the chapter exists so you can say which property a procedure actually has.

The likelihood is the probability of the sample as a function of the parameter. Maximum likelihood is the parameter that makes the sample least surprising. Asymptotic confidence intervals are what the central limit theorem gives you when the exact sampling distribution is unavailable. The bootstrap, already met in the modern-statistics book as a computational idea, returns here as a method with a place in the theory. The power of a test is the probability of detecting a false null. Neyman–Pearson says the likelihood ratio is the most powerful test of a given size. That is the jewel of the testing chapter.

## What it asks of the other books

Polyanskiy (25) for measure-theoretic probability, or a reader who can use the preliminaries chapter as a serious review after Grinstead and Snell (08) and the central limit theorem. Modern statistics (09) for the intuition of intervals, tests and the bootstrap on data. Linear algebra helps the random-vector sections. Calculus helps the transformations and the asymptotics.

Samworth and Shah (30) take regression and estimation into high dimension and nonparametric settings this book does not try to cover. Murphy (C.02) is the optional Bayesian and probabilistic-model companion after this foundation. This book remains the curriculum’s inference text.

## A walk through the chapters

### Chapter 1. Preliminaries

The welcome pages state the scope, the software, how to cite the book, the license, contributions and credits. Chapter 1, Preliminaries, reviews probability, random variables, random vectors and transformations of random vectors. A transformation of a random vector is a derived distribution. The exercises begin here and do not stop.

### Chapter 2. Introduction

Chapter 2, Introduction. Basic definitions of a statistical model and a sample, sampling distributions in normal populations, and the central limit theorem, with an appendix. The normal sampling distributions, chi-squared, Student’s t, and the F law, are the exact tools the later normal intervals will quote. The central limit theorem is the permission to proceed when the population is not normal and the sample is large.

### Chapter 3. Point estimation

Chapter 3, Point estimation. Unbiased estimators, invariant estimators, consistent estimators, sufficient statistics, minimal sufficient statistics, efficient estimators, and robust estimators, again with an appendix. Consistency is about the sample size tending to infinity. Unbiasedness is about the expectation at a fixed sample size. A procedure can be one without the other.

### Chapter 4. Estimation methods

Chapter 4, Estimation methods. The method of moments, and maximum likelihood. Moments match the sample’s averages to the model’s averages. Likelihood maximizes the joint density of the sample. The exercises are where the two disagree on a small example, which is the right place to see the difference.

### Chapter 5. Confidence intervals

Chapter 5, Confidence intervals. The pivotal quantity method, intervals for a normal population and for two normal populations, asymptotic intervals, and bootstrap intervals. A pivot is a function of the sample and the parameter whose distribution does not depend on the parameter. Solving the pivot for the parameter yields the interval.

### Chapter 6. Hypothesis tests

Chapter 6, Hypothesis tests. An introduction, tests for one normal population and for two, asymptotic tests, then the section the outline titles in the truncated form “6.5-value of a test,” then the power of a test and Neyman–Pearson’s lemma, and the likelihood-ratio test. The pages after the asymptotic examples discuss that value before the power section begins. The likelihood-ratio test compares the best likelihood under the alternative with the best likelihood under the null. It is the general procedure the earlier normal tests secretly were. References close the book.
