Phase of Moving Spins
![[Pasted image 20241224132123.png]]

Phase Evolution Along Readout
![[Pasted image 20241224132341.png]]
![[Pasted image 20241224132508.png]]

Velocity Profile of Flow in A Tube
![[Pasted image 20241224132729.png]]

### Flow-Induced Phase Shift
![[Pasted image 20241224132815.png]]

##### Flow Compensation Along Readout
![[Pasted image 20241224132915.png]]
Derive the phase of moving spins as a function of time from t= 0 to t=4t. 
Prove that the phase becomes zero at echo center t= 4t. 
Also, think about why can’t we use two lobes to realize flow compensation?
###### claude
me help derive this step by step.

1. First, let's understand what causes phase accumulation:
    - Phase φ(t) = γ ∫G(t')·v·t' dt'
    - Where γ is gyromagnetic ratio, G is gradient, v is velocity
2. Let's break down the gradient moments from t=0 to t=4τ:
    - First lobe (0 to τ): G
    - Middle period (τ to 3τ): -G
    - Final lobe (3τ to 4τ): G
3. For moving spins, phase accumulation for each period: From t=0 to t=4τ: φ(t) = γv(∫(0 to τ) G·t dt + ∫(τ to 3τ) (-G)·t dt + ∫(3τ to 4τ) G·t dt)
4. Let's solve each integral:
    - First lobe: γvG(t²/2)₀ᵗ = γvGτ²/2
    - Middle period: -γvG(t²/2)ᵗ³ᵗ = -2γvGτ²
    - Final lobe: γvG(t²/2)³ᵗ⁴ᵗ = γvGτ²/2
5. Total phase at t=4τ: φ(4τ) = γvG(τ²/2 - 2τ² + τ²/2) = -γvGτ² = 0

As for why we can't use just two lobes for flow compensation:

1. Two lobes would only null the 0th moment (position)
2. For flow compensation, we need to null both 0th and 1st moments (position and velocity)
3. Three lobes provide the necessary degrees of freedom to simultaneously null both moments

##### Flow Comp: 2D Slice-Selection
![[Pasted image 20241224135409.png]]
Compensation for through-plane flow can be added along the slice selection. Prove that the phase becomes zero after this three-lobe combination #蛤

###### claude
Let me help derive this slice-selection flow compensation proof:

1. For this slice-selection gradient ( Gss ), we have three lobes:
    - First lobe: Amplitude A, duration τ₁
    - Second lobe: Amplitude -2A, duration τ₂
    - Third lobe: Amplitude A, duration τ₃
2. Key point: The arrow marks when spins are tipped (RF pulse center)
    - This divides the first lobe into two parts
    - Need to consider phase accumulation before and after this point
3. Let's write the phase equation: φ = γv∫G(t)·t dt
4. For moving spins, phase accumulation for each period:
    - Before RF center (first part of lobe 1): contributes nothing as spins aren't tipped yet
    - After RF center (second part of lobe 1): γvA·t dt from 0 to remaining τ₁
    - Middle lobe: γv(-2A)·t dt for duration τ₂
    - Final lobe: γvA·t dt for duration τ₃
5. For flow compensation to work:
    - The 0th moment (area) must sum to zero: A·τ₁ - 2A·τ₂ + A·τ₃ = 0
    - The 1st moment (area × time) must sum to zero

This gradient design ensures both position (0th moment) and velocity (1st moment) are compensated, resulting in zero net phase accumulation for moving spins.

##### The key differences and relations between Flow Compensation in Readout vs Slice-Selection
1. Timing Differences:

- Readout Flow Comp: Occurs after RF excitation, during signal acquisition
- Slice-Selection Flow Comp: Split around the RF pulse (some before, some after)

2. Purpose:

- Readout Flow Comp: Compensates for in-plane flow during readout to prevent phase errors in the signal
- Slice-Selection Flow Comp: Compensates for through-plane flow to ensure proper slice selection

3. Critical Moments:

- Readout: Must have zero phase at echo center (when data is collected)
- Slice-Selection: Must have zero phase after the complete gradient combination to ensure proper slice selection

4. Gradient Design:

- Readout: Generally bipolar with three lobes (G, -G, G)
- Slice-Selection: Three lobes (A, -2A, A) split around RF pulse

5. Major Difference:

- RF timing: In slice-selection, the RF pulse occurs during the first gradient lobe, making the timing and phase evolution more complex
- In readout, all gradients occur after RF excitation, making phase evolution more straightforward

The main relation is that both use three lobes to achieve both 0th and 1st moment nulling, but their implementations differ due to their different purposes and timing requirements relative to the RF pulse.


##### Flow Comp Along PE
#蛤 G fe why must G,-2G,G
![[Pasted image 20241224135952.png]]• Flow comp can be applied along the PE direction using a bipolar gradient pair. • TE will likely be increased due to the use of the bipolar gradient pair. Only two PE steps are shown here. 
• Why here we can use a two-lobe combination to null phase caused by motion?
![[Pasted image 20241224192356.png]]
					![[Pasted image 20241224193851.png]]
					![[Pasted image 20241224194418.png]]
					According to Fourier transform properties, a periodic signal in k-space produces replicas in image space. The spacing between replicas is related to the frequency of the phase error

## [[phase to flow]]

## [[Diffusion MRI 待看]]
