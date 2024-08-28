# transformer_from_scratch

each component of Transformer with PyTorch implementation:

InputEmbedding: This layer converts input tokens (represented as integers) into continuous vector representations.
PositionalEncoding: This adds positional information to the embeddings. It uses sine and cosine functions of different frequencies to encode position.
MultiHeadAttention: This is the core of the Transformer. It applies self-attention using queries, keys, and values derived from the input. The attention is split into multiple heads, allowing the model to focus on different aspects of the input.
FeedForward: This is a simple feed-forward neural network applied to each position separately, consisting of two linear transformations with a ReLU activation in between.
TransformerBlock: This combines multi-head attention and a feed-forward network, along with layer normalization and residual connections.
Transformer: This is the full model, combining all the above components. It applies the embedding and positional encoding, then passes the result through a stack of TransformerBlocks.
