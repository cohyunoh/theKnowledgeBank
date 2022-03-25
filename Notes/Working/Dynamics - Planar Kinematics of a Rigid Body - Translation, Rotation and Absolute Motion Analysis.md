# Dynamics - Planar Kinematics of a Rigid Body - Translation, Rotation and Absolute Motion Analysis
___
## Planar Motion
- This is when ==all of the particles of a rigid body move along paths== which are **equidistant from a fixed plane**
	- Make sure to remember that we are focused on rigid bodies here and not rigid bodies represented as particles and not individual particles
- There are three types of motion that a rigid body can experience
	1. ==Translation:== a randomly drawn line in a rigid body remains *parallel to its original orientation during the entire motion* and it has the **same length** (e.g. no deformations)
		- All particles maintain the same orientation: **rectilinear vs. curvilinear translation**
	2. ==Rotation about a Fixed Axis:== all particles *move in circular paths, except those along the axis of rotation*
		- All particles maintain the same orientation after the rotation
	3. ==General Planar Motion:== a *combination of translation and rotation* (for us, the rotation will occur about an axis perpendicular to translation plane)
## Translation and Rotation

^018985

![[EE29268E-7815-4FEF-801E-04845EE3E499.jpeg]]
## General Planar Motion
![[802813F6-81E0-4BF2-90A7-9FF09AC4A6B7.jpeg]]
![[Recording 20220302092938.m4a]]
## Polar Coordinates
- May be used to **describe rotations or general planar motions**
- ==Pure translation== is easy and follows all of the same rules that we have discussed so far
- Position of a Translating Rigid Body
![[C17CA48B-A04A-499B-BA02-78416F85A999.jpeg]]

![[Recording 20220302093150.m4a]]
## Velocity and Acceleration of a Translating Rigid Body
- Velocity is the time derivative of position
	- $\frac{d}{dt}(r_B = r_A + r_{B/A}) \to v_B = v_A + v_{B/A}$
	- $v_{B/A} = 0 \to$ rigid body
	- $v_B = v_A$
- Acceleration is the time derivative of velocity
	- $a_B = a_A$
