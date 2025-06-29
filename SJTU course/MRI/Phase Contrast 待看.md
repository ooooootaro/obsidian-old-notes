![[Pasted image 20241225144436.png]]
##### claude 



### Phase-Contrast MR Angiography
For the vascular imaging, It requires 6 images to depict the vessels in any orientation.
![[Pasted image 20241225144720.png]]
##### claude
Let me explain why we need 6 images and how we can potentially reduce them:

1. Why 6 Images Initially:
- Need 2 images (±M1) for each direction (SS, PE, FE)
- This gives us velocity components in all 3 directions
- Total = 2 × 3 = 6 images

2. How to Reduce Measurements:
- Instead of acquiring separate +M1 and -M1 for each direction
- We can use one reference scan (no flow encoding) 
- Then combine it with one flow-encoded scan per direction
- This reduces total scans from 6 to 4:
  * 1 reference scan
  * 3 direction-encoded scans (SS, PE, FE)

3. The Math Works Because:
- Phase difference = Flow-encoded - Reference
- Rather than: (+M1) - (-M1)
- Both approaches give us the same velocity information
- But with fewer acquisitions

This optimization maintains the same information while reducing scan time by 33%.

### 啊啊
![[Pasted image 20241225145246.png]]
Let me explain this Phase Contrast MR Angiography process:

1. Acquisition Process (Left):
- Pulse sequence shows timing of RF and gradients
- Red dashed box highlights the flow encoding gradients
- Need to encode flow in all three directions (SS, PE, FE)

2. Direction-Specific Images (Right):
- SS (Slice Selection) image: Shows flow in through-plane direction
- PE (Phase Encoding) image: Shows flow in up-down direction
- FE (Frequency Encoding) image: Shows flow in left-right direction
- Speed image (bottom): Combines all directions

3. Speed Image Creation:
- For each direction, calculate phase difference from ±M1 pairs
- Speed = √(vSS² + vPE² + vFE²)
  * vSS = velocity in slice direction
  * vPE = velocity in phase direction
  * vFE = velocity in frequency direction

4. Result:
- Final speed image shows total flow magnitude regardless of direction
- Brighter pixels indicate faster flow
- Can see vessels clearly regardless of their orientation

This is why it's powerful for angiography - it captures all flow directions and combines them into a single comprehensive image.

##### 略5张slides

