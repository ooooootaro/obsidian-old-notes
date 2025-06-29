Stable Diffusion Sampler.
Stable Diffusion的基本原理是通过降噪的方式(如完全的噪声图像)，将一个原本的噪声信号变为无噪声的信号(如人可以理解的图像)。其中的降噪过程涉及到多次的采样，采样的系数在KSampler中配置:
- seed:控制噪声产生的随机种子
- control after generate:控制seed在每次生成后的变化
- steps:降噪的迭代步数，越多则信号越精准，相对的生成时间也越长
- cfg: classifier free guidance决定了prompt对于最终生成图像的影响有多大。更高的值代表更多地展现prompt中的描述
- denoise: 多少内容会被噪声覆盖
- sampler name、scheduler:降噪参数


Sampler使用总结
1. 如果你希望更快的、收敛的、新的且质量高的sampler，可以尝试下DPM++2M Karras1.20-30步、UniPC with 20-30 步
2. 如果你想获得高质量的图像，并不关心是否收敛，可以使用DPM++SDEKarras，10-152.步 (这种方法比较慢)，DDIM，10-15 步
3. 如果你希望获得稳定、可复现的图像，不要使用带a的方法。3.
4. Euler和Heun作为简单尝试是个好的方法。后者可以使用更少的步数。