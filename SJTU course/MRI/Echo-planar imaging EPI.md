one of the fastest imaging methods in MRI
Fast imaging applications: 
- Functional MRI (fMRI) 
- Diffusion(弥散) Imaging 
- Perfusion (灌注) Imaging 
- Cardiac imaging 
Fast and Faster
- Dynamic imaging 
- Real-time imaging
![[Pasted image 20241223200201.png]]
Freq Encoding (FE) and phase encoding (PE) in flash EPI
![[Pasted image 20241223200414.png]]
### Gradient-Echo EPI
![[Pasted image 20241223200501.png]]
What contrast you get if TR>>T1, and TE=50ms?

### Spin-Echo EPI (T2 contrast)
![[Pasted image 20241223200529.png]]

### EPI is motion insensitive
![[Pasted image 20241223200553.png]]


### Adding a 180° refocusing pulse to EPI

When we say "single excitation" in EPI, we specifically mean one 90° excitation pulse that moves magnetization into the transverse plane.

The 180° pulse is a refocusing pulse, not an excitation pulse:
    - It doesn't bring new magnetization into the transverse plane
    - It simply flips/reverses the existing transverse magnetization**


From claude
Let me break down the benefits of adding a 180° refocusing pulse to EPI:

1. Spin Echo Contrast:

- The 180° pulse flips the spin phases
- This reverses the effects of T2* dephasing
- Results in T2 contrast instead of T2* contrast
- T2 contrast is often preferred for clinical imaging because it's less affected by local field inhomogeneities

2. Reduced Susceptibility Effects:

- Susceptibility effects are artifacts caused by magnetic field variations at tissue interfaces (like air/tissue boundaries)
- These variations cause spins to diphase faster (T2* decay)
- The 180° refocusing pulse helps recover signal lost to these field inhomogeneities
- This means less signal dropout and distortion in areas prone to susceptibility artifacts (like the brain base near sinuses)

So while basic EPI is very fast but susceptible to these artifacts, adding a 180° refocusing pulse (making it Spin-Echo EPI) helps:

- Get more reliable contrast (T2 vs T2*)
- Reduce image distortions
- Improve signal in problematic areas

The trade-off is a slightly longer acquisition time due to waiting for the spin echo to form.