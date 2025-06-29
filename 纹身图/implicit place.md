latent diffusion -> stable diffusion
利用图像像素冗余的特性，训练一个自编码器将图像压缩到潜空间，然后在潜空间进行扩散操作。潜变量的尺寸通常只有原图的1116-1/196，从而可以极大的提高训练和推理效率

deficit
图像压缩存在信息损失，对于需求精细像素表示的复杂场景(例如高清街景)，解码器输出的图片可能出现比例失真、肢体扭曲等现象，使得生成图片的保真度不足。


### stable AI stable cascade
Stage C:16x24x24的latent feature(相比于1024x1024，压缩比达到42倍)Stage B和Stage A-起充当VAE中的decoder角色，将图片从隐空间恢复到像素空间，同时拥有大的分辨率由于使用了StageC的输出作为StageB的输入，因此StageB可以使用更少的步长达到更好的结果
![[Pasted image 20250205130536.png]]