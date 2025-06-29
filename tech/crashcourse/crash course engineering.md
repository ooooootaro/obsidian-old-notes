### norms
conversion转换率, yield产出率
accumulation
	mass: input - output
	molecules: generation, consumption
	![[Pasted image 20240406132759.png]]
	Whatever’s left over is what’s accumulated inside the system.
### reversibility
###### piston
![[Pasted image 20240406133555.png]]
![[Pasted image 20240406133650.png]]
#### work
- pressure-volume work
	![[Pasted image 20240406133916.png]]
	![[Pasted image 20240406133934.png]]

- shaft work, which is when a shaft轴 or propeller推进器/螺旋桨 rotates through a liquid or gas.
- electrical work, which is the work done on a charged particle by an electric field.

If a process is reversible, that means it can go back to its initial state and start over with no additional work input.
Everything is happening so slowly and gradually that you aren’t losing energy as heat, which means you don’t need to ‘add’ work to replace that lost energy.
You can use the same amount of work produced by the system to get it right back to where it started.
As an engineer, the goal is to figure out how close you can get a system to being reversible, while still **keeping it time, effort, and cost effective.** In this case, efficiency helps quantify how close a system is to perfectly reversible.


 [[fluid mechanics]]

#### conduction
low thermal conductivity
copper: high
![[Pasted image 20240405200536.png]]
![[Pasted image 20240405200622.png]]

#### convection
the transfer of energy by the physical movement of a fluid(liquid or gas)

ex: As air heats up its particles spread out lowering its density
![[Pasted image 20240405201049.png]]

no-slip condition

![[Pasted image 20240405201235.png]]
double pane window
#### radiation

### energy
![[Pasted image 20240405204500.png]]

![[Pasted image 20240405204533.png]]
It's similar to Ek and potential energy but on a much smaller, microscopic scale.
![[Pasted image 20240405204732.png]]

###### for the energy that can cross the boundary
![[Pasted image 20240405204840.png]]

##### first law
![[Pasted image 20240405204943.png]]

special cases
1. stationary
2. adiabatic process
	without transfer of heat or matter between a system and its surroundings![[Pasted image 20240405205059.png]]
3. isochoric
	![[Pasted image 20240405205225.png]]
	
###### open system
*Enthalpy includes internal energy, but also adds in the energy required to give a system its volume and pressure.*

WS <- W
Here you’ll want to focus on shaft work, which is basically any type of mechanical energy other than what’s necessary for flow.
![[Pasted image 20240405205544.png]]

![[Pasted image 20240405205700.png]]



### cycle
###### Y we can't build a perfect engine

![[Pasted image 20240405213652.png]]
![[Pasted image 20240405215957.png]]

![[Pasted image 20240405220204.png]]
![[Pasted image 20240405220350.png]]

[[Sadi Carnot]]
We still need to understand another property – one that wasn’t even put into words until a few decades after Carnot came up with his cycle.
[[Rudolf Clausius]]
###### heat engine fluid cycle
![[Pasted image 20240405230240.png]]

![[Pasted image 20240405230352.png]]
![[Pasted image 20240405230424.png]]
This plot lets us easily see what phase our fluid is in as it goes through each stage of the heat engine cycle.

![[Pasted image 20240405235239.png]]


###### fridge
![[Pasted image 20240405233935.png]]
freon:
	In your kitchen fridge, this working fluid is a hydrochlorofluorocarbon chemical that’s usually referred to generically as freon.

1. The evaporator removes heat from the inside of the fridge.
	It starts out with liquid fluid that’s colder than the inside of the fridge, which is the result of the last stage of the previous cycle.
	So, this liquid is really cold, but its boiling point is also really low. And when a liquid changes to a gas, it absorbs heat.
	So when the liquid in the evaporator boils, it absorbs heat from the refrigerator at the same time. All that heat energy is going into changing the liquid into a gas, not raising its temperature.
2. compressor
	Its job is to raise the pressure of the gas, which also raises its temperature — and its boiling point. After stage two is complete, the gas is really hot — hotter than the air outside the fridge.
	But because its boiling point increased too, it’s still around the temperature where it’s ready to condense into a liquid.
	
3.  condenser
	![[Pasted image 20240405234556.png]]
	In the condenser, the gas turns into a liquid, a process that releases heat. Since the refrigerant is now hotter than the air outside, heat can flow from inside the condenser to the surrounding air.
	But, like in the evaporator, the temperature of the refrigerant stays constant in the condenser.
4. expansion valve
	![[Pasted image 20240405235104.png]]
	It’s the opposite of what happens in the compressor.

not complete
![[Pasted image 20240405235401.png]]
Well, as the moisture from the sand evaporates, it cools the inner pot by “pulling” out heat.
Without recapturing the evaporated water, we’re going to need some outside work to make our sand wet again if we want to continue the cooling process.

###### reusable
we can use solar-powered photovoltaic panels to convert the sun’s rays into electricity by exciting the electrons within the panel’s cells.

