Aka Spin-spin relaxation: decay of **transverse magnetization** arising from natural interactions at the atomic or molecular levels.
- Each spin is a magnetic field and affects spins nearby.
- Spins are changing their location due to e.g. Brownian motion.
Therefore, dephasing such is a non invertible and always exists.


Both reflect decay of transverse magnetization (Mxy) after excitation.
Both follow a decaying exponential model.

Through the use of spin echo or gradient echo acquisition, one can create T2 or T2* contrast. 
Longer T2 or T2* leads to reduced decay, thus higher signals when acquisition is performed.
![[Pasted image 20241205210050.png]]
1/T2* = 1/T2 + 1/T2’ 
	T2’: extra signal dephasing caused by local field inhomogeneity



[[Refocusing Pulses 重聚焦脉冲]]
![[Pasted image 20241205133119.png]]
如果我们没有refocusing pulse，同样时间点采集数据，我们得到的信号存在什么weighting？→ 这个序列就叫做gradient echo sequence
#蛤 为啥f方向不一样


##### T2 of normal tissue
T2 relaxation time is the time constant of the mono-exponential decay
Different tissues have different T2 relaxation time because density of the spins are different. 
比如，固体状的组织通常比液体状的组织拥有 更短的T2弛豫时间
