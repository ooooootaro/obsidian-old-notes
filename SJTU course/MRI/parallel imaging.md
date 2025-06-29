![[Pasted image 20241226202008.png]]
##### claude
This is related to the Nyquist sampling theorem and how k-space sampling affects MRI image reconstruction. Let me explain why the image appears "folded" or has reduced FOV when using skipped k-space lines:

1. When you undersample k-space by skipping lines (as shown in part b), you're effectively reducing the sampling rate in the phase-encoding direction by a factor of R=2.

2. According to the Nyquist sampling theorem, reducing the sampling rate leads to aliasing in the spatial domain after Fourier transformation. In MRI terms:
- The sampling interval in k-space (Δk) is inversely related to the field of view (FOV)
- When you double the distance between k-space lines (2Δk), you halve the FOV in the corresponding spatial dimension

3. The image appears folded because:
- The reduced sampling rate causes signal from outside the reduced FOV to "wrap around" or "alias" into the image
- Information from the top half of the original FOV gets superimposed onto the bottom half
- This is why you see what appears to be a half-sized, overlapped version of the brain image

This is a fundamental consequence of the Fourier relationship between k-space and image space. To avoid this folding artifact, you would need to either:
- Sample k-space fully (as in part a)
- Use parallel imaging techniques with multiple receiver coils
- Restrict the imaging FOV to only cover the region of interest
- Apply anti-aliasing techniques during reconstruction

The Chinese text asks "Why does sampling every other line in frequency domain result in halving the FOV in time domain?" - and this is precisely because of the reciprocal relationship between sampling density in k-space and FOV in image space, as described above.

##### aliasing
![[Pasted image 20241226202525.png]]


Signal equation and its solution
![[Pasted image 20241226202933.png]]
matirx已知


**SENSE: Sensitivity Encoding for Fast MRI** 
very robust