Simple Physics Engine
===================
It's View is based on Unity.
The Physics is implemented in C#

<img src="img/Picture1.png" width="300">
<img src="img/Picture2.png" width="300">
<img src="img/Picture3.png" width="300">

[Demo](https://www.youtube.com/watch?v=K6Fja1hseOY&feature=youtu.be)

### Implement

[Constraint Tutorial](https://www.youtube.com/watch?v=iwEmcWjrcbA&list=PL-yGOsK2iEWjXERY62X2bsa17a2UoA8GK&index=4)
This series course help me to understand what is contraint and how a physics engine work. It is very useful to me.

#### 1. Physics Model

<img src="img/PhysicsEngine.png" width="300">

* 1.Update Collision : Update Contact Manifold From Collision Model
* 2.Compute Island : Compute Island to Solve Constraint(Ignore object if it is sleeping, and no object collide with it)
* 3.Solve Contact : Impulsed base response, Penetration constraint
* 4.Update Sleep State : Change the object state if its linear velocity and angular velocity stay at low speed for a period of time

#### 2. Collision Model

<img src="img/CollisionEngine.png" width="300">

* 1.GJK Algorithm : Check overlap, Get EPA Start Simplex
* 2.EPA Algorithm : Get Penetration Vector, Penetration Depth
* 3.Clipping : Get Contact Points By Clipping, Get Contact Manifold
* 4.Update Contact Points for warm start(Use Distance between Contact Points)






