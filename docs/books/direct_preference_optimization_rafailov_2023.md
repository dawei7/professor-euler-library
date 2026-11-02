# CS.08 Direct Preference Optimization: Your Language Model is Secretly a Reward Model

License: CC BY 4.0 · Source: <https://arxiv.org/abs/2305.18290> · 27 pages, 0 exercises in the prepared bundle

*Rafael Rafailov, Archit Sharma, Eric Mitchell, Stefano Ermon, Christopher D. Manning and Chelsea Finn*

## What this book trains

Direct Preference Optimization is a research paper, presented at NeurIPS 2023, not a textbook. It starts from the usual RLHF pipeline: supervised fine-tuning, a reward model fitted to human choices between two responses, and reinforcement learning that maximizes that reward while a KL-divergence penalty keeps the policy near a reference model. The paper replaces the last two steps by one maximum-likelihood objective on the policy itself, a binary cross-entropy loss over preference pairs. No reward model is trained, and nothing is sampled from the policy during fine-tuning.

The key step is a change of variables. The KL-constrained objective has a closed-form optimum, the reference policy reweighted by the exponential of the reward over β and normalized by a partition function Z(x). Solved for the reward, this gives β times the log ratio of optimal to reference policy, plus β log Z(x). The Bradley–Terry model uses only the difference of two rewards for one prompt, so Z(x) cancels, and a preference’s probability depends only on the policy and the reference. Hence the title: the policy, read against the reference, is itself a reward model.

## Why it is worth knowing

The derivation is short enough to check line by line, and it turns reinforcement learning into classification. The gradient raises the likelihood of the preferred response and lowers that of the other, weighted by how wrongly the implicit reward orders the pair. Without that weight, the paper reports, the model can degenerate, and its unlikelihood samples repeat one word.

In Section 5, rewards that differ by a function of the prompt alone induce the same preferences and the same optimal policy, and Theorem 1 says every such class contains a reward of DPO’s form. The normalizing term is read as a soft value function. Without it a policy gradient can have high variance, which RLHF meets with a learned value function or a human-written baseline. DPO’s reward needs no baseline.

The claims rest on three tasks with models of up to 6 billion parameters. On IMDb sentiment generation, where a classifier is the true reward, DPO reaches the highest reward at every KL, ahead of PPO even when PPO is given the true reward. On Reddit TL;DR summarization GPT-4 prefers DPO’s summaries to the reference ones about 61 percent of the time at temperature 0, PPO’s at best 57 percent. On single-turn dialogue from Anthropic’s Helpful and Harmless data, DPO is the only computationally efficient method that improves on the preferred responses. A human study finds that GPT-4 agrees with people about as often as people agree with each other.

## What it asks of the other books

Sutton and Barto (CS.05) for policies, rewards and policy gradients, including REINFORCE with a baseline and the actor–critic methods that Section 5.2 diagnoses. Paaß and Giesselbach (CS.06) for language models, fine-tuning and InstructGPT. Prince (28) for transformers and for deriving a classification loss from maximum likelihood, the shape of the DPO loss. Probability (08 or CS.01) for conditional distributions and expectations. Murphy (C.02) treats the KL divergence in its information-theory chapter.

On the Computer Science & AI path the paper ends the last stage, Language models and alignment, after CS.06 and beside Constitutional AI (CS.07), and closes the Computer science & AI shelf. The two are read as a pair. Both start from RLHF. Constitutional AI replaces human harmlessness labels by AI feedback guided by principles. DPO keeps the preference data and removes the reward model and the reinforcement-learning loop. Its related work cites Constitutional AI for preference data a language model generates from a text rubric. The license recorded in the catalog is CC BY 4.0.

## A walk through the chapters

The paper prints no exercises, so its bundle carries the PDF and its contents and no exercise frames. Its appendix carries out derivations that a careful reader can first attempt on their own sheet: the optimum of the KL-constrained objective (A.1), the DPO loss from Bradley–Terry (A.2), its gradient (A.4) and the two lemmas (A.5).

### Sections 1–5

Sections 1 to 3 state the problem, survey related work and review the RLHF pipeline. Section 4 derives the DPO objective, reads its gradient and outlines the method. Section 5 states Definition 1, Lemmas 1 and 2 and Theorem 1 with a proof sketch, then analyses the instability of actor–critic algorithms.

### Sections 6–7

Section 6 sets out the tasks, the GPT-4 evaluation and baselines such as PPO and Best of N, and adds news articles as a new input distribution. Section 7 names open questions: generalization, reward over-optimization, larger models, and win rates that depend on GPT-4’s prompt.

### Appendices A–D

Appendix A holds the derivations, with the Plackett–Luce version for rankings, the proof of Theorem 1 and Proposition 1, that each class has exactly one reward of DPO’s form. Appendix B prints a short PyTorch function for the loss and the default hyperparameters. Appendix C gives the IMDb set-up, the GPT-4 prompts and the unlikelihood samples. Appendix D shows Best of N for several N, sample responses with GPT-4’s judgments, and the human study.
