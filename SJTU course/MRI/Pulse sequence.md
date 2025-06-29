### concept
The goal of MRI is to acquire Fourier transform of the image, which is called k-space in MRI world.
To do it, we need to add different initial phases and carrier frequencies to signal at each location. Note that the Fourier transform is given by
![[Pasted image 20241205124401.png]]
#蛤 (n - N/2)
![[Pasted image 20241205124511.png]]

Essentially we need the precession frequency and phase of spins to linearly vary as a function of x and y! What hardware in MRI can do that? [[gradient coil]]

### example

![[Pasted image 20241205124711.png]]
Repeat [[TR]]（time of repetition)  many times to sample k-space line-by-line

![[Pasted image 20241205131837.png]]
This is called a pulse sequence!
##### MR is a slow imaging technique!

Scan time = TR x NPE x NEX 
		NEX = Number of excitations (i.e., averages)
