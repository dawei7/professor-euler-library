# 28 Understanding Deep Learning

License: CC BY-NC-ND 4.0 · Source: <https://udlbook.github.io/udlbook/> · 622 pages, 197 exercises in the prepared bundle

*Simon J. D. Prince*

## What this book trains

Simon J. D. Prince’s Understanding Deep Learning is the curriculum’s account of modern neural networks. Supervised learning, shallow networks and the universal approximation theorem, deep networks as compositions, loss functions built from maximum likelihood, gradient descent and its stochastic and adaptive forms, backpropagation and initialization, the measurement of error, and regularization. Convolutional networks, residual networks, and transformers, including encoder, decoder and encoder–decoder examples. Then the generative family: adversarial networks, normalizing flows, variational autoencoders and diffusion models. Reinforcement learning. A chapter asks why deep learning works. Another treats ethics. Appendices collect notation, the mathematics and the probability the formulas use.

A network is a composition of linear maps and simple nonlinearities. Training chooses parameters to make a loss small on a sample. The book keeps those two sentences visible while the architectures grow.

## Why it is worth knowing

Universal approximation says a shallow network can approximate a continuous function on a compact set. It does not say the approximation is easy to find, or that a deep composition is not a better practical parameterization. The book is careful about that gap. Double descent, in the chapter on measuring performance, is the modern observation that adding parameters past the point of interpolation can make test error fall again. Residual connections are a structural answer to an optimization failure, a path through the network that can carry a gradient.

A transformer’s self-attention is a data-dependent weighted average, and the weights are a softmax of scaled dot products. That sentence is linear algebra plus the logistic normalizing constant. BERT, GPT-3 and a translation model appear as examples of what the same block can be wired to do, not as a product tour. Diffusion models and flows are ways to turn a simple noise distribution into a complicated data distribution by a process you can write down. The ethics chapter is part of the book’s own contents, beside the mathematics rather than instead of it.

## What it asks of the other books

Calculus in several variables (06) and linear algebra (03, 07), because a layer is a matrix and a gradient is a derivative. Suh (24) for gradient descent, convexity and the knowledge of what is lost when the network is not convex. Probability (08) and enough statistics to read a likelihood. The mathematics and probability appendices are a repair. They are not a substitute for Axler or for Polyanskiy. Prince does not require Gallager.

Bach (29) is the next book on the AI path: approximation, optimization and generalization, with this book’s models in view. Dive into Deep Learning (C.01) is the coding companion. Bishop, named in the personal-download notes, is the probabilistic generation beside this one. Prince remains the deep-learning book.

## A walk through the chapters

### 1. The introduction distinguishes supervised, unsupervised and reinforcement learning, and points at ethics, the structure of the book and how to read it

The introduction distinguishes supervised, unsupervised and reinforcement learning, and points at ethics, the structure of the book and how to read it. Supervised learning gives the overview and a linear-regression example, so the later networks are regressions with a richer function class.

### 2. Shallow neural networks state the universal approximation theorem and the notation for several inputs and outputs

Shallow neural networks state the universal approximation theorem and the notation for several inputs and outputs. Deep neural networks compose those units, write the composition with matrices, and compare shallow and deep parameterizations. Loss functions derive the objective from maximum likelihood: univariate regression, binary classification, multiclass classification, and cross-entropy. Fitting models is gradient descent, stochastic gradient descent, momentum and Adam. Gradients and initialization cover backpropagation and the scale of the initial weights. Measuring performance separates sources of error, including double descent. Regularization treats explicit penalties, implicit effects of the algorithm, and the heuristics people actually use.

### 3. Convolutional networks

Convolutional networks are invariance and equivariance, in one and two dimensions, with downsampling and upsampling. Residual networks add skip connections, batch normalization, and the question of why the skip helps. Transformers process sequences by dot-product self-attention, then stack layers. The examples are an encoder (BERT), a decoder (GPT-3), an encoder–decoder translation model, and the extensions to long sequences and to images.

### 4. The generative and sequential chapters follow

The generative and sequential chapters follow: unsupervised learning, generative adversarial networks, normalizing flows, variational autoencoders, diffusion models, and reinforcement learning. Why does deep learning work? is its own chapter, after the architectures rather than before them. Deep learning and ethics follows. Notation, a mathematics appendix, a probability appendix, the bibliography and the index close the book.