- All kinematic relationships discussed still hold (acceleration does not need to be constant)
- *Refer back to [[Dynamics - Planar Kinematics of a Rigid Body - Translation, Rotation and Absolute Motion Analysis#^018985|here]]*
![[Recording 20220302093610.m4a]]
## Rotation about a Fixed Axis
- Any point P on a rigid body that rotates about a fixed axis, travels along a circular path
- Points cannot undergo radial motion (e.g. r remains the same), radial lines experience radial motions
- Angular position is defined by $\theta$, which is the angle that r makes with regard to some reference line
![[35B12EA0-84E3-4B44-8111-B9290CD0DEA4.jpeg]]
### Displacement/Velocity
- Angular displacement is the change in angular position, measured as a $d\theta$
	- The magnitude is given in degrees/radians/revolutions
	- The direction is given by the right-hand rule (counter-clockwise is positive along a positive axis of rotation)
- Angular velocity is the time rate of change of angular position
	- $\overrightarrow{\omega} = \frac{d\overrightarrow{\theta}}{dt}$ 
	- $\omega$ is vector with magnitude in rad/s and direction as given by the right-hand rule
### Angular Acceleration
- Angular acceleration is the time rate of change of angular velocity
	- $\overrightarrow{\alpha} = \frac{d\overrightarrow{\omega}}{dt} = \frac{d^2\overrightarrow{\theta}}{dt^2}$
	- $\alpha$ acts in the same line as $\omega$ but may have a different direction (if it is accelerating or decelerating)
- We can also obtain the following:
	- $dt = \frac{d\overrightarrow{\omega}}{\overrightarrow{\alpha}}$
	- $\overrightarrow{\omega} = \frac{d\overrightarrow{\theta}}{\frac{d\overrightarrow{\omega}}{\overrightarrow{\alpha}}}$  
	- $\overrightarrow{\omega}d\overrightarrow{\omega} = \overrightarrow{\alpha}d\overrightarrow{\theta}$ 
![[C7A19461-78B8-4DDD-8E18-877469CAB79C.jpeg]]
### Constant Angular Acceleration
- If $\alpha = \alpha_c$ then the previous equations can be integrated to get:
	- $\omega(t) = \alpha_c t + \omega_0$ 
	- $\theta(t) = \frac{1}{2} a_c t^2 + \omega_0 t + \theta_0$
	- $\omega^2 = \omega_0^2 + 2\alpha_c(\theta - \theta_0)$ 
- This is analogous to the linear kinematic equations that were described before
### Motion of Point P
- As the rigid body rotates, point P follows a circular path, that can be quantified
- As we have learned, the position of P is defined by the position vector $\overrightarrow{r}$
- The curvilinear displacement of P is defined by an arc length, which is defined as: $ds = rd\theta$
- By taking the time reate of change of this arc length formula, one gets the linear velocity at an instant in time (notice these are not vectors)
	- $\frac{ds}{dt} = v = r\frac{d\theta}{dt} = r\omega$
### Linear Velocity - Continued
- The direction of this velocity is tangent to the circular path
- In vector form, this is represented as: $\overrightarrow{v} = \overrightarrow{\omega} \times \overrightarrow{r_p}$
	- $\overrightarrow{r_p}$ is off of the rotation axis, does not need to be $\overrightarrow{r}$ 
![[CC67445A-A327-462A-AFCA-540355816F30.jpeg]]
### Linear Acceleration of P
- The acceleration of point P is composed of 2 parts
	- Normal acceleration: $a_n = \frac{v^2}{r} = \omega^2r$ 
	- Tangential acceleration: $a_t = \frac{dv}{dt} = \alpha r$
- The normal acceleration is the time rate of change of the velocity direction
- The tangential acceleration is the time rate of change of velocity (this depends on acceleration of deceleration)
- In vector form:
	- $\overrightarrow{a} = \frac{d\overrightarrow{v}}{dt} = \frac{d}{dt} (\overrightarrow{\omega} \times \overrightarrow{r_p}) = \frac{d\overrightarrow{\omega}}{dt} \times \overrightarrow{r_p} + \overrightarrow{\omega} \times \frac{d\overrightarrow{r_p}}{dt} = \overrightarrow{\alpha} \times \overrightarrow{r_p} + \overrightarrow{\omega} \times (\overrightarrow{\omega} \times \overrightarrow{r_p})$
	- $\overrightarrow{\alpha} = \overrightarrow{\alpha_t} + \overrightarrow{\alpha_n} = \overrightarrow{\alpha} \times \overrightarrow{r_p} - \omega^2\overrightarrow{r_p}$ 
	- Magnitude of $a = \sqrt{a_t^2 + a_n^2}$
- The second to last equation is only applicable in two dimensions
### Acceleration Figures
![[E74F0F33-9D69-4EC0-9ADC-06E2C1810148.jpeg]]
![[Recording 20220302095517.m4a]]
## Absolute Motion Analysis
- This is one technique that can be usted to determine the position of a body that undergoes general planar motion (e.g. translation and rotation)
- By knowing the angular rotation of a line and the motion of one point, you can describe the motion of the body
- The trick is to relate the rectilinear motion of a point on the velocity(e.g. the velocity and acceleration) to the rotation of the body (e.g. the angular velocity and the angular acceleration)
- Practically, trig rules will be used extensively to make these relationships
![[Recording 20220302100726.m4a]]
## Two Rotating Bodies in Contact
- Meshed Gears or a belt around a drum or pinned linkages
- At the point of contact the linear velocity and the tangential component of the linear acceleration must be the same
	- This comes in to play when making use of gear ratios to alter the rotation
- The normal acceleration will not be the same unless the radius of the two gears are the same
- Note that this concept is how we move through gear boxes or other connected components and will be used extensively in rigid body dynamics
### Two meshed gears
![[6FEA34EC-FEAC-4E68-851D-5F5B593D23F0.jpeg]]
![[Recording 20220302101242.m4a]]