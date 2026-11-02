# CS.06 Foundation Models for Natural Language Processing: Pre-trained Language Models Integrating Media

License: CC BY 4.0 · Source: <https://doi.org/10.1007/978-3-031-23190-2> · 448 pages, 0 exercises in the prepared bundle

*Gerhard Paaß and Sven Giesselbach*

## What this book trains

Gerhard Paaß and Sven Giesselbach’s Foundation Models for Natural Language Processing is a survey of pre-trained language models and of the large models that grew out of them. After a review of the classical tools, it explains three architectures through one representative each: BERT, an encoder trained to restore masked tokens; GPT, a decoder trained to predict the next token; and the transformer encoder–decoder for translation. A long chapter improves these models and another asks what they know. The rest is applications, information extraction and text generation, then speech, images, video, control, and DNA and protein sequences, and a closing chapter weighs what the models can do against the harm they can cause.

The book prints no numbered exercises. The library’s copy carries the full PDF and its contents but no exercise frames, so it is a reading book, and notes go on the learner’s own sheet.

It surveys a field that moves fast. The preface is dated July 2022 and the book appeared in 2023. Its rankings of the leading models and its benchmark tables describe that moment, not the present.

## Why it is worth knowing

Self-attention is the mechanism under almost every model in the book. Each token’s new embedding is a weighted average of value vectors, with weights from a softmax of scaled scalar products between queries and keys, so “bank” near “river” gets a different embedding from “bank” near “money”. Its cost grows with the square of the input length, and Section 3.2 collects remedies such as sparse attention and low-rank approximations. Pre-training needs no labels. Fine-tuning adapts a model with a small annotated set, adapters train a few added parameters, and few-shot prompts change none at all.

The section on InstructGPT is the bridge to the end of the path. A reward model is trained on human comparisons of generated answers, and the language model is then tuned by proximal policy optimization, which follows the policy gradient pattern. The book calls this process alignment to human preferences. Retrieval runs through the book as well, from dense passage embeddings and nearest-neighbor search to Retro, WebGPT and dialog systems that retrieve and filter.

The chapter on knowledge is a corrective. Benchmarks may not test all aspects of a task, a high score on a reasoning benchmark can come from word correlations rather than knowledge of the world, and published results often depend on conditions that are not reported. The last chapter lists harms, from biased or false statements and intentional misuse to the disclosure of private information and costs to society and the environment, and argues that a legal regulation of foundation models is necessary. Many sections end with links to available code and pre-trained parameters, as they stood in 2022.

## What it asks of the other books

The preface addresses readers familiar with the fundamentals of text and media processing; the foreword calls the book an overview for newcomers and a reference. Its mathematics is light and reviewed where it is used: the softmax, matrix products, conditional probabilities of the next token, and stochastic gradient descent. Hefferon (03) and Grinstead and Snell (08) cover the formulas. Prince (28) is the real preparation: its transformer chapter derives the block this book uses on every page, and its chapters on training and on diffusion models explain what Section 2.4 and Chapter 7 summarize. Dive into Deep Learning (C.01) is the coding companion. Sutton and Barto (CS.05) supply the states, rewards and policy gradients that the InstructGPT section and the section on control describe in a paragraph.

On the Computer Science & AI path the book opens the last stage, language models and alignment, after Thimm (CS.04), Prince and Sutton and Barto. The two papers that close the path follow: Constitutional AI (CS.07), which trains a harmless assistant from written principles, first by critiques and revisions and then by reinforcement learning from AI feedback, and Direct Preference Optimization (CS.08), which fits a language model to preferences directly, without a separate reward model or reinforcement learning. The license recorded in the catalog is CC BY 4.0.

## A walk through the chapters

### Chapters 1–2

Chapter 1 states the scope and reviews the classical tools: tokenization with byte-pair encoding and WordPiece, vector space models and the logistic classifier, nonlinear classifiers, static word embeddings, and recurrent and convolutional networks. Chapter 2 is BERT (self-attention, masked-token training, fine-tuning, computational cost), GPT (next-token training, generation, GPT-2) and the transformer for translation (cross-attention, beam search, evaluation). A section on training and assessment covers optimization, regularization, architecture search, uncertainty and explanation.

### Chapter 3

Chapter 3 improves the models. Other pre-training objectives give autoencoders such as RoBERTa and DeBERTa, autoregressive models such as GPT-3, Gopher, Chinchilla and PaLM, and encoder–decoders such as T5 and BART. Then come longer inputs, many languages, added knowledge, larger and smaller models, and fine-tuning by adapters, few-shot prompts, thought chains and instructions.

### Chapter 4

Chapter 4 measures what the models know: benchmark collections such as GLUE and SuperGLUE, probing classifiers for syntax, common sense and logical consistency, and the transferability and reproducibility of results.

### Chapters 5–6

Chapter 5 is information extraction: text classification, word sense disambiguation, named entity recognition and entity linking, and relation extraction. Chapter 6 is text generation: document retrieval, question answering, machine translation, summarization, text with a given style or plot, fake news and its detection, computer code, and dialog systems.

### Chapters 7–8

Chapter 7 moves to other media: speech and music; the Vision Transformer, text with images, and image generation, including diffusion models; video captioning, action recognition and generation; the Decision Transformer and GATO for control; and DNA and protein sequences. Chapter 8 summarizes the paradigm and its performance, discusses economic prospects and potential harms, and closes on advanced systems: innovative content, grounding language in the world, fast and slow thinking, and planning. An appendix on image sources and the index close the book.
