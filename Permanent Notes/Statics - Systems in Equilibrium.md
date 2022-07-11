# Statics - Systems in Equilibrium
___
## Review of Salient Definitions (work on markdown files linked)
- [[Statics]]: An area of mechanics that is concerned with the analysis of rigid bodies of in equilibrium
- [[Rigid bodies]]: undergoes no deformations under externally applied loads
- [[Equilibrium]]: a body at rest or under constant velocity motion (e.g. acceleration is zero)
- [[Newton’s Second Law]] (Equation of Motion): $\overrightarrow{F} = \frac{d}{dt}(m\overrightarrow{v})$ if $\frac{dm}{dt} = 0$, then $\overrightarrow{F}=m\overrightarrow{a}$.
	- **Mass** is a *measure of inertia*, which is the ==tendency of a body to resist changes in its motion==
	- The more inertia that a body has, the less likely that body is to resist changes in its motion
## Linear vs. Angular Motion (incomplete markdown)
- The equation of motion is **only valid for translational motion**
	- This is *motion*, where all ==molecules of a body follow the same path== (can be [[rectilinear]] or [[curvilinear]], but *all molecules experience the same distance traveled*)
	- Constrained piston, linkages (or things that can be modeled like this)
- An analogous equation of motion can be written for rotational motion
	- $\overrightarrow{M}=I\overrightarrow{\alpha}$ (if the mass moment of inertia is constant as a function of time)
		- Notice how *I* is **not constant like mass** because ==it changes with where the axis is==
	- *All particles do not experience the same distance traveled*
	- Fly wheels, gears, discs, constrained linkages (or things that can be modeled like this)
- In general, motions are a ==combination of translational motion and rotational motion==
	- Many examples, would use both equations of motion
![[4F6D05FD-313D-422F-9AC5-11D60D179AB4.jpeg]]
## Conditions for Equilibrium
- A body is in [[Equilibrium|equilibrium]], if and only if, **the sum of the forces and the sum of the moments (in each applicable direction) sum to zero**
- In this case, the **velocity (angular or linear)** does *not experience an acceleration and are thus constant* (this includes zero velocity)
- Translational Equilibrium: $\Sigma \overrightarrow{F} = 0$
- Rotational Equilibrium: $\Sigma \overrightarrow{M} = 0$
## Coplanar Force System - In Equilibrium (finish latex and graphic)
$\Sigma \overrightarrow{F} = (F_{1x}$
## Free Body Diagrams
- This is one of the most important concepts in mechanics
- All **known** and **unknown forces and moments** are shown on a diagram that is not constrained by anything
	- ==Known forces==: *magnitude and direction are known*
	- ==Unknown forces==: *magnitude or direction are not known*
- **Location of loads** should be *placed accurately* (e.g. scale) *on the figure*
- This figure will be used to determine what equations are needed and how to solve the problem
## Support Reaction Forces
- If a support **prevents the translation of a body in a given direction**, then a *force is developed on the body in that direction*
- If **rotation is prevented** a *moment is exerted on the body at that point*
- Common supports (2D problems):
	- ==Roller==: prevents motion in one direction
	- ==Pin==: prevents motion in two directions
	- ==Fixed support==: prevents motion and rotation
![[19BC3C1B-F01B-497B-B600-815E552A30CD.jpeg]]
___
![[61D7511B-AF73-487E-8407-C471968C47A1.jpeg]]
___
![[96BF53F0-22EE-40DF-9B70-FF6605B908EC.jpeg]]
## Biological Examples of Support Reactions
![[16E71258-52A2-43EA-8BFB-D97B09DD73F8.png]]
## Weight and Center of Gravity
- If a body is subjected to any gravitational attraction, then the body has a specific weight
- This weight is a summation of all of the gravitational forces for each particle within the body
- We assume that this summation acts at one particular location (instead of a distributed system over the entire body) at the center of gravity
	- For a uniform body (uniform density and geometry) this location is at the centroid of the body
	- For a non‐uniform body, we may have to calculate where the centroid is located
![[2129017D-6DBB-4ED4-9D44-4899ECDD7400.jpeg]]
## Springs, Cables and Pulleys
- [[Springs]] or materials that can be idealized to springs are always assumed to be **linearly elastic**
	- The *length of spring* changes in **direct proportion with the force acting on the spring**
	- The spring constant (or stiffness) equates this proportion
- [[Cables]] or materials that can be idealized to cables are always assumed to have **negligible mass and they cannot elongate** (e.g. rigid)
	- A continuous cable has the same tension within the cable
- [[Pulleys]] are always assumed to be **massless and idea**l
	- Massless pulleys have no resistance to changes in rotational motion 
	- Ideal means that they have no friction during their rotation
![[8EDAD66C-F859-49CF-AA81-FC37AAE7D585.png]]
## A Bit on Cross Products (incomplete)
## Usefulness of Cross Product Definition(incomplete)
- It does not matter how you defined the distance vector in these cases