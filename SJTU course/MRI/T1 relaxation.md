Longitudinal Relaxation, or Spin-lattice Relaxation. 
T1 relaxation reflects the regrowth of longitudinal magnetization (Mz)

The time constant is called T1 relaxation time/rate.
![[Pasted image 20241205214908.png]]

Through the use of inversion pulse or saturation pulse, one can create T1 contrast. Overall, longer T1 causes inadequate regrowth, leading to low Mz that can be transformed into Mxy by RF pulses


#蛤 
- Inversion recovery
	线圈也采集mz方向？！！！不该是T1长的higher signal嘛
	![[Pasted image 20241205133716.png]]
- partial [[saturation]] and T1-weighted contrast
	![[Pasted image 20241205133738.png]]
	



###### Fast Imaging using Low Angle Shot (FLASH)
![[Pasted image 20241205133835.png]]
Key Features of FLASH:

1. Spoiled Gradient Echo:

- Uses gradient spoiling to destroy remaining transverse magnetization
- Ensures clean slate for next TR period
- Prevents interference between successive signals

2. Short TR & Small Flip Angles:

- Uses partial flip angles (usually <90°) to maintain steady state
- Short TR allows for rapid imaging
- Results in some signal saturation but enables fast scanning

FLASH is popular because it:

- Provides rapid imaging
- Offers good tissue contrast
- Is less sensitive to motion artifacts
- Uses less RF power than spin echo sequences