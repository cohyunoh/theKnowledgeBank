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
- YOU MUST INCLUDE $\overrightarrow{a}$ AND $\overrightarrow{\alpha}$ IN YOUR CALCULATIONS UNLESS YOU KNOW IT IS ZERO
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
## Velocity
- For a particle that moves through a displacement of $\Delta s$ during the time interval $\Delta t$, the average velocity is defined as $v_{avg} = \frac {\Delta s}{\Delta t}$
	- Note that this does not assume that the velocity is constant
- The **instantaneous velocity** is derived from taking the limit of the average velocity as $\Delta t \rightarrow 0$
	- $\lim_{\Delta t \to 0} (\frac{\Delta s}{\Delta t}) = \frac{ds}{dt}$
- Velocity is a vector that has the same sign as the displacement, because time always moves in the positive direction
![[15AF2F25-045D-4316-A4CC-998D2814D3B9.jpeg]]
## Speed
- The magnitude of velocity is known as the speed
	- This is a scalar and does not give directions
- The **average speed** is defined as the *total **distance** the particle traveled divided by the elapsed time*
	- $(v_{sp})_{avg} = \frac {s_T}{\Delta t}$
![[B1F04E07-2914-4D51-A631-EE7DD4E2C3AF.jpeg]]
## Acceleration
 - Knowing the **velocity of a particle at two instances in time, the average acceleration** of the particle is defined as $a_{avg} = \frac{\Delta v}{\Delta t}$
	 - Note that this does not assume that the acceleration is constant over the time period
 -  The ==instantaneous acceleration== is derived from taking the limit of the average acceleration as $\Delta t \rightarrow 0$
	 - $a = \lim_{\Delta t \to 0} (\frac{\Delta v}{\Delta t}) = \frac{dv}{dt} = \frac{d^2 s}{dt^2}$
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
	- $\textbf{v} = \lim_{\Delta t \to 0} (\frac{\Delta \textbf{r}}{\Delta t}) = \frac{d \textbf{r}}{dt}$
- The direction of v is always tangent to the curve
- The magnitude (“speed”) of v is defined by the differentiation of the path function ($v = \frac{ds}{dt}$)
![[729B2974-07F6-4428-91AB-518C3F96C30F.jpeg]]
## General Curvilinear - Acceleration
- If the particular has a velocity of $v$ at some time ($t$) and a velocity of $v’ = v + \Delta v$ at some later $(t + \Delta t)$, then the average acceleration is
	- $a_{avg} = \frac{\Delta v}{\Delta t}$
- The instantaneous acceleration is determined as $\Delta t$ approaches zero
	- $a = \lim_{\Delta t \to 0} \frac{\Delta v}{\Delta t} = \frac{dv}{dt} = \frac{d^2 r}{dt^2}$
- The derivative of $a$ acts tangent to the plot of the velocity. In general this, is not tangent to the path function and tends to be directed towards the center of the path function.
![[0EE9D274-C796-4C9D-AEB0-BCCE5C5DBBC9.jpeg]]
## Rectangular Component System - Position
- If a particular path can be described in x, y, and z coordinates then
- Position: $\textbf{r} = x\overrightarrow{i} + y\overrightarrow{j} + z\overrightarrow{k}$
- The magnitude of position would be given by: $r = \sqrt{x^2 + y^2 +z^2}$ 
- Direction would be given by three angles
![[A726016E-11A0-45EA-A9FD-729E93C82321.jpeg]]
## Rectangular Component System -  Velocity
- The velocity is obtained from the first derivative of position
	- $\textbf{v} = \frac{d\textbf{r}}{dt} = \frac{d}{dt}(x\overrightarrow{i})+ \frac{d}{dt}(y\overrightarrow{j})+ \frac{d}{dt}(z\overrightarrow{k})$
- Note that these derivatives would need the chain rule: $\frac{d}{dt}(x\overrightarrow{i}) = \overrightarrow{i}\frac{dx}{dt} + x\frac{d\overrightarrow{i}}{dt}$
- This takes into account both changes in direction and magnitude
	- $\textbf{v} = v_x\overrightarrow{i} + v_y\overrightarrow{j} + v_z\overrightarrow{k}$ 
	- $v = \sqrt{v_{x}^2 + v_{y}^2 + v_{z}^2} \to$ magnitude
![[25BCACB0-64FA-4F9C-B874-164AE42ADE2F.jpeg]]
## Rectangular Component System -  Acceleration
- The acceleration is obtained from the first derivative of velocity 
	- $\textbf{a} = \frac{d\textbf{v}}{dt} = a_x\overrightarrow{i} + a_y\overrightarrow{j} + a_z\overrightarrow{k}$
- These formular are related as:
	- $a_x = \frac{d}{dt}v_x = \frac{d^2}{dt^2}x$
	- $a_y = \frac{d}{dt}v_y = \frac{d^2}{dt^2}y$
	- $a_z = \frac{d}{dt}v_z = \frac{d^2}{dt^2}z$
	- $\textbf{a} = \sqrt{a_{x}^2 + a_{y}^2 + a_{z}^2} \to$ magnitude
![[9982A865-3FF9-4D69-AB31-79928C6ECBE7.jpeg]]