inversely estimate 
Flow-induced phase is proportional to flow velocity
However,
1. here is a background phase in the image
2. the background phase is not a constant.(because of the B0 inhomogeneity)
Therefore, we cannot directly use image phase to infer velocity.

[[M1]]
However, we can acquire two images that have
The same background phase and Direct phase accrual due to different M1.
![[Pasted image 20241225143210.png]]
Note: if the flow-induced phase difference is larger than 2p, phase aliasing will occur.
##### explain
Let me explain this flow imaging concept step by step:

1. Why We Need Two Images:
- Background tissue has some inherent phase (due to field inhomogeneities, etc.)
- We want to measure ONLY the phase caused by flow
- Solution: Take two images and subtract them

2. Looking at Background Pixels (Top Row):
- Both images have the same background phase
- When we subtract them, background phase cancels out
- Result: No phase difference (flat arrow)
- This automatically removes background noise!

3. Looking at Vessel Pixels (Bottom Row):
- Both images have:
  * Same background phase (just like background pixels)
  * DIFFERENT flow-induced phase (because we used different M1 values)
- When we subtract:
  * Background phase cancels out
  * Flow-induced phase difference remains
- Result: Phase difference proportional to flow velocity

4. Warning Note:
- If flow is too fast, phase difference might exceed 2π
- This causes phase aliasing (velocity wrap-around)
- Need to choose appropriate M1 values to avoid this

### Velocity Encoding: venc
![[Pasted image 20241225143445.png]]
##### explain
Looking at the equations in the slide:

1. From the phase difference equation:
Δφflow = γ(M1b - M1a)v = γΔM1v

2. The VENC equation:
VENC = π/γΔM1

3. And the velocity equation:
v = VENC·Δφ/π

Key points that show VENC can be positive or negative:
- When velocity v is positive: 
  * Phase difference Δφ is positive
  * v = +VENC when Δφ = +π
- When velocity v is negative:
  * Phase difference Δφ is negative
  * v = -VENC when Δφ = -π

So while the VENC equation shows π/γΔM1 (seems positive), the actual velocity measurement range is ±VENC because:
- Phase difference Δφ can be either positive or negative (-π to +π)
- This maps to velocities from -VENC to +VENC

Does this help explain why VENC represents both positive and negative velocity limits?

### [[Phase Contrast 待看]]