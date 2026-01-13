# **LLM-dataset-challenge-4**
📘 Challenge 4 — Mini Transformer Block

## Welcome to Challenge 4 of the LLM Micro Challenge Series!
In the previous challenge you built embeddings (token meaning).
Now you will build the Transformer Block, which gives tokens context.

This is the core component inside every modern LLM (GPT, BERT, LLaMA, etc).

🚀 What You Will Build

## A complete Mini Transformer Block containing:

✔ Multi-Head Self-Attention
Allows tokens to interact with each other.

✔ Layer Normalization
Stabilizes training and prevents exploding activations.

✔ Residual Connections
Enable deep models and stable gradient flow.

✔ Feed-Forward Network (FFN)
Processes each token embedding to transform information.

This block is the engine that drives language models.

📂 Repository Structure
Challenge4-transformer-block/
│
├── src/
│   ├── transformer_block.py
│   ├── attention.py
│   ├── feedforward.py
│   └── __init__.py
│
├── examples/
│   └── run_example.py
│
├── tests/
│   └── test_transformer.py
│
├── assets/
│   ├── architecture_diagram.png   (optional)
│   └── output_sample.txt
│
├── requirements.txt
└── README.md

## 🧠 How the Transformer Block Works

A Transformer Block consists of two major sub-layers:

## 1️⃣ Multi-Head Self-Attention

This layer allows each token to "look" at every other token and decide:
Which words are important
How much attention to give each word

It uses:

Query (Q)
Key (K)
Value (V)
Scaled dot-product attention
Multiple heads to capture multiple types of relationships

## 2️⃣ Feed-Forward Network (FFN)

A two-layer MLP applied on every token independently.
This increases model capacity by transforming each token’s representation.

## 3️⃣Residual Connections

Each sub-layer returns:
output = LayerNorm(x + sublayer(x))

This stabilizes training and lets information flow deeper.

## 4️⃣ Layer Normalization

Applied after each residual addition to avoid exploding/vanishing gradients.
🏁 Deliverables for Challenge 4

## Your submission should include:

✔ Transformer block Python code
✔ README file (this file)
✔ Output sample from example script
✔ Clean repo structure
## 🎯 Learning Outcome

After this challenge, you understand:
How self-attention works
How Transformer blocks process embeddings
How residuals + layernorm help stabilize deep models
These concepts are the foundation of LLMs, ChatGPT, BERT, LLaMA, GPT-NeoX, and more.
