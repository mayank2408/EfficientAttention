# EfficientAttention
1. In this work, we propose a multi-level attention mechanism that has better time complexity than the standard attention mechanism.
2. In our technique, we represent the input sequence using different levels where the first level is the hidden states obtained by running an LSTM over the input sequence. And the length of vectors in the subsequent level decreases by a constant factor. Using this level structure we can describe the input compactly where each level contains coarser details than the previous level.
3. For each decoder time stamp, we will start by attending to the top-most level representation of input and will subsequently go down a particular branch based on the computed attention scores.
4. We propose three different approaches to get the representation of input sequence:
    - RNN
    - CNN
    - ACT(Adaptive Computation Time)
