# Statics - Friction, Center of Gravity, and Simply Supported Structures
___
## Cable-Pulley Systems and Traction Devices
- **The Rules of Pulleys**
	- $R_y = T_{B_y} + T_A$
	- $R_x = T_{B_x}$
	- $W = T_A$
	- $r T_A = r T_B$
- Under ==dynamic conditions==, these relationships may be *altered* if **accelerations need to be considered** or if **the mass of the pulley need to be considered**
![[6B4415D5-3D05-45B0-8CC3-398F6C76478D.jpeg]]

## You must be Careful with the Linkages within the Pulley System and how many Ropes there are
![[0CE2D0F0-A9A4-4CA0-940D-B50ACA01977C.jpeg]]
- In *case 1*:
	- We assume $T_1 = W$
	- Also assume if we pull on the free end down *1 foot*, the weight will move *1 foot* upwards
- In *case 2*:
	- $T_2 = \frac{W}{2}$
	- If we move free end down *1 foot*, it will move upwards *1/2 feet*
- In *case 3*:
	- $T_3=\frac{W}{3}$
	- If we move free end down *1 foot*, it will move upwards *1/3 feet*
- You gain in force by adding pulleys but you lose in **displacement**
## Dry Friction
- ==Friction== is a force that **resists the movement of two contacting surfaces**
- ==Friction== always **acts tangent to the surfaces at the point of contact**
	- Is there ever a single point of contact?
		- Due to deformations, no
	- *The direction of friction opposes the possible or existing direction of motion*
- ==Friction== arises due to the *irregularities* of the surfaces in contact
	- The force that prevents the motion is divided into a normal force (which balances the weight) and a frictional force that balances the pulling force
___
![[57E2DA9E-52BD-43F0-A325-7B7A9DE9D9C4.jpeg]]
- Why is it not uniform the normal force?
	- Rigid bodies rotate
	- The box is tipping towards the pulling force
	- The force is not acting equally on the rigid body
___
## At Impending Motion or During Motion
- The frictional force is directly proportional to the normal force
	- $F_S = \mu_S N$
- During motion the frictional force is also directly proportional to the normal force
	- $F_k = \mu_k N$
- In statics, we can have either of these, but in general the **frictional coefficient is provided in the prompt** (e.g. you do not need to determine which type of friction you have)
- Some *definitions*:
	- When **slipping is ==about== to occur**, we use *static friction*
	- When **slipping is occurring**, we use *kinetic friction*
	- Must be careful if it is a ==rigid body==; can tipping occur, where is the normal force
## Center of Gravity (incomplete)
- The resultant of the ==gravitational force== on every particle in a rigid body is the **weight** and this acts at the *center of gravity of the body*
- If the ==rigid body== has a *uniform and regular geometry* then the center of gravity is the same as the geometric center of the body
![[00348051-9A90-4582-B6EC-059DA4E98E0B.jpeg]]
- Every point of mass in the greater mass of question has these ~ coordinates while the bar coordinates represents the coordinates of the **center of gravity**
## Location of the Center of Gravity
![[61295C04-1A93-4276-BB18-917553DF60C1.jpeg]]
- Can be extended to the mass center or centroid, which we will assume is the same (they have slightly different formulations)
- Be careful that these locations **do not need to lie within the body**, since it would be an *effective location*
![[DF503876-EC4F-4008-A1C0-72534A8F06F6.jpeg]]
## General Method to Solve Center of Gravity Examples
- You must **make a relationship for area and x as a function of y** (and z if you have 3 dimensions)
- Solve the integrals and plug in the numbers as appropriate for the integral bounds
## Composite Body Method
- A ==composite body== consists of a *series of connected common shapes* whose centroid can be easily identified
- These bodies are typically divided into their components and each component is analyzed separately
- The centroid of the composite body is then the weighted average of each of the components
![[715560AF-E412-407D-9AB5-139B4DA1D012.jpeg]]
## Classical Statics Courses
- These concepts are extended to simple structures, such as **trusses**’
- In the design of a truss, one would be interested in the *overall loading on the members*, whether or not they are in compression or tension and what kind of constraints are needed at each end
- We assume that **loading** occurs at ==joints only== and **members** are joined by ==smooth pins==
- We will analyze a simple truss in this course as an example
- This can be extended to the skeleton
___
![[EEAA95AB-A7A9-4C0F-9052-F7517B4018F7.jpeg]]
___