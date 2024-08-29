# Transformer from Scratch

This repository contains a PyTorch implementation of each component of a Transformer, built from scratch.

## Components

- **InputEmbedding**: Converts input tokens (integers) into continuous vector representations.

- **PositionalEncoding**: Adds positional information to embeddings using sine and cosine functions of different frequencies to encode positions.

- **MultiHeadAttention**: The core of the Transformer, applying self-attention using queries, keys, and values derived from the input. The attention is divided into multiple heads, allowing the model to focus on different aspects of the input.

- **FeedForward**: A simple feed-forward neural network applied to each position separately, consisting of two linear transformations with a ReLU activation between them.

- **TransformerBlock**: Combines multi-head attention and a feed-forward network, along with layer normalization and residual connections.

- **Transformer**: The full model, combining all the above components. It applies input embedding and positional encoding, then passes the result through a stack of TransformerBlocks.

## Usage

To use this implementation, clone the repository and run the provided scripts:

```bash
git clone https://github.com/yourusername/transformer_from_scratch.git
cd transformer_from_scratch
python main.py

