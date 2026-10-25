# 09 Introduction to Modern Statistics

License: CC BY-SA 3.0 · Source: <https://openintro-ims.netlify.app/> · 637 pages, 368 exercises in the prepared bundle

*Mine Çetinkaya-Rundel and Johanna Hardin*

## What this book trains

Introduction to Modern Statistics, second edition, by Mine Çetinkaya-Rundel and Johanna Hardin, asks what a dataset entitles you to say. The book moves from data and study design, through exploration of categorical and numerical variables, to linear and logistic regression, and then to inference: randomization tests, bootstrap confidence intervals, mathematical models, decision errors, and the classical inferences for proportions, means, tables and regression.

A study design is part of the mathematics. A random sample and a randomized experiment support different claims. An observational study can show association. A causal claim wants an experiment, or a set of assumptions you can point at. Simpson’s paradox, in the applications chapter on data, is the warning that an aggregate and a subgroup can tell opposite stories.

## Why it is worth knowing

Probability says what a model implies. Statistics says what the data imply about a model, and how loud the implication is allowed to be. A confidence interval is a procedure with a coverage property. A test is a procedure with an error probability. Decision errors, false positives and false negatives, are the chapter that keeps a significant result from being confused with an important one.

The modern half of the title is serious. Randomization and the bootstrap compute the inference by reusing the sample, before the mathematical-model chapter derives the same ideas from probability. Seeing both is the education. Linear regression with one predictor and with many, and logistic regression for a yes-or-no outcome, are the models the inference chapters then put uncertainty on. A fit without an interval is a picture. The interval is the claim.

## What it asks of the other books

Grinstead and Snell (08) for probability, expectation, variation and the central limit theorem. The mathematical-model chapter of this book leans on that theorem. Algebra and functions from the entry books. Calculus is the tool behind the probability course more than a daily tool here. Hefferon (03) helps the multiple-regression chapter, because a design matrix and a least-squares fit are linear algebra. The book can be read when matrices are still young. It becomes clearer after the line of best fit in Hefferon.

García-Portugués and Molina (26) turn estimation and testing into a theorem-driven course after measure-theoretic probability. Samworth and Shah (30) take regression into high dimension, where the intuition from this book’s low-dimensional pictures needs correction. This book is the place the pictures are formed.

## A walk through the chapters

### 1. Hello data, Study design, and Applications

Hello data, Study design, and Applications: Data. A case study on stents, the vocabulary of variables and observations, sampling, experiments, observational studies, and then a case study on the Olympic 1500 metres together with Simpson’s paradox. Interactive computing tutorials and R labs sit in the applications chapter. The statistical ideas do not depend on memorizing a language. They do depend on seeing data move.

### 2. Exploring categorical data, Exploring numerical data, and Applications

Exploring categorical data, Exploring numerical data, and Applications: Explore. Contingency tables, bar plots, proportions, pie charts and waffle charts. Scatterplots, means, histograms, variance and standard deviation, box plots, robust statistics, transformations, and maps. Robust statistics are the ones that do not collapse when a few observations are wild. A transformation can make a skewed measurement into one whose shape the later normal approximations recognize.

### 3. Linear regression with a single predictor, with multiple predictors, logistic regression, and Applications: Model

Linear regression with a single predictor, with multiple predictors, logistic regression, and Applications: Model. A line chosen to fit paired numerical data. Several predictors at once, where each coefficient is an effect holding the others in the model. Logistic regression when the outcome is a category and a straight line would predict impossible probabilities. The applications chapter asks you to communicate a model, not only to fit one.

### 4. Hypothesis testing with randomization, Confidence intervals with bootstrapping, Inference with mathematical models, Decision Errors, and Applications: Foundations

Hypothesis testing with randomization, Confidence intervals with bootstrapping, Inference with mathematical models, Decision Errors, and Applications: Foundations. Randomization builds a reference distribution by breaking the association the hypothesis denies. The bootstrap builds an interval by resampling the observations. The mathematical-model chapter connects those computational ideas to the central limit theorem and to named sampling distributions. Decision errors name the two ways a yes-or-no procedure can be wrong, and the trade between them.

### 5. Inference for a single proportion, two proportions, two-way tables, a single mean, two independent means, paired means, and many means

Inference for a single proportion, two proportions, two-way tables, a single mean, two independent means, paired means, and many means. Then Applications: Infer. These are the classical settings, now with the foundations in place. Paired means are not two independent samples. Many means are the analysis of variance: one question about several groups, not a pile of pairwise tests.

### 6. Inference for linear regression with one predictor, with multiple predictors, and for logistic regression, then Applications: Model and infer

Inference for linear regression with one predictor, with multiple predictors, and for logistic regression, then Applications: Model and infer. A coefficient is an estimate. The chapter supplies the interval and the test. Multiple predictors raise the question of which variables are doing the work, and of what “holding the others fixed” really fixed. The outline closes with a references appendix. The exercises throughout are part of the text, not an optional extra.
