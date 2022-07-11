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
## Planar Motion - Position
- The ==t axis== (**tangent axis**) is tangent to the curve and its positive with increasing s direction
	- s is measured from the initial point of the curve
	- *The unit normal vector for this direction is $\overrightarrow{u}_t$* 
- The ==n axis== (**normal axis**) is always perpendicular to the t axis and is directed toward the center of curvature of the arc
	- This is always the ==concave side==
	- The *unit normal vector for this direction is $\overrightarrow{u}_n$*
	- A straight line has no curvature
![[F023EE48-F594-474B-B59D-3BB2BD2679C4.jpeg]]
## Planar Motion - Velocity
- Since the particle moves, **its displacement can be defined as a function of time**
- Therefore, *the velocity of the particle can be obtained as the derivative of this displacement function*
	- The direction of v, at a given time, always aligns with the t axis (remember the t axis can change though)
- $\overrightarrow{v} = \frac{ds}{dt} \overrightarrow{u}_t$
![[D1C46FDD-1F9F-436C-A9F5-533C99628227.jpeg]]
## Planar Motion - Acceleration
- The acceleration of the particle is the time rate of change of velocity
- Mathematically this is represented as
	- $\overrightarrow{a} = \frac{d\overrightarrow{v}}{dt} = a\overrightarrow{u_t} + v\frac{d\overrightarrow{u_t}}{dt}$ 
	- This makes use of the product rule
- How do we find the time derivative of a direction vector?
![[Recording 20220223094740.m4a]]
## Time Derivative of Direction Vector
- Assume that **$dt$ is small**
- ==We know that $\overrightarrow{u}_t$ cannot change in length==; i**t can change in direction and this direction change is what we need to know**
- Using vectors we have the following: $\overrightarrow{u_t}’ = \overrightarrow{u_t} + d\overrightarrow{u_t}$, where $\overrightarrow{u_t}’$ is the tangent unit vector after the small time $dt$ 
![[90745EB1-EB90-47EB-880F-1531AFED11AD.jpeg]]
![[Recording 20220223095133.m4a]]
## Continuation of Time Derivative
- Therefore, **the time derivative of the direction vector becomes** $\frac{d\overrightarrow{u}_t}{dt} = \frac{d\theta}{dt}$, **in the normal direction**. Since the *magnitude does not change in time*, this is not included in the formulation and only the directional change is considered
- For small changes in time, $d\theta = \frac{ds}{\rho}$, therefore, $\frac{d\theta}{dt} = \frac{ds}{dt\rho} = \frac{v}{\rho} = \frac{d\overrightarrow{u_t}}{dt}$ 
![[E3274819-0D9C-490A-ABF7-45858BF86B99.jpeg]]
![[Recording 20220223095528.m4a]]
## Planar Motion - Acceleration Forms
- The final form of acceleration is
	- $\overrightarrow{a} = \frac{d\overrightarrow{v}}{dt} = a\overrightarrow{u_t} + v\frac{d\overrightarrow{u_t}}{dt} = {a_t}{\overrightarrow{u_t}} + {a_n}{\overrightarrow{u_n}}$
- where
	- $a_t = \frac{dv}{dt} = v\frac{dv}{ds}$
	- $a_n = \frac{v^2}{\rho}$
	- $a = \sqrt{a_t^2 + a_n^2}$
![[Recording 20220223095849.m4a]]
## Acceleration Conclusions
- If the path is straight, then $\rho \to \infty$ and $a_n = 0$  
- If the velocity is constant, then the only acceleration is the normal component, which is termed the centripetal acceleration (center seeking)
![[A256EB3A-8094-497D-95E5-534D76F6E4B4.jpeg]]
![[Recording 20220223100000.m4a]]
## Other useful Formula for Normal/Tangential
- If the tangential acceleration is constant
	- $s = s_0 + v_0 t + \frac{1}{2}(a_t)_c t^2$
	- $v = v_0 + (a_t)_c t$
	- $v^2 = v_0^2 + 2(a_t)_c(s-s_0)$
- If the path function is expressed as y=f(x), then the radius of curvature can be defined as
	- $\rho = \frac{[1 + (\frac{dy}{dx})^2]^{\frac{3}{2}}}{\frac{d^2 y}{dx^2}}$ 
![[Recording 20220223100205.m4a]]
## Summary of Normal-Tangential Problems
- Be careful of the wording of the problem to determine what components of acceleration you have (e.g. constant velocity means $a_t = 0$).
- Make sure you know the path function (to calculate the radius of curvature) or radius  of curvature
- If the given acceleration is not constant do not use the constant acceleration formulations!
![[Recording 20220223100226.m4a]]
## Curvilinear Motion: Cylindrical Components
- Sometimes, it is easiest to describe the path function using cylindrical coordinates
- If this is the case, then we must move to polar notation
- Polar notation is described by a radial coordinate (r) and a transverse coordinate ($\theta$), given from a fixed point
- Make use of radians where π radians = 180 degrees
![[2168C240-EF90-47EE-B08B-DD1119850570.jpeg]]
![[Recording 20220223100346.m4a]]
## Cylindrical Coordinates: Position and Velocity
- Position is defined by the radial coordinates: $\overrightarrow{r}=r\overrightarrow{u}_r$
- Velocity is defined by the time rate of change of this value, which makes use of a similar derivation from normal/tangential
	- $\overrightarrow{v} = \frac{d\overrightarrow{r}}{dt} = \frac{dr}{dt} \overrightarrow{u_r} = r \frac{d\overrightarrow{u_r}}{dt} = {v_r}\overrightarrow{u_r}+v_{\theta}\overrightarrow{u_{\theta}}$ 
		- $v_r = \frac{dr}{dt}$
		- $v_{\theta} = r \frac{d\theta}{dt}$
	- $v = \sqrt{(\frac{dr}{dt})^2 + (r\frac{d\theta}{dt})^2}$ 
