### basic
Similar to vision transformer of recognizing model
									![[Pasted image 20250205132523.png]]
 1. split the pic to a lot of patch
 2. transfer the series of patch to transformer blocks, gain each of the outcome
 3. unpatchify to 解构 the outcome, recover its original size


- sampling T
- category of the pic

ada LN-Zero
use conditioning to predict the "scaling" and "skewing" of the middle transformer block

[[FID]]
![[Pasted image 20250205133310.png]]


the more Transformer Gflops, the better the image fidelity
![[Pasted image 20250205133523.png]]

### use text as conditioning
(原始的DIT架构它只支持类别作为控制条件)
##### PixArt

additional **cross attention**

its KV is the feature of texting prompt
unlike DIT whose KS is sampling T and category


提出了3阶段的训练模式，大幅提高训练速

1. Pixel dependency learning
2. Text-image alignment learning 微调
3. High-resolution and aesthetic image generation 语义对齐

to ensure the velocity of converging while maintain good outcome
##### SD3 (Stable Diffusion 3)
Similar to in context conditioning from DIT
