---
title: RNN review paper notes
subtitle:  

# Summary for listings and search engines
summary: "Notes on the paper: A Critical Review of Recurrent Neural Networks for Sequence Learning (Lipton and Berkowitz) - 
about RNN architectures, algorithms, results, comparison to alternative methodologies on sequence learning."
# Link this post with a project
projects: []

# Date published
date: "2018-06-13T00:00:00Z"

# Date updated
lastmod: "2020-12-13T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- paper

categories:
- reading
---

# Reading notes of [A Critical Review of Recurrent Neural Networks for Sequence Learning](https://arxiv.org/pdf/1506.00019.pdf).

## Main Idea
Answered the question of **Why recurrent neural networks?** in aspects of Architectures, algorithms, results, comparison to alternative methodologies on sequence learning.
- RNNs are able to manage text sequences of arbitrary lengths. While processing each token/element in the sequence one at a time, they pass information across time steps.
	- SVM, logistic regression and feedforward networks proved to be useful under independece assumption which precludes modeling long-range dependencies.
	- HMM has memeoryless property and has exponentially growing state space even when considering large context window which is computationally impractical for modelling long-range dependencies. 
	- RNNs are differentiable end to end given fixed architectures and regularization techniques can be used for preventing overfitting.

## Neural Nets and RNNs
- Neural nets: Neurons in the neural networks has values equal to the output of the activation function applied on the weighted sum of the input nodes' values: $ v_{j} = l_{j}(\sum_{j'}w_{jj'}\cdot{v_{j'}})$, which was then written as  $ v_{j} = \sigma(a_j)$ 
where $a_j = \sum_{j'}w_{jj'}\cdot{v_{j'}}$ and $\sigma$ for sigmoid. And activation functions are task-specific, for example, softmax are normally used in multiclass problems.
- Feedforward and backprop
	- Goal of feedforward NNs: minimize loss function: $L(\hat{y}, y)$.
	- Backprop for training: calculate derivatives of the loss function $L$ wrt the parameters of the network. Parameters are then updated by stochastic gradient descent (SGD), i.e. take steps of modifications towards the expecting direction which decreases the loss $L$. Note, loss function may be non-convex, thus global optimal is not gauranteed
- RNNs: takes both current input $\mathbf{x}^{(t)}$ and hidden state from previous $\mathbf{h}^{(t-1)}$: 
	- $h^{(t)} = \sigma(W^{hx}\mathbf{x}^{(t)}+W^{hh}\mathbf{h}^{(t-1)} + \mathbf{b}_h)$ 
	- $\hat{\mathbf{y}}^{t}= softmax(W^{yh}\mathbf{h}^{(t)} + \mathbf{b}_y)$ 
With above forward network, backprop of RNN is called Backprop through time (BPTT).
- Exploding/vanishing gradients: When learning long-distance dependencies, the gradients of weights may explode or vanish through the time steps. The following tutorial also gives a  detailed description. [Neural Machine Translation and Sequence-to-sequence Models: A Tutorial](https://arxiv.org/abs/1703.01619).

## LSTMs, GRUs, Bidirectional
A memory cell and gates are introduced in LSTM, which has unit gradient when adding previous memory $\mathbf{c}_{t-1}$ to the current $\mathbf{c}_t$.
Bidirectional structure has one more layer of hidden nodes which takes inputs from the end, which allows context information before and after the current step. 

Gated recurrent units (GRUs) appear as a simpler and computationally easier alternative of LSTM, which was not introducted in this paper but has on par performance as LSTM.

## Neural Turing Machines
Incorporate external memory buffer compared to RNNs. 
- Memory matrix +  controller(may be a rnn)
- differentiable end-to-end
- can backprop via SGD
- outperforms LSTM (without external memory) when generalizing on longer inputs.

## Applications
- representing natural language inputs and outputs
	- character-level, word level, one-hot, word embeddings 
- BLEU score for translation evaluation
	- vrevity penalty, ngram precisions
	- METEOR as an alternative which is based on word to word matches
- translation as a SEQ2SEQ problem
- image captioning:  input images and target captions as inputs. Encoding can be dong using CNN for images. Attention mechanism can be used in decoding.
- More: handwriting recognition, unsupervised video encoding, video captioning, computer programs reading.

### discussion
I don't include most of the equations in the notes. The paper is clear in why and how RNN makes a difference in learning long-dependencies, which serves pretty well as a review/tutorial from a higher level with math well explained.








