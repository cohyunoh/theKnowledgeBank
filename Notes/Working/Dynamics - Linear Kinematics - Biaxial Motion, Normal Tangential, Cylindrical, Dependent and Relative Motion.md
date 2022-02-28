# Dynamics - Linear Kinematics - Biaxial Motion, Normal Tangential, Cylindrical, Dependent and Relative Motion
___
## Biaxial Motion -Projectile Motion
- This analysis is used often, because it is *a simplified curvilinear motion*, where the **motion occurs within one plane**
- Also, ==the only force acting on the particle is the force of gravity== (due to the mass of the particle), *no drag, no wind, no lift … vacuum.*
	- Thus, the **only acceleration that is involved is the acceleration due to gravity**
	- Note, that you can be given a different gravitational acceleration (e.g. you are on a different planet)
![[4A4529F0-946B-448B-96CF-A7E8F7E40810.jpeg]]
![[Recording 20220223092457.m4a]]
## Equations for Projectile Motion
- Horizontal direction ($a_x = 0$)
	- $v_x = (v_0)_x$
	- $x = x_0 + (v_0)_x t$
- Vertical direction ($a_y = -g$)
	- $v_y = (v_0)_y - gt$
	- $y = y_0 + (v_0)_y t - \frac{1}{2}gt^2$
	- $v_y^2 = (v_0)_y^2 - 2g(y-y_0)$
- *Only four useful equations because only 2 of the 3 vertical direction equations are interdependent*
![[Recording 20220223092732.m4a]]
## There are many types of Problems Associated with Projectile Motion
- Given initial velocity, find where it lands, how long it takes to land, velocity at landing, maximum height, angle needed to hit a particular location …
- Limited by height of a building, where does it land, what time does it land …
- Have to make it over a building, where does it land, what time does it land

___
### Forget Physics Tricks
- velocities @ max height
	- $v_y = 0$
	- $v_x = (v_x)_0$
- relationship between t’s
	- $\Delta t_1 + \Delta t_2 = \Delta t$
		- True
	- $\Delta t_1 = \Delta t_2 = \frac{1}{2} \Delta t$
		- Only if symmetrical
- final velocity if symmetrical
	- $(v_f)_y = -(v_0)y$
	- $(v_f)_x = (v_0)_x$

___
![[Recording 20220223093751.m4a]]
## Curvilinear Motion: Normal and Tangential Components
- If the path that the particle traverses ==is known==, then it is sometimes **easier to describe the path with normal (perpendicular to the curve) components**
- In this situation, *the origin of the axes always resides with the particle* - this would be termed a ==translating coordinate system==
	- Also, it is important to note, that *the normal and tangential directions can (and normally do) change with time*
## Planar Motion - Position (Latex)
- The t axis (tangent axis) is tangent to the curve and its positive with increasing s direction
	- s is measured from the initial point of the curve
	- The unit normal vector for this direction is $\overrightarrow{u}_t$ 
- The n axis (normal axis) is always perpendicular to the t axis and is directed toward the center of curvature of the arc
	- This is always the concave side
	- The unit normal vector for this direction is $\overrightarrow{u}_n$
	- A straight line has no curvature
![[F023EE48-F594-474B-B59D-3BB2BD2679C4.jpeg]]
## Planar Motion - Velocity
- Since the particle moves, its displacement can be defined as a function of time
- Therefore, the velocity of the particle can be obtained as the derivative of this displacement function
	- The direction of v, at a given time, always aligns with the t axis (remember the t axis can change though)
- $\overrightarrow{v} = \frac{ds}{dt} \overrightarrow{u}_t$
![[D1C46FDD-1F9F-436C-A9F5-533C99628227.jpeg]]
## Planar Motion - Acceleration (Latex)
- The acceleration of the particle is the time rate of change of velocity • Mathematically this is represented as
𝑎⃗ 􏰀 𝑑 𝑣⃗ 􏰀 𝑎 𝑢􏰁 􏰂 􏰃 𝑣 𝑑 𝑢􏰁 􏰂 𝑑𝑡 𝑑𝑡
• This makes use of the product rule
• How do we find the time derivative of a direction vector?
![[Recording 20220223094740.m4a]]
## Time Derivative of Direction Vector (incomplete)
- Assume that $dt$ is small
- We know that $\overrightarrow{u}_t$ cannot change in length; it can change in direction and this direction change is what we need to know
- Using vectors we have the following: 
![[Recording 20220223095133.m4a]]
## Continuation of Time Derivative (incomplete)
- Therefor, the time derivative of the direction vector becomes $\frac{d\overrightarrow{u}_t}{dt} = \frac{d\theta}{dt}$, in the normal direction. Since the magnitude does not change in time, this is not included in the formulation and only the directional change is considered
- For small changes in time, $d\theta = \frac{ds}{\rho}$, therefore, $\frac{d\theta}{dt} = \frac{ds}{dt\rho}$ 
![[Recording 20220223095528.m4a]]
## Planar Motion - Acceleration Forms (incomplete)
- The final form of acceleration is
- where
![[Recording 20220223095849.m4a]]
## Acceleration Conclusions (incomplete)
- If the path is straight, then $\rho \rightarrow \inf$ 
![[Recording 20220223100000.m4a]]
## Other useful Formula for Norma/Tangential (incomplete)
- If the tangential acceleration is constant
- If the path function is expressed as y=f(x), then the radius of curvature can be defined as
![[Recording 20220223100205.m4a]]
## Summary of Normal-Tangential Problems (incomplete)
- Be careful of the word
![[Recording 20220223100226.m4a]]
## Curvilinear Motion: Cylindrical Components (incomplete)
- Sometimes, it is easiest to describe the path function using cylindrical coordinates
• If this is the case, then we must move to polar notation
• Polar notation is described by a radial coordinate (r) and a transverse coordinate ($\theta$), given from a fixed point
• Make use of radians where $\pi$ radians = 180 degrees
![[Recording 20220223100346.m4a]]
## Cylindrical Coordinates: Position and Velocity (incomplete)
- Position is defined by the radial coordinates: $\overrightarrow{r}=r\overrightarrow{u}_r$
- 
![[Recording 20220223100519.m4a]]
## Cylindrical Coordinates: Acceleration (incomplete)
- The acceleration is defined as
![[Recording 20220223100559.m4a]]
## Summary of Cylindrical Coordinates

![[Recording 20220223100723.m4a]]
## Absolute Dependent Motion (incomplete)
- In some cases, the motion of one particle is dependent on the motion of another
	- Typically the particles are coupled by a linkage (shown as a rope and pulley system)
	- In the figure, as A moves down, B would move up
- Using the rope length method, we describe displacements in terms of the rope segments
	- $l_\tau = $ 

___
### Derivation of the Rope Length Equation (incomplete)

___
### Can This be More Complicated? (incomplete)

___

![[Recording 20220223101142.m4a]]
## Relative Motion of Two Particles
- In some instances, it is easy to relate the motion of two moving bodies using a translating axes

___
### Position

___
### Velocity/Acceleration

___

![[Recording 20220223101348.m4a]]
