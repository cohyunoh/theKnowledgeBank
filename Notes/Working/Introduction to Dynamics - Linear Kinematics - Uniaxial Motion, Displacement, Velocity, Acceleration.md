# Introduction to Dynamics - Linear Kinematics - Uniaxial Motion, Displacement, Velocity, Acceleration
___
## Side Note
- Equations of Motion:
	- $\Sigma \overrightarrow{F} = m \overrightarrow{a}$
	- $\Sigma \overrightarriw{M} = I \overrightarrow{\alpha}$
	- Secret of Statics:
		- It solves the left hand side of these equations
		- Deal with forces/moments
		- FBD
	- Secret of Kinematics:
		- $\overrightarrow{a}$
		- $\overrightarrow{\alpha}$
## Remember
- ==Dynamics== is the ***branch of mechanics** that is concerned with the accelerated motion of a body*
- Dynamics is divided into two main section
	- ==Kinematics:== concerned with only the geometric aspects of the motion
	- ==Kinetics:== concerned with the analysis of forces that induce the motion
- We will study both particle dynamics and rigid body dynamics
- YOU MUST INCLUDE $\overrightarrow{a}$ AND $\overrightarriw{\alpha}$ IN YOUR CALCULATIONS UNLESS YOU KNOW IT IS ZERO
## Rectilinear Kinematics: Continuous Motion
- **Motion of a particle on a straight line**
- By definition, a ==particle== has a *mass but negligible size and shape*
	- In reality, this analysis must be applied **sparingly**, where the size has little to no effect on the motion
- For ==objects with a size==, this analysis may be used, if we discuss the motion of the bodies mass center and *neglect any rotation of the body or if the body can be assumed to be rigid*
	- For example, if all of the particles in a body move the same distance, in the same time interval in the same direction
## Rectilinear Kinematics
- The kinematics of a particle is characterized by **specifying (at a given instant in time) the particles position, velocity and acceleration**
- ==Position coordinate==, is defined using a single coordinate axis, *s*
	- The origin on this path is *O*
	- The magnitude *s* is the distance of the particle from *O*
	- This is used to determine the location of any particle
![[B5E187F7-5D06-4929-B8E8-84675A0F69EE.jpeg]]
## Displacement
- This is defined as the change in the particles position
- As the particle moves from one point to another, we can mathematically represent displacement as $\delta s = s’ - s$
- Displacement can be negative or positive, therefore displacement is a **vector quantity**
 ![[A32865D2-C26F-445F-A4A1-D625D0AC2BB5.jpeg]]
## Velocity (EQUATION MISSING)
- For a particle that move through a displacement of $\Delta s$ during the time interval $\Delta t$, the average velocity is defined as $v_{avg} = \frac {\Delta s}{\Delta t}$
	- Note that this does not assume that the velocity is constant
- The **instantaneous velocity** is derived from taking the limit of the average velocity as $\Delta t \rightarrow 0$
- Velocity is a vector that has the same sign as the displacement, because time always moves in the positive direction
![[15AF2F25-045D-4316-A4CC-998D2814D3B9.jpeg]]
## Speed
- The magnitude of velocity is known as the speed
	- This is a scalar and does not give directions
- The **average speed** is defined as the *total **distance** the particle traveled divided by the elapsed time*
	- $(v_{sp})_{avg} = \frac {s_T}{\Delta t}$
![[B1F04E07-2914-4D51-A631-EE7DD4E2C3AF.jpeg]]
## Acceleration (EQUATION MISSING)
 - Knowing the **velocity of a particle at two instances in time, the average acceleration** of the particle is defined as $a_{avg} = \frac{\Delta v}{\Delta t}$
	 - Note that this does not assume that the acceleration is constant over the time period
 -  The ==instantaneous acceleration== is derived from taking the limit of the average acceleration as $\Delta t \rightarrow 0$
 ![[DF8549C4-6702-4EC1-AFAB-725574FF97C2.jpeg]]
## Acceleration Discussion
- *If the velocity at the second point is the same as the first point*, then the **particle is not accelerating** (or the average acceleration is zero)
- *If the velocity at the second point is less than the velocity at the first point*, then the **particle is decelerating**
- *If the velocity at the second point is more than the velocity at the first point*, then the **particle is accelerating**
	- Note that for the last two bullets, the velocity may be negative and either get more negative (deceleration) or more positive (accelerating)
- **Acceleration is also a vector**, whose *direction is determined by the relationship between the velocities*
## Units of the Quantities Discussed
 - **Position, Displacement or Distance** have units of length (i.e. feet, meter, inch ...)
 - **Velocity or Speed** have units of length divided by time (i.e. meters/second, miles/hour ...)
 - **Acceleration** has units of length divided by time squared (i.e. meters/second2, feet/second2 ...)
## An Important Relationship
- There is an important relationship that relates displacement, velocity and acceleration, without a consideration on time
- We know:
	- $a = \frac{dv}{dt}$
	- $v = \frac{ds}{dt} \rightarrow dt = \frac{ds}{v}$
	- $a = \frac{dv}{ds/v}$
	- $ads = vdv$
## General Kinematic Relationships
- In general, the equations from the section above can be used to solve many kinematic problems ==(USE THESE EQUATIONS)==
	- ![[ED6AEAB6-DF4E-4CCA-BA34-67D6503980CE.jpeg]]
- However, in the case when the acceleration is constant
	- ![[FCEED62B-B65F-4E3C-8AA3-BCD5C624D454.jpeg]]
## Procedures for Analysis - Uniaxial Motion
1. Establish a coordinate system
2. Draw known values on the coordinate system
3. If a relationship is known between 2 of the 4 variables ($a, v, s or t$) we can use the the three kinematic relationships to gain information about the other variables
4. Make sure the integration bounds are correct; many times they will be zero, like depicted on the previous slide, but now always
## General Curvilinear Motion - Position
- Curvilinear motion occurs when a particle moves along a curved path (sometimes termed biaxial or triaxial motion)
- In the most general form, paths are in three‐dimensional space, therefore vectors are needed
- The path function (this is what the particle follows) will be defined as $s(t)$
- The position of that particle will be $r = r(t)$
- The magnitude and direction of r will change with time
![[6F1A5E18-B03F-483B-A008-F02BA6FE9B1E.jpeg]]
## General Curvilinear Motion - Displacement
- During a small time interval a particle moves from $r$ to $r’$
- The displacement of the particle is defined by the vector subtraction
	- $\Delta r = r’ - r$
- Note that $\Delta r$ is not necessarily the same as $\Delta s$ because of the curvature ($\Delta r$ is “as the bird flies”)
 ![[7B92EDA5-6408-4C88-9C33-24798D6C6FFA.jpeg]]
## General Curvilinear Motion - Velocity (Missing Equation)
- The average velocity over a particular time interval ($\Delta t$) will be defined as 
	- $v_{avg}= \frac {\Delta r}{\Delta t}$
- The instantaneous velocity is determined as $\Delta t$ approaches zero 
- The direction of v is always tangent to the curve
- The magnitude (“speed”) of v is defined by the differentiation of the path function ($v = \frac{ds}{dt}$)
![[729B2974-07F6-4428-91AB-518C3F96C30F.jpeg]]
## General Curvilinear - Acceleration
