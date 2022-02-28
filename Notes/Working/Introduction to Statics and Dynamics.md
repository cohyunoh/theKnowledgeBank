# Introduction to Statics and Dynamics
---
## Mechanics and Historical Perspective
- **Mechanics** is concerned with *the motion and deformation of bodies that are subjected to forces*
	- Origins of mechanics may lie with **Archimedes**(287-212 BC)
	- ==Everything is subject to forces==
	- ==Lots of things are in motion==
	- ==Everything technically deforms==, but a lot of times **not signficantly**
		- *There are no actual rigid bodies*
- **Galileo** conducted first experiments in [[dynamics]]
- **Newton** formulated the [[Introduction to Statics and Dynamics#^9950c5|laws of motion]] and [[gravity]]
## Branches of Mechanics/Classifications
- Solid vs. Fluid(liquid or gas)
- [[Solids]] can be *rigid* or *deformable*
	- ==All real materials are deformable==; rigid means *the deformation is not significant*
- Rigid materials can be under [[static loading]] or [[dynamic loading]]
- **Kinematics** is a branch of [[dynamics]] that is only consiered with the geometric/time-dependent motion (no force analysis)
- **Kinetics** is more concerned with the forces that elicit accelerated motion
## Rigid vs. Deformable Bodies
- **Rigid body analysis** is only concerned with the *external forces that are applied into the body*
	- It is assumed that all (if any) internal forces summate to zero
- **Deformable body analyses** is concerned with *how the external forces effect the internal reorganization of bodies* ^9f15fa
- For BME 303/305
	- Elastic deformation: all deformations are recovered
	- Plastic deformation: all deformations are permanent
	- Fluids: continually defomr under a constant external load
## Overall Idealizations Used at Some Points
- **Particle**: A particle has mass but has no size asociated with  ^7f1707
	- (e.g. the size of the Earth is negligible as compared with the size of its orbit)
- **Rigid Body**: A combination of particles; all the particles remain at a fixed distance from each other, before and after loading
	- The deformation is negligible
	- ![[A2AAEE8B-B830-44FD-BAA1-6A1180B8FA49.jpeg]]
		- It can be ==both a rigid body and a particle==, depending on the need
		- Rigid body: *It requires knowing the ring's geometry and the angle the hooks are tugging at for this model*
		- Particle: *The geometry does not matter. The hooks and chain act a singular point for this model*
- **Concentrated Force**: The overalll effect of a loading condition that is assumed to at at one point
	- ![[CCD68F89-06FC-4D8A-A805-B27327294619.jpeg]]
		- Assume only one point of contact, but in reality it can be deformed
## Biomechanics and Historical Perspective
- **Biomechanics** is concerned with *the application of mechanics principles to biology/physiology*
- Leonardo da Vinci (1452-1519) studied some biomechanics problems (Horse gait)
- In general, **biomechanics analyses** can be conducted with *each branch of mechanics*
## Basic Concepts
- Basic concepts are **fundamental units of measurement that are not dependent on each other**
	- For Newtonian mechanics, these include:
		- Length, time, and mass (using SI units)
		- Or length, time, and force (using English units)
	- Note that once the basic concepts are defined, all other variables can be defined from the basic ones
- There are many other values that will be defined throughout your engineering career
	- Velocity, acceleration, force (or mass), energy, moment, momentum, ...
## Newton's Laws

^9950c5

- 1st: A body that is originally at rest will remain at rest, or a body in motion will move in a straight line with constant velocity, if the net force on the body is zero
- 2nd: A body with a net force acting on it will accelerate in the direction of that force and that the magnitude of the net force and inversely proportional to the mass of the body (if the mass does not change)
- 3rd: For every action there is always an equal an opposite reaction. These forces have the same line of action, the same magnitude but opposing directions
- ![[CFFE66D0-1A7F-4F00-857B-04A3B19B4F1C.jpeg]]
## Newton's Law of Gravitational Attraction
- This governs the gravitational attraction between two [[Introduction to Statics and Dynamics#^7f1707|particles]]
	- $F = G \frac{m_1 * m_2}{r^2}$
- **The universal constant of gravitation**; $G=66.73*10^-12 \frac{m^3}{kgs^2}$ 
- If one mass is the mass of the Earth ($5.972*10^24 kg$) and r is the radius of the Earth($6378.1 km$) you get:
	- $F=weight=mg$
- $g$ is determined at sea level at 45 degrees latitude
	- Stony Brook is ~41, which is ~27m above sea level
- The *g* for Stony Brook is lower than the standard!
## Dimensional Analysis and Units
- Very important to make sure you have proper quantities; meant to determine what the units should be
	- e.g. $[AREA]=[LENGTH][LENGTH]=[LENGTH]^2$
- Units are arbitrary measurements of these dimensions
## Numerical Calculations
- All equations must be dimensionally homogenous 
	- $s=vt+\frac{1}{2}at^2$
	- Each quantity is in dimensions of length
- ==SIG FIGS==
	- Write a decimal point or two after calculating entirely in calculator
## Cartesian Coordinate System
- The normal Cartesian system is a **right-handed system**
- Any vector can be broken into its Cartesian components if the appropriate angles are known
	- $\vec A\ = \overrightarrow{A_x} + \overrightarrow{A_y} + \overrightarrow{A_z}$
- Unit vectors are termed *i, j, and k* for x, y, z respectively
## Vector Representation
- $\vec A\ = A_x \hat{i} + A_y \hat{j} + A_z \hat{k}$
- $A = \sqrt{A_x^2 + A_y^2 + A_z^2}$
- $cos(\alpha) = \frac{A_x}{A}$
- $cos(\beta) = \frac{A_y}{A}$
- $cos(\gamma) = \frac{A_z}{A}$
	- $cos(\alpha)^2 + cos(\beta)^2 + cos(\gamma)^2 = 1$