##### Intro
As you can see, no matter how we choose to vary our gradient, we are essentially creating different ways to sample the k-space.
If we do not consider constraints such as [[gradient slew rate]] and [[eddy currents]], the faster we can sample up the k-space, the faster we can finish our scan. 

EPI is one of the example to accelerate scan by using one trajectory to finish sampling the entire k-space. However, EPI still samples k-space along the Cartesian grid. 

Since the energy of image spectrum usually falls more in the central k-space, can we sample more densely in the central k-space and coarsely in **peripheral** k-space to accelerate the imaging? The answer is yes → it leads to several well-known non-Cartesian trajectories

### Main
- Radial sampling
	![[Pasted image 20241223200914.png]]
- Spiral sampling
	![[Pasted image 20241223220214.png]]
- 