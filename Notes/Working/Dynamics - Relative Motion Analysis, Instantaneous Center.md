# Dynamics - Relative Motion Analysis, Instantaneous Center
___
## Relative Motion Analysis: Velocity
- This is a technique to analyze the general planar motion of a rigid body by **separately** analyzing the translation and the rotation
- Definitions: the translating reference frame does not rotate and the motion of A is known at the particular time of interest
![[3D0A3930-2760-4195-91AD-B873A111B722.jpeg]]
## Position Definitions in this Reference Frame
- $\overrightarrow{r}_A$ specifies the location of A, termed the base point
- $\overrightarrow{r}_{B/A}$ is the relative position of B with respect to A
- Therefore, he position of B is defined by: $\overrightarrow{r}_B = \overrightarrow{r}_A + \overrightarrow{r}_{B/A}$
## Displacement Definitions in this Reference Frame
- After some time *dt*, A and B undergo some displacement by $dr_A$ and $dr_B$, respectively
- *Since A is our base point, the entire bar translates by $dr_A$*
- From this translation B moves to B’ and the bar is rotated by $d\theta$
	- B’ undergoes a relative displacement of $dr_{B/A}$
### Displacement Figures
![[64C81613-6351-4747-8A36-058F1739452F.jpeg]]
## Velocity Definitions
- To determine the velocity of A and B, take the time rate of change of the position equation
	- ![[4C7A3E30-8BDD-41F4-A42E-F2FD0BA34A36.jpeg]]
- The $\overrightarrow{\omega} \times \overrightarrow{r}_{B/A}$ is a relative velocity term and can be written as $\overrightarrow{v}_{B/A}$ 
- Hint: when choosing points A and B, it is best to choose points that can easily be described; for instance pin connectors are good choices
    
![[73221169-8F8B-46BF-BFDB-484F11B77A05.jpeg]]
## Instantaneous Center of Zero Velocity
- Only for velocity
- This is an easier way to obtain the velocity of any point ($\overrightarrow{v}_B$) by choosing the base point ($\overrightarrow{v}_A$) to have a zero velocity at the instant in time that you are interested in
- Therefore, $\overrightarrow{v}_A = 0$ and $\overrightarrow{v}_B = \omega \times \overrightarrow{r}_{B/A}$
- The point A, is always the point of contact between the body undergoing general planar motion and the plane of motion
- The body is assumed to be rotating about the instantaneous center of zero velocity (IC), instead of its axis of rotation
	- Note that the IC typically moves with time, but we are only interested in one time point
### Instantaneous Center Figure
![[748709B1-C129-4B9F-B68D-939B43AD93D8.jpeg]]
- **No slip condition**
	- At any point of contact, the velocities match
- In the next time instant, the IC is in the same spot, just translated to a different location
## Location of the IC (some bodies do not have a point of contact)
- To locate the IC we use the fact that the velocity of any point on a rigid body is always perpendicular to the relative position vector directed from the IC to the point
- If the velocity of one point and the angular velocity of the body are known, the IC can be located
![[1D0402C4-F761-4927-A53B-86537C2BF9E8.jpeg]]
## Location of IC, continued
- The lines of 2 non-parallel velocities $\overrightarrow{v}_A$ and $\overrightarrow{v}_B$ are known; draw lines that are perpendicular to the velocities until they intersect
	- The intersection is the location of the IC at this particular instant in time
- The magnitude and direction of two parallel velocities $\overrightarrow{v}_A$ and $\overrightarrow{v}_B$ are known
	- The IC is found by similar triangles
![[FA61C2AA-23A6-4AAE-A3A0-41AF1D9BFCC3.jpeg]]
![[CC8AA945-3260-41E2-8FD4-3D27F76E74E6.jpeg]]
## IC Rules
- The IC acts in one particular location for one instant in time
- Therefore, in a different configuration, you must solve for a new IC
	- This may make the process of finding the IC laborious if time is a component of your problem.
	- However, if you are interested in many velocities at one instant in time, IC may be worth it.
