最大方差最佳全局阈值选取法(Otsu法) 也叫大津法, 1979年由日本学者大津提出； 
一般而言，图像中目标或背景内的像素灰度相近，而背景和目标之间往往存在较大的差异，因此，合理的图像分割结果应该体现出
**区域内部的相似性和不同区域之间的差异性**

### 算法

![[58f1092cc7ef4f59b8f3fac06166aaa.jpg]]
![[a0884ec971b9e84b8664737b8ede972.jpg]]
[OTSU算法详解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/111101737#:~:text=%E7%94%A8%E5%BC%8F%EF%BC%888%EF%BC%89%EF%BC%8C%E5%AF%B9%E4%BA%8E%20k%3D0%2C1%2C2%2C...%2CL-1%EF%BC%8C%E8%AE%A1%E7%AE%97%E7%B1%BB%E9%97%B4%E6%96%B9%E5%B7%AE%20sigma_%20%7BB%7D%5E%20%7B2%7D%20%28k%29%20%E3%80%82%20%E5%BE%97%E5%88%B0OTSU%E9%98%88%E5%80%BC,%7B%2A%7D%20%E5%80%BC%E3%80%82%20%E5%9C%A8%20k%3Dk%5E%20%7B%2A%7D%20%E5%A4%84%E8%AE%A1%E7%AE%97%E5%8F%AF%E5%88%86%E6%80%A7%E5%BA%A6%E9%87%8F%20eta%20%E3%80%82)
![[fe388a2e5f8b97ba02fb016829c749d.jpg]]


### more

![[Pasted image 20240107013113.png]]
![[Pasted image 20240107013046.png]]
but（P1数太少）![[Pasted image 20240107013207.png]]
‘ 
### 边缘信息改进全局阈值处理
（P1数太少）
ex：多发性极化，单点就是很小，so必要借助边缘信息![[Pasted image 20240107013723.png]]
![[6acc50eccee331364a69a0a7bc50371.jpg]]
![[Pasted image 20240107013829.png]]



## more and more
### Otsu二阈值处理
![[Pasted image 20240107014153.png]]
###  Otsu多阈值处理
![[Pasted image 20240107014021.png]]
