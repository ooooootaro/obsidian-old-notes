##### Intro
Typical T2* ~ 50ms -> need TR~ 250ms for “natural” spoiling
Reduce TR to improve the speed?-> rapid GRE with appropriate spoiling (TR ≪ T2 < T1)

To make gradient echo faster (shorter TR), we need active spoiling methods since we can't wait for natural decay of transverse magnetization.
Two main types of spoiling:

- RF spoiling (varying RF phase)
- Gradient spoiling (additional gradients to diphase spins)

### Main
![[Pasted image 20241224123802.png]]
![[Pasted image 20241224123926.png]]
### Balanced SSFP
![[Pasted image 20241224123953.png]]
![[Pasted image 20241224124223.png]]

...略

Banding artifacts
- bSSFP has freq-dep null bands 
- spatially varying field inhomogeneity 
- shim not perfect 
- worse at high field (e.g., 3 T vs 1.5 T) 

Mitigating banding artifacts
- reduce TR 
- custom shim; shift center freq 
- phase cycling

![[Pasted image 20241224124447.png]]

Advantages
- High SNR efficiency 
- Gx and Gz first moments nulled 
Challenges
- Field homogeneity 
- TR 
- SAR 
- Catalyzation 
- Bright fat

### Gradient-spoiled GRE
![[Pasted image 20241224124023.png]]

End-of-TR gradient spoiler 
- typically on Gx and/or Gz 
- Range of β within each voxel 
- Mxy is a complex sum of all spins

Contrast depends on T1 and T2

![[Pasted image 20241224124723.png]]

略


Image characteristics
- no banding (averaged in voxel) 
- SSFP-FID: T2/T1 contrast 
- SSFP-Echo: more T2 contrast 
- sensitive to motion / flow / diffusion

When all gradients are balanced
- SSFP-FID and SSFP-Echo coalesce 
- T2 instead of T2* weighting 
- Balanced SSFP!!!