- A collection of all of the ICs is termed the centroid for that motion
	- The IC typically does not have a zero acceleration (since the body has a general planar motion) and therefore this method cannot be used to quantify the acceleration of a body during general planar motion
## Relative Motion Analysis
- To obtain the acceleration of a body, you must quantify the time rate of change of the relative velocity equation
	- ![[49470FB2-A76C-4018-B17C-1AFFD2A9C5ED.jpeg]]
- These accelerations are measured with respect to the fixed axis
## Derivation of Relative Acceleration
- $\frac{d\overrightarrow{v}_{B/A}}{dt}$ is measured relative to the translating coordinate system (x’y’)
	- Since x’y’ is fixed at A, it will look as if B is rotating about A
- Therefore, $\overrightarrow{a}_{B/A}$ will have two components
	- One of these is tangential to the path and the other is normal to the path
		- $\overrightarrow{a}_B = \overrightarrow{a}_A+(\overrightarrow{a}_{B/A})_t + (\overrightarrow{a}_{B/A})_n$
- Since these terms are relative to A and represent a circular path about A
	- ![[3F0202CC-9B5F-48AC-B655-2ABEAF7FDFF5.jpeg]]
### Acceleration Images
![[3734C833-B2EC-414F-95E4-0B3005590D97.jpeg]]
## Complete Acceleration Formulation
![[CAEE89BE-22EA-495C-B77D-194CBB233B8A.jpeg]]
-  last term would need to be a cross‐product if the general planar motion was in three dimensions; in two‐dimensions it simplifies to what is written e.g. $\overrightarrow{\omega} \times (\overrightarrow{\omega} \times \overrightarrow{r}_{B/A}$
• When looking at the same pin, the acceleration of the point must be the same
• If the two bodies pass without slipping (e.g. gears), $\overrightarrow{a}_t$ will be the same but $\overrightarrow{a}_n$ will be different
 ### Acceleration for Two Bodies
 ![[07FB105E-0E95-451F-AEA9-381F6A0117F1.jpeg]]
 ## Relative Motion Analysis: Rotating Axes
 - This analysis is helpful when two rigid bodies are in contact with each other and are sliding at their connections
 - It is best to use a coordinate system that translates and rotates with one of the bodies
 - This is also useful for points not on the same body but on the same mechanism
	 - These points have some movement in common, but differ in some other movement
## Rotating Axes: Position
- The relative position vector must be measured with respect to the translating/rotating coordinate system to the translating coordinate system
![[0BEB194C-1105-4775-998C-5FE527D8D12F.jpeg]]
## Position Definitions Continued
- Point A has a velocity and acceleration of $\overrightarrow{v_A}$ and $\overrightarrow{a_A}$
- The angular velocity and acceleration is defined for the translating/rotating coordinate system, which is based at A
- ==Angular velocity== is defined as $\overrightarrow{\Omega}$ 
- ==Angular acceleration== is defined as $\frac{d\overrightarrow{\Omega}}{dt} = \dot{\Omega}$ 
## Rotating Axes: Velocity
- The velocity of B is defined by taking the time derivative of the position equation, to get (complete derivation is lengthy):
![[0EA1F074-4305-40D5-9352-6AD5A67F0B5B.jpeg]]
## Rotating Axes: Velocity - continued
- For small angles $d\hat{i}$ and $d\hat{j}$ are equal to $d\theta$
	- The direction of $d\hat{i}$ acts in the $\hat{j}$ direction
	- The direction of $d\hat{j}$ acts in the $\hat{i}$ direction
![[DC1972DF-1C76-4B75-B0FA-92114BDBA12A.jpeg]]
## Rotating Axes: Acceleration
- The acceleration of B is obtained from the time derivative of the velocity equation
![[881239A6-2E7E-4E8E-B951-9DB2A08D3ABC.jpeg]]
- All $\Omega$ terms and terms with xyz subscripts are relative to the translating/rotating coordinate axis