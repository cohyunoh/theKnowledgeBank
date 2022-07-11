# Dynamics - Planar Kinetics of a Rigid Body: Force and Acceleration
___
## Mass Moment of Inertia
- Since a body has a definite shape and size, a force applied to a system can cause the body to translate and/or rotate
- Translation is governed by $\Sigma \overrightarrow{F} = m\overrightarrow{a}$
- Rotation caused by a moment is governed by $\Sigma M = I \overrightarrow{\alpha}$
- **I** is defined as the ==mass moment of inertia== and it isa body’s resistance towards angular acceleration
	- This is analogous to how mass is a body’s resistance towards linear acceleration
## Mass vs. Mass Moment of Inertia
- **The mass of an object does not change very easily**
	- Unless you are burning fuel or very long time scales
- The ==mass moment of inertia== **changes depending on the axis of rotation**, but about a particular axis of rotation it does not change (if mass does not change)
- **Flywheels** are *used to resist changes in angular motion in engines*; this helps to provide a nearly uniform power output from the engine and prevents the engine from stalling
	- Flywheels have a very large mass moment of inertia about the axis of rotation 
## Mass Moment of Inertia
- This moment of inertia is the second moment of mas about the axis of rotation
	-  $I = \int_{m} r^2 dm$ 
	- Units are $mass \times length^2$
- **r** is the moment arm to an elemental mass, *dm*
- If the rigid body is uniform and the axis of rotation goes through the mass center, than *I* is the same
	- If this is not true, then the moment of inertia is different
![[7B61624E-510B-408A-B5C5-0EA479BC6739.jpeg]]
## Planar Kinetics and Mass Moment of Inertia
- In planar kinetics, the axis rotation generally passes through the body’s center of mass, *G*
	- The moment of inertia about this axis is denoted as $I_G$
- If the body has a variable density, where $\rho = \rho(x, y, z)$, then $dm = \rho dV$
- In this case the moment of inertia becomes: $I = \int_{V} r^2 \rho dV$
- If density is constant as a function of volume: $I = \rho \int_{V} r^2 dV$
## Triple Integrals and More
- The previous equation may need to be solved using
	- $I = \rho \int_{x} \int_{y} \int_{z} r^2 dx dy dz$
	- This can typically be simplified to a single integral if you can choose your elements to have a differential dimension in one direction
- Assuming that $x=y$ 
	- $Disk Element \to dV = \pi y^2 dz$
	- $Shell Element \to dV = 2 \pi y z dy$
![[05A0AAF4-28E3-4650-81BD-77C5A8EC7399.jpeg]]
## Parallel Axis Theorem and Radius of Gyration
- If the moment of inertia through the body’s center of mass is known, the moment of inertia through any parallel axis can be found with this theorem
	- $I = I_G + md^2$
- *d* is the distance between the two parallel axes
- ==Radius of Gyration:== to tabulate values of *I*, some normalized value should be found
	- $k = \sqrt{\frac{1}{m}} \to I = m k^2$
## Composite Bodies
- The moment of inertia of different shapes can be added (or subtracted to get the total moment of inertia of the body)
- The parallel axis theorem may be needed to move the moments to the same axis of rotation
	- This is necessary if the mass centers do no overlap on the axis of rotation
## Regular, Common Shapes can be Tabulated
![[BFAEB038-17F7-4489-B87C-43714AB721DF.jpeg]]
## Regular, Common Shapes can be Tabulated if the Density is Constant - 2
![[EC6BC619-B655-4189-BB69-1507A999C88E.jpeg]]
## Regular, Common Shapes can be Tabulated if the Density is Constant - 3
![[27601EBB-E1C5-4947-9D05-93016B0A60AF.jpeg]]
## Planar Kinetics: Equations of Motion
- For this analysis, we will restrict ourselves to rigid bodies that are symmetrical with respect to a fixed reference plane
- At the same time, we will assume that the particular loading conditions are also symmetrical with respect to the same fixed reference plane
- These assumptions allow us to simplify the rotational equations of motion because the references plane cannot rotate but may translate with a constant velocity
![[044C9513-62D6-4096-BBA7-E4605EAE8743.jpeg]]
## Equation of Translational Motion
- The following equation is related to the mass center of the rigid body and assumes that the mass of the body does not change with time
	- $\Sigma \overrightarrow{F} = m \overrightarrow{a}_{G}$
	- $\Sigma F_x = m(a_G)_x$
	- $\Sigma F_y = m(a_G)_y$
- We will restrict this analysis to motion with a 2D plane
	- The example uses a Cartesian coordinate system; a normal-tangential or cylindrical system may be used in this formulation
## Equation of Rotational Motion
- For any particle not located at the center of mass (*P* is the axis of rotation in the z-direction)
	- $\overrightarrow{r} \times \overrightarrow{F}_i + \overrightarrow{r} \times \overrightarrow{f}_i = (\overrightarrow{M}_p)_i = \overrightarrow{r} \times m_i \overrightarrow{a}_i$
- The moments about P can also be expressed as a function of its acceleration
	- $(\overrightarrow{M}_P)_i = m_i [\overrightarrow{r} \times \overrightarrow{a}_P + \overrightarrow{r} \times (\overrightarrow{\alpha} \times \overrightarrow{r})]$
![[A52A0681-1180-4D4A-BA0A-87421728ADAC.jpeg]]
- Carrying out the cross-produces and summing over particles (looking only at accelerations), we get
	- $\Sigma M_P = -\bar{y}m (a_P)_x + \bar{x}m (a_P)_y + I_P \alpha$
	- Signs fully dependent on the following figure
![[D26B93DA-C7F8-4DAA-A410-154341387325.jpeg]]
## Equation of Rotational Motion - Final Form
- If point P coincides with the mass center
	- $\Sigma M_G = I_G \alpha$
- If point P does not coincide with the mass center, but its fixed (e.g. at a linkage) then the formula above is still valid, if you move *I*
- If point P does not coincide with the mass center and is an arbitrary axis of rotation then the following formula is used
	- $\Sigma \overrightarrow{M}_P = -\bar{y}m (a_G)_x + \bar{x}m(a_G)_y + I_G \alpha$
## Images of Rotational Motion Equations
![[2E43DFC8-F0AC-4EDD-A1F4-CA81B2FF4453.jpeg]]
## General Application of the Equations of Motion
- In our case, there are three independent scalar equations of motion
- They are:
	- $\Sigma F_x = m(a_G)_x$
	- $\Sigma F_y = m(a_G)_y$
	- $\Sigma M_G = I_G \alpha$ or $\Sigma M_P = -\bar{y}m(a_G)_x + \bar{x}m(a_G)_y + I_G /alpha$
- Be careful with the signs on the $\bar{x}$ and $\bar{y}$; these signs were derived from the figure used in notes