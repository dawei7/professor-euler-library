# C.01 Dive into Deep Learning

License: CC BY-SA 4.0; code Apache 2.0 · Source: <https://d2l.ai/d2l-en.pdf> · 1151 pages, 551 exercises in the prepared bundle

*Aston Zhang, Zachary C. Lipton, Mu Li and Alexander J. Smola*

## What this book trains

Dive into Deep Learning, by Aston Zhang, Zachary C. Lipton, Mu Li and Alexander J. Smola, is the working companion to Prince. The same ideas are built, trained and measured. The book opens with a motivating example and the kinds of learning problems, then reviews data, linear algebra, calculus, automatic differentiation, and probability. Linear networks for regression and for classification come before multilayer perceptrons. A builders’ guide treats layers, parameters and GPUs as objects you manage. Convolutional networks run from the fully connected layer to LeNet, and the modern chapter names AlexNet, VGG, NiN, GoogLeNet, batch normalization, ResNet and ResNeXt, and DenseNet. Recurrent networks, LSTMs and GRUs, attention and transformers, optimization, computational performance, computer vision, two chapters of natural language, reinforcement learning, Gaussian processes, hyperparameter search, generative adversarial networks, and recommender systems follow. An appendix collects the mathematics the formulas use.

The companion is optional. It does not replace Prince (28).

## Why it is worth knowing

A formula can hide a shape error, a learning rate that diverges, or a metric that does not measure the claim. Running the model makes those failures visible, and the book is written so that a from-scratch implementation and a concise one sit next to each other. You see which lines are the mathematics and which lines are the framework.

Softmax regression is multiclass classification with a normalizing constant. A convolution reuses weights across positions. Attention is queries, keys and values. The transformer chapter then stacks self-attention, and the pretraining chapter shows BERT as one use of that stack. Residual networks and densely connected networks are different answers to the same practical question: how a gradient survives a deep composition. Optimization includes convexity, so the nonconvex training of a network is compared with a case you can prove. Reinforcement learning is a Markov decision process, value iteration and Q-learning, a small precise chapter rather than a slogan. Gaussian processes are the nonparametric neighbor, here as a chapter of their own.

## What it asks of the other books

Prince (28) is the mathematical text this companion serves. Calculus in several variables (06), linear algebra (03 or 07), and a first probability course (08) are what the preliminaries review. Suh (24) helps the optimization chapter, which discusses convexity and gradient methods in the same spirit. You can code from this book before finishing Bach (29). The generalization theorems remain Bach’s job.

The license recorded in the catalog is CC BY-SA 4.0 for the text, with code under Apache 2.0. The companion is not required for any path. Read it beside book 28.

## A walk through the chapters

### 1. Front matter

Front matter is the title, preface, installation and notation. The introduction is a motivating example, the key components, the kinds of machine learning problems, the roots, the road to deep learning, success stories, and a statement of what the authors take the essence to be.

### 2. Preliminaries

Preliminaries are data manipulation, data preprocessing, linear algebra, calculus, automatic differentiation, probability and statistics, and documentation. Linear neural networks for regression cover linear regression itself, an object-oriented implementation, synthetic data, a from-scratch version, a concise version, generalization, and weight decay. Linear neural networks for classification cover softmax regression, the image-classification dataset, a base classification model, both implementations, generalization in classification, and environment and distribution shift.

### 3. Multilayer perceptrons

Multilayer perceptrons cover the model, its implementation, forward and backward propagation with computational graphs, numerical stability and initialization, generalization, dropout, and a house-price prediction exercise. The builders’ guide covers layers and modules, parameter management, initialization, lazy initialization, custom layers, file input and output, and GPUs.

### 4. Convolutional neural networks go from fully connected layers to convolutions, then images, padding and stride, multiple channels, pooling, and LeNet

Convolutional neural networks go from fully connected layers to convolutions, then images, padding and stride, multiple channels, pooling, and LeNet. Modern convolutional neural networks are AlexNet, networks using blocks (VGG), network in network, multi-branch networks (GoogLeNet), batch normalization, residual networks and ResNeXt, densely connected networks, and a chapter on designing the architecture.

### 5. Recurrent neural networks

Recurrent neural networks cover sequences, text as sequence data, language models, the recurrent net from scratch and in concise form, and backpropagation through time. Modern recurrent networks are long short-term memory, gated recurrent units, deep and bidirectional recurrent nets, a machine-translation dataset, the encoder–decoder architecture, sequence-to-sequence learning, and beam search.

### 6. Attention mechanisms and transformers

Attention mechanisms and transformers cover queries, keys and values, attention pooling, scoring functions, Bahdanau attention, multi-head attention, self-attention and positional encoding, the transformer architecture, transformers for vision, and large-scale pretraining.

### 7. Optimization algorithms

Optimization algorithms cover the relation of optimization to deep learning, convexity, gradient descent, stochastic and minibatch stochastic gradient descent, momentum, Adagrad, RMSProp, Adadelta, Adam, and learning-rate scheduling. Computational performance covers compilers, asynchronous computation, automatic parallelism, hardware, training on multiple GPUs, and parameter servers.

### 8. Computer vision

Computer vision covers augmentation, fine-tuning, object detection and anchor boxes, multiscale detection, single-shot detection, region-based convolutional networks, semantic segmentation, transposed convolution, fully convolutional networks, neural style transfer, and two competition-style image tasks. Natural language pretraining covers word embeddings, approximate training, global vectors, subword embedding, analogy, and BERT with its pretraining dataset. Natural language applications cover sentiment analysis with recurrent and convolutional nets, natural language inference with attention, and fine-tuning BERT.

### 9. Reinforcement learning

Reinforcement learning is the Markov decision process, value iteration, and Q-learning. Gaussian processes are priors and inference. Hyperparameter optimization is the search, including asynchronous and multi-fidelity variants. Generative adversarial networks include the deep convolutional case. Recommender systems are an overview. Appendix A is the mathematics: geometry and linear algebra, eigendecompositions, single-variable, multivariable and integral calculus, random variables, maximum likelihood, distributions, naive Bayes, statistics, and information theory. Appendix B is the tooling. References close the book.
