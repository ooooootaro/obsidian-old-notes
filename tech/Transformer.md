
- Transformer有一個我們一直無法解決的問題
- Transformer Alternative是一個熱門研究領域
- 其中一個SSM，最近開始受到比較多的關注


### category

[[GPT (Generative Pre-trained Transformer)]]

The original Transformer, introduced by Vaswani et al. in 2017, was designed for sequence-to-sequence tasks like machine translation. 
It uses self-attention mechanisms to process sequential data.

[[DiT ( Diffusion Transformer)]], introduced by Microsoft Research in 2023, specifically adapts the Transformer architecture for image generation using diffusion models. 
It replaces the convolutional neural networks (CNNs) typically used in diffusion models with a modified Transformer architecture that:

1. Processes images as sequences of patches (similar to Vision Transformers)
2. Incorporates time embeddings to handle the diffusion process
3. Uses a specialized architecture optimized for the denoising task in diffusion models

So while DiT uses the core concepts from Transformers (like self-attention and positional embeddings), it's better thought of as a specialized adaptation rather than just a branch. 
It's specifically designed to merge the benefits of Transformers with diffusion models for image generation, rather than being a general-purpose sequence processing architecture like the original Transformer.
