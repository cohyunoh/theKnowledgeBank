# Introduction to Force, Moment, and Torque Vectors

## Scalars vs. Vectors
- All physical quantities in engineering mechanics are **measured using either [[Scalar|scalar]] or [[Vector|vectors]]** (note that there are tensors, but we do not discuss them in this class)
-[[Scalar]]: a *positive or negative* physical quantity that can be ==completely specified by its magnitude only==
	- **Length, mass, time, speed**
- [[Vector]]: a *physical quantity* that requires both ==magnitude and direction==
	- **Force, position, moment, velocity**
- Why do we have speed limits and not velocity limits?
	- Velocity requires a direction as well as a magnitude
	- Not all roads go from east to west

## More on Vectors
- Shown graphically by an arrow
	- Length represents the magnitude
	- Angle between an *arbitrary reference* represents line of action
	- Head of arrow represents the direction
	- [[Vector]]s are typically presented as **bold capital letters** or **non-bold capital letters** with an ==arrow over the letter== or **underscored non-bold capital letters**
	- $\textbf{A} = \overrightarrow{A} = \underline{A}$
![[59BA16AD-ED37-45B7-8567-20679EFC6EAD.jpeg]]

## Vector Addition
- Only components in the same direction add
- Can use **graphical methods** (parallelogram law or triangle rule)
- No such thing as **vector subtraction**; must add a negative value
	- $\overrightarrow{A} - \overrightarrow{B}$ (bad)                  
	- $\overrightarrow{A} + (-\overrightarrow{B})$ (good)
![[B9B4546B-37AE-4480-B592-48A20C8A5C77.jpeg]]

## Scalar Multiplication
- **Scalar Multiplication** of a vector increases (or decreases) the magnitude of the vector
- This operation has ==no net effect on the line of action== of the vector but can *reverse the direction*
![[0F2D0D95-B13F-478B-845F-A6E0936BC14F.jpeg]]

## Force as a Vector
- [[Force]] is fundamentally a *load applied to some material*
- [[Force]]s are **all around us**, in everything we do
	- Sitting on a chair, air movement around us, moving muscles, …
- Forces can cause motion (but do have to)
- Forces can also cause [[Introduction to Statics and Dynamics#^9f15fa|deformation]] (although will not consider this)
- **Multiple forces can act at the same time**, we will typically couple forces by directions of action (we may break a force into components)
- Forces however ==must have a magnitude and a direction associated with their actions==

## Resultant Forces
- The *addition of forces* acting on a particular object into **one net force**
- The ==magnitude of the resultant force== can be calculated from the **Pythagorean theorem** if the known components are perpendicular to each other
- ==The direction of the resultant force== can be calculated from *the inverse tangent of the known components*, if they are perpendicular to each other
- $F_R = \sqrt{(F_Q)^2 +(F_P)^2}$
- $\theta = tan^{-1}(\frac{F_P}{F_Q})$
![[9B41D0A0-5601-4819-8313-830D4E701CCC.jpeg]]

## Other Examples of Resultant Forces
![[F9BEEBB5-4185-413A-8956-12F78146A133.jpeg]]
- Notice the two different assumptions made about the connecting pieces from the upper and bottom left graphics
## Types of Forces
- **[[Normal force]]**
- **[[Tangential force]]**
- **[[Tensile forces]]**
- **[[Compressive forces]]**
- **[[Coplanar forces]]**
- **[[Collinear forces]]**
- **[[Concurrent forces]]**
- **[[Parallel force]]**
![[13356D13-0B78-43E1-84A0-A6461BC9992E.jpeg]]

## Gravitational Force or Weight
- This is the force ==exerted by Earth on an object==
- We will always consider *g* be a constant
	- If you go into space biomechanics, this may not be a good assumption
- $g = 9.81 \frac{m}{s^2} = 32.2 \frac{ft}{s^2}$
- An object in free fall (near Earth) will accelerate at *g*
	- Weight is the force that is associated with this acceleration

## Distributed Loads
- In general for all mechanic problems, ==loads will be distributed and *not* act at a point==
	- Remember: **Density is constant**, which is also assumed
- However, we generally make use of the assumption that **these distributed loads can be represented by an equivalent point load**
- Be careful when considering *pressure (force/area)*
	- Why does your snow booted foot sink in snow, but it does not sink on a ski?
		- More area on ski, therefore less pressure

![[F4CDA7F5-0BCC-40DA-8E74-0604900A9176.jpeg]]
- *C.G. stands for center of gravity*

## Friction
- ==Frictional forces== occur between **any two surfaces in contact when one surface slides (or is trying to slide) over the other**
- ==Friction== is defined *by the surfaces (and their properties) that are in contact*
- The **static friction** is the force that *must be overcome prior to initiating motion*
	- Characterized by the static coefficient of friction, $\mu_s$
- The **kinetic friction** is the force *associated with the motion*
	- Characterized by the kinetic coefficient of friction, $\mu_k$
- $\mu_s > \mu_k$
	- Harder to get something to move than to keep it moving
- ==Friction forces== are a function of the normal force between the surfaces
	- $\overrightarrow{{F_f}_{max}} = \mu_s \overrightarrow{N}$
	- $\overrightarrow{{F_f}_{k}} = \mu_k \overrightarrow{N}$

## Friction Coefficients and Diagram
![[BC5F3E33-187D-41BE-AEE9-C699E051281C.jpeg]]
- Big ranges due to defects, not all materials of the same category are the same, or lots of different variations of combinations
## Moments vs. Torques
- [[Torque]] is associated with the ==rotational and twisting actions of applied forces==
	- *Opening a door, rotating a valve*
- **Moments** are associated with the ==bending effect of applied forces==
	- *Standing on the end of a diving board*
- Mathematically they are represented in the same way and we will use their definitions interchangeably and nothing bends in this class
- The **magnitude of moment** is equal to the *magnitude of the force, multiplied by the shortest length between the line of action of the force and the point of rotation (termed the moment arm)*
- The **direction of the moment** is determined by the *direction of the force about the point of rotation*

## Moment Figures
![[A3CE931E-E6E0-4FCB-B228-A56989CD16DC.jpeg]]
## Magnitude of Moment 
- **If the distance is perpendicular**: $M_0 = Fd$
	- Direction by the right hand rule
- **If the distance is not perpendicular**: $M_0 = d \times F$
	- Direction by the hand rule
	- Also useful for 3D problems, not as useful for 2D problems
![[604EDC43-9A6A-4FBF-AB5F-ACC3A35F51F8.jpeg]]
![[8AAD2FEF-1DDE-4DDD-ABE3-8AEE00459ED9.jpeg]]