<p align="center">
    <img alt="AI Engineering Interview Questions and Answers" src="https://github.com/amitshekhariitbhu/llm-internals/blob/main/assets/banner.png">
</p>

# LLM Internals

**Learn LLM internals step by step - from tokenization to attention to inference optimization.**

---

Prepared and maintained by the **Founder** of Outcome School: [Amit Shekhar](https://x.com/amitiitbhu)

---

**Note: This series will continue to grow as I write more blogs and create more videos on new topics. Keep learning.**

---

## Large Language Models (LLMs)

Before diving into the internals of an LLM, it’s a good idea to first understand what an LLM actually is.

In this video, we will cover the following:

* LLM
* RAG
* MCP
* Agent
* Fine-tuning
* Quantization

Let's get started: [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)

---

## Tokenization in Large Language Models (LLMs)

In this video, we will learn about Tokenization and why they are essential for Large Language Models.

Let's get started: [Tokenization in Large Language Models (LLMs)](https://www.youtube.com/watch?v=sK2s9I84EVI)

---


## Byte Pair Encoding in LLMs

In this blog, we will learn about BPE (Byte Pair Encoding) - the tokenization algorithm used by most modern Large Language Models (LLMs) to break text into smaller pieces before processing it.

We will understand what BPE is, why it is needed, and how it works step by step with a simple example.

We will cover the following:

* What is Tokenization?
* The Problem: How to Break Text into Tokens?
* What is BPE (Byte Pair Encoding)?
* How BPE Works: Step by Step
* How BPE Tokenizes New Text
* Why BPE is Used in Modern LLMs

Let's get started: [Byte Pair Encoding in LLMs](https://outcomeschool.com/blog/bpe-in-llms)

---

## Math behind Attention - Q, K, and V

In this blog, we will learn about the math behind Attention: Query(Q), Key(K), and Value(V) with a step-by-step numeric example.

We will cover the following:

* The Attention Formula
* Setting Up: From Words to Vectors
* Creating Q, K, and V Matrices
* Computing Attention Scores (Q x K^T)
* Scaling the Scores
* Applying Softmax
* Computing the Final Output (Attention Weights x V)
* Putting It All Together

Let's get started: [Math behind Attention - Q, K, and V](https://outcomeschool.com/blog/math-behind-attention-qkv)

---

## Math behind √dₖ Scaling Factor in Attention

In this blog, we will learn about why we scale the dot product attention by √dₖ in the Transformer architecture with a step-by-step numeric example.

We will cover the following:

* The Attention Formula (Quick Recap)
* What Happens Without Scaling?
* Why Do Dot Products Grow with dₖ?
* Understanding Variance of the Dot Product
* Proving It Step by Step: Variance of the Dot Product is dₖ
* What Large Dot Products Do to Softmax
* Why √dₖ is the Right Scaling Factor
* Seeing It with Real Numbers
* Putting It All Together

Let's get started: [Math behind √dₖ Scaling Factor in Attention](https://outcomeschool.com/blog/scaling-dot-product-attention)

---

## Causal Masking in Attention

In this blog, we will learn about causal masking in attention.

We will start with the introduction of causal masking, understand the problem of seeing future tokens through an example, and then walk through its implementation to see how masked attention prevents the model from accessing future tokens.

We will cover the following:

* Without Causal Masking
* With Causal Masking
* Implementation of Causal Masking
* The Causal Mask Matrix

Let's get started: [Causal Masking in Attention](https://outcomeschool.com/blog/causal-masking-in-attention)

---

## Math Behind Backpropagation

In this blog, we will learn about the math behind backpropagation in neural networks.

Backpropagation is the core algorithm that allows neural networks to learn from their mistakes. Without it, training neural networks efficiently would not be possible. Understanding the math behind it gives us a deeper understanding of how neural networks actually learn. Do not worry, we will learn about each concept step by step so that everything is clear.

We will cover the following:

* What is backpropagation?
* The chain rule of calculus
* Forward pass
* Loss calculation
* Backward pass (backpropagation)
* Step-by-step numeric example
* Weight update using gradient descent
* Backpropagation in Python

Let's get started: [Math Behind Backpropagation](https://outcomeschool.com/blog/math-behind-backpropagation)

---

## Math Behind Cross-Entropy Loss

In this blog, we will learn about the math behind Cross-Entropy Loss with a step-by-step numeric example.

When we train a classification model in machine learning, the model predicts probabilities for each class. For example, given an image, the model outputs something like: "I am 70% sure this is a cat, 20% sure it is a dog, and 10% sure it is a rabbit." To train the model, we need a way to measure how wrong these predictions are compared to the true answer. This is exactly what Cross-Entropy Loss does. It is the most widely used loss function in classification tasks, and it powers the training of almost every modern AI model, including GPT, BERT, and image classifiers.

We will cover the following:

* The Big Picture
* What is Cross-Entropy
* The Cross-Entropy Loss Formula
* Why We Take the Negative Log
* Binary Cross-Entropy Loss
* Categorical Cross-Entropy Loss
* Step-by-Step Numeric Example
* Cross-Entropy Loss for Language Models
* The Gradient of Cross-Entropy Loss
* Quick Summary

Let's get started: [Math Behind Cross-Entropy Loss](https://outcomeschool.com/blog/math-behind-cross-entropy-loss)

---

## Decoding Transformer Architecture

In this blog, we will learn about the Transformer architecture by decoding it piece by piece - understanding what each component does, how they work together, and why this architecture powers every modern Large Language Model (LLM).

We will cover the following:

* Why the Transformer was needed
* The two halves of the architecture
* Tokenization, Embedding, and Positional Encoding
* The Attention Mechanism and Multi-Head Attention
* Feed-Forward Networks, Residual Connections, and Layer Normalization
* How the Encoder and Decoder work
* How data flows through the entire architecture
* The three variants of the Transformer
* Why the Transformer is so powerful

Let's get started: [Decoding Transformer Architecture](https://outcomeschool.com/blog/decoding-transformer-architecture)

---

## Feed-Forward Networks in LLMs

In this blog, we will learn about Feed-Forward Networks in LLMs - understanding what they are, how they work inside the Transformer architecture, why every Transformer layer needs one, and what role they play in making Large Language Models so powerful.

We will cover the following:

* What is a Feed-Forward Network?
* Understanding Feed-Forward Networks with a Real-World Analogy
* Where Does the Feed-Forward Network Sit in a Transformer?
* How Does a Feed-Forward Network Work - Step by Step
* The Expand-then-Contract Pattern
* Why Does the FFN Expand and Then Contract?
* ReLU and Activation Functions
* What Does the Feed-Forward Network Actually Learn?
* How Much of the Model is the Feed-Forward Network?
* Feed-Forward Networks in Mixture of Experts
* Why Feed-Forward Networks Are So Important

Let's get started: [Feed-Forward Networks in LLMs](https://outcomeschool.com/blog/feed-forward-networks-in-llms)

---

## KV Cache in LLMs

In this blog, we will learn about KV Cache - where K stands for Key and V stands for Value - and why it is used in Large Language Models (LLMs) to speed up text generation.

We will start with how LLMs generate text one token at a time, understand the role of Key, Value, and Query inside the model, see the problem of repeated computation through an example, and then walk through how KV Cache solves this problem by storing and reusing past results.

We will cover the following:

* How LLMs Generate Text
* What Happens Inside the Model
* The Problem: Repeated Computation
* The Solution: KV Cache
* Why Only Key and Value Are Cached, Not Query
* How Much Faster Does It Get
* The Trade-Off: Speed vs Memory

Let's get started: [KV Cache in LLMs](https://outcomeschool.com/blog/kv-cache-in-llms)

---

## Paged Attention in LLMs

In this blog, we will learn about Paged Attention, a technique that solves the memory waste problem of KV Cache, allowing LLMs to serve many more users at the same time.

We will start with a quick recap of KV Cache, understand the memory problem it creates, see how traditional memory allocation wastes space through an example, and then walk through how Paged Attention solves this problem by borrowing an idea from how computers manage memory.

We will cover the following:

* Quick Recap: KV Cache
* The Problem: Memory Waste in KV Cache
* What is Paged Attention?
* How Paged Attention Works
* Why Paged Attention Is So Effective
* Memory Sharing Across Requests

Let's get started: [Paged Attention in LLMs](https://outcomeschool.com/blog/paged-attention-in-llms)

---

## Decoding Flash Attention in LLMs

In this blog, we will learn about Flash Attention by decoding it piece by piece - understanding why standard attention is slow, what makes Flash Attention fast, how it uses GPU memory cleverly, and why it is used in almost every modern Large Language Model (LLM).

We will cover the following:

* A quick recap of standard attention
* Why standard attention is slow
* How GPU memory actually works (HBM vs SRAM)
* The core idea behind Flash Attention
* Tiling: breaking the work into small blocks
* Online softmax: computing softmax without the full matrix
* Recomputation in the backward pass
* Flash Attention 2
* Flash Attention 3
* Advantages and impact of Flash Attention

Let's get started: [Decoding Flash Attention in LLMs](https://outcomeschool.com/blog/decoding-flash-attention)

---

## Mixture of Experts Explained

In this blog, we will learn about the Mixture of Experts (MoE) architecture - understanding what experts are, how the router picks them, why MoE makes large models faster and cheaper, and why it powers many of today's most powerful Large Language Models (LLMs).

We will cover the following:

* Why Mixture of Experts was needed
* What an "expert" really means
* The router and how it picks experts
* Where MoE sits inside a Transformer
* Sparse activation and why it saves compute
* Load balancing across experts
* Advantages and challenges of MoE
* Why MoE powers many modern LLMs

Let's get started: [Mixture of Experts Explained](https://outcomeschool.com/blog/mixture-of-experts)

---

## Grouped Query Attention

In this blog, we will learn about Grouped-Query Attention (GQA) and how it differs from Multi-Head Attention (MHA). We will also learn about Multi-Query Attention (MQA) along the way and see when to use which one.

We will cover the following:

* The Big Picture
* Quick Recap: Multi-Head Attention (MHA)
* The Problem with Multi-Head Attention
* What is Multi-Query Attention (MQA)?
* What is Grouped-Query Attention (GQA)?
* How Grouped-Query Attention Works
* GQA is a Generalization of MHA and MQA
* GQA vs MHA vs MQA
* Real-World Use Cases
* A Note on Terminology
* Uptraining: Converting MHA to GQA
* Quick Summary

Let's get started: [Grouped Query Attention](https://outcomeschool.com/blog/grouped-query-attention)

---

## Math Behind RoPE (Rotary Position Embedding)

In this blog, we will learn about the math behind Rotary Position Embedding (RoPE) and why it is used in modern Large Language Models.

We will cover the following:

* The Big Picture
* Why a Transformer Needs Position Information
* Older Approaches and Their Problems
* The Core Idea Behind RoPE
* The 2D Rotation Math
* How RoPE Is Applied to Q and K
* Why the Dot Product Captures Relative Position
* A Small Numeric Example
* Real-World Use Cases
* Quick Summary

Let's get started: [Math Behind RoPE (Rotary Position Embedding)](https://outcomeschool.com/blog/math-behind-rope-rotary-position-embedding)

---

## Harness Engineering in AI

In this blog, we will learn about Harness Engineering in AI. We will understand what a harness is, why we need it, and how it is used in AI Agents and evaluation systems.

We will cover the following:

* What is a Harness in AI?
* Why do we need Harness Engineering?
* Components of an AI Harness
* Harness Engineering for AI Agents
* Harness Engineering for Evaluation
* Best Practices in Harness Engineering
* Putting It All Together

Let's get started: [Harness Engineering in AI](https://outcomeschool.com/blog/harness-engineering-in-ai)

---

## More blogs and videos coming soon!

### License
```
   Copyright (C) 2026 Outcome School

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
