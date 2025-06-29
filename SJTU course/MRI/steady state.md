![[Pasted image 20241206074959.png]]
![[Pasted image 20241206075201.png]]
#蛤
![[Pasted image 20241206075233.png]]
Also, notice that 𝑀^𝑛 0+ becomes constant starting at n=2. 
We say the magnetization enters the steady state ( 稳态) if 𝑀𝑛 0+ does not change anymore. 

**Therefore, for a saturation recovery sequence, the magnetization enters steady state very quickly.**
So far, we did not say how we acquire the Mxy signal.

### Saturation recovery spin-echo sequence
![[Pasted image 20241206075517.png]]
### Saturation recovery GRE sequence
In saturation recovery sequences, the magnetization rapidly enters the steady state.
However, this is not always the case


Before we perform the calculation, note that the magnetization will reduce in the early TRs, because of the partial saturation
![[Pasted image 20241222151810.png]]

类似数学归纳法
![[Pasted image 20241222151852.png]]
Plug this into the previous equation, we can derive the steady state magnetization to be
![[Pasted image 20241222151929.png]]
### Ernst Angle
In MRI, usually we acquire signal at the steady-state. This is because if we acquire from the beginning, different k-space lines will be sampled with different signal magnitude, which would cause image artifacts (伪影). 

Therefore, how many TRs before we enter the steady state is critical. The signal at the steady state is also critical, because it determines the SNR. 
Notice that the SS-signal for the gradient echo sequence is a function of flip angle. Can you determine at what flip angle is the maximal signal attained?

![[Pasted image 20241222152155.png]]

![[Pasted image 20241222152228.png]]

For interested students, you can read Chapters 7 & 9 from Zhi-Pei Liang’s book for more information

#蛤
![[Pasted image 20241222195842.png]]