- Velocity is always tangent to the path
![[AB9BAEC9-2C8A-427A-ACC4-0F38D6E28367.jpeg]]
![[Recording 20220223100519.m4a]]
## Cylindrical Coordinates: Acceleration (incomplete)
- The acceleration is defined as the time derivative of the velocity equation, which has quite a complicated derivation, because of the two product rules that must be incorporated
- $\overrightarrow{a} = \frac{d\overrightarrow{v}}{dt} = \frac{d^2r}{dt^2} \overrightarrow{u_r} + \frac{dr}{dt}\frac{d\overrightarrow{u_r}}{dt} + \frac{dr}{dt}\frac{d\theta}{dt}\overrightarrow{u_{\theta}} + r\frac{d^2\theta}{dt^2}\overrightarrow{u_{\theta}} + r\frac{d\theta}{dt}\frac{d\overrightarrow{u_{\theta}}}{dt}$
- $\overrightarrow{a} = a_r\overrightarrow{u_r} + a_{\theta}\overrightarrow{u_{\theta}}$
- $a_r = \frac{d^2r}{dt^2} - r(\frac{d\theta}{dt})^2$
- $a_{\theta} = r(\frac{d^2\theta}{dt^2}) + 2\frac{dr}{dt}(\frac{d\theta}{dt})$
- $a = \sqrt{[\frac{d^2r}{dt^2}-r(\frac{d\theta}{dt})^2]^2+[r(\frac{d^2\theta}{dt^2})+2\frac{dr}{dt}(\frac{d\theta}{dt})]^2}$ 
![[Recording 20220223100559.m4a]]
## Summary of Cylindrical Coordinates
- The functions of importance for cylindrical coordinates are:
	- $\overrightarrow{r_p} = r\overrightarrow{u_r} + z\overrightarrow{u_z}$
	- $\overrightarrow{v} = \frac{dr}{dt} \overrightarrow{u_r} + r\frac{d\theta}{dt}\overrightarrow{u_{\theta}} + \frac{dz}{dt}\overrightarrow{u_z}$ 
	- $\overrightarrow{a} = (\frac{d^2r}{dt^2} - r(\frac{d\theta}{dt})^2)\overrightarrow{u_r} + (r(\frac{d^2\theta}{dt^2})+2\frac{dr}{dt}(\frac{d\theta}{dt}))\overrightarrow{u_{\theta}} + \frac{d^2z}{dt^2}\overrightarrow{u_z}$ 
- The $\overrightarrow{u_z}$ terms are only valid for certain problems
- There are two general problem types:
	1. $r=r(t)$ and $\theta = \theta(t)$ are given, then we can take the derivatives
	2. $r=f(\theta)$, must find a relationship between the first derivatives of $r/\theta$ and the second derivatives of $r/\theta$ (this will make use of chain rule)
![[Recording 20220223100723.m4a]]
## Absolute Dependent Motion
- In some cases, the motion of one particle is dependent on the motion of another
	- Typically the particles are coupled by a linkage (shown as a rope and pulley system)
	- In the figure, as A moves down, B would move up
- Using the rope length method, we describe displacements in terms of the rope segments
	- $l_T = s_A + s_B + l_{CD}$ 
![[4F6E4F8B-4E4C-49BE-BFFB-AFBFDDAFD7A6.jpeg]]
___
### Derivation of the Rope Length Equation
- If we take the time derivative of the rope length equation, we get
	- $0 = \frac{ds_A}{dt} + \frac{ds_B}{dt}$
	- The total length and the length associated with pulley remain constant!
- Therefore, the velocities of the particles are
	- $v_A = -v_B$
	- The negative sign is for directionality associated with $s_A$ and $s_B$ 
- The accelerations can be found to be
	- $a_A = -a_B$

___
### Can This be More Complicated?
- Sure!
- The rope length equation becomes
	- $2s_B + h +s_A = l_T$
	- $2v_B = -v_A$
	- $2a_B = -a_A$
- Lengths in red stay the same at all instances in time and are ignored in the rope length equation
- ESTABLISH FIXED DATUMS!
![[A05B03A6-449B-43BC-8105-2AD4445053B9.jpeg]]

___

![[Recording 20220223101142.m4a]]
## Relative Motion of Two Particles
- In some instances, it is easy to relate the motion of two moving bodies using a translating axes
- A train is moving and a person is moving on the train
![[5F2077AF-C751-4657-920C-59BD2553AD27.jpeg]]

___
### Position
- The absolute position of each particle would need to be known to some fixed point
	- You would be interested in the relative position between the two points (e.g. A and B)
- The relative position of B with respect to A is denoted as $r_{B/A}$
- Therefore: $\overrightarrow{r_B} = \overrightarrow{r_A} + \overrightarrow{r_{B/A}}$
![[5F9DF955-ADD8-4499-A8E3-F566DBA5EBF8.jpeg]]

___
### Velocity/Acceleration
 - Take the time derivative of the relative position equation: $\overrightarrow{v_B} = \overrightarrow{v_A} + \overrightarrow{v_{B/A}}$
 - $\overrightarrow{v_{B/A}}$ is the relative velocity and it is important to note that only the magnitudes change because the directions change with the translating axes
 - Take the time derivative of the relative velocity equation: $\overrightarrow{a_B} = \overrightarrow{a_A} + \overrightarrow{a_{B/A}}$
 - $\overrightarrow{a_{B/A}}$ is the relative acceleration and its magnitude changes as well
 - These are vector equations.

___

![[Recording 20220223101348.m4a]]
