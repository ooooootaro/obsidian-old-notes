### Main
After excitation, every spin is tipped down towards the same direction (perpendicular to B1’ field). Thus, when the RF pulse stops, every spin is pointing along the same direction in the xy-plane.

	![[Pasted image 20241222203007.png]]
##### Now consider a FID sequence, in which only Gx is turned on after the RF pulse
![[Pasted image 20241222213726.png]]
![[Pasted image 20241222213812.png]]

##### Now consider a more realistic frequency-encoding gradient waveform.
![[Pasted image 20241222213901.png]]
![[Pasted image 20241222214010.png]]
That's why we definitely need a pre-phasor & gradient-echo sequence中需要spoiler

##### Now let’s also add the phase encoding gradient.
During the pre-phasing period, both gradients are turned on. 
What happens mathematically?
![[Pasted image 20241222214108.png]]
![[Pasted image 20241222214119.png]]
![[Pasted image 20241223010849.png]]
(since has kx all the time)
![[Pasted image 20241223011524.png]]
![[Pasted image 20241223011637.png]]
Note that here we assume each time when a new TR starts, we always start from k=0! Typically this is done by spoiling, by moving existing Mxy “out of k-space”.

##### More than rectangular gradient--[[non-Cartesian trajectory]]

### Questions and Discussion
Why should we always sample the k-space at steady state? (Firstly using Cartesian sampling as an example)

If I change my k-trajectory during transient states each time when I image the same object, would image artifacts be the same? 


If you can figure out the answers, it means you are able to mix Bloch equation and k-space sampling to think about how signal variations will affect image quality in MRI. Congratulations! This is essentially how most MR physicists think about pulse sequences and MRI

### The relationship between spin echo and k-trajectory
Recall the gradient waveform for a spin-echo sequence:
![[Pasted image 20241223155517.png]]
You use positive gradient to go to k = +1
The 180° pulse hits and INSTANTLY flips your position to k = -1
Now you can use another positive gradient to move from k = -1 back to k = 0
It's like someone picked up your car and turned it around - you can keep driving forward to get back!
![[Pasted image 20241223155612.png]]
Therefore in a spin-echo sequence with Cartesian sampling, the k-trajectory is like:
![[Pasted image 20241223155758.png]]
