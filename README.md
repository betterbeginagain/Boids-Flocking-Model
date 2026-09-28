# Boids-Flocking-Model
This is an interactive 2D Boids flocking model with sliders for separation, alignment, and cohesion.
https://betterbeginagain.github.io/Boids-Flocking-Model/

In 1986, computer graphics researcher Craig Reynolds tackled an animation problem: animating a flock of hundreds of birds frame by frame by hand was nearly impossible, and scripting a central path for them made the flock look stiff and mechanical.

Reynolds realized that real flocks do not follow a flight plan or a commander. Instead, he treated each bird as an independent autonomous agent—shortened to "boid" (a blend of "bird-oid object"). He published the concept at SIGGRAPH in 1987.

# The Three Steering Behaviors
Instead of coding the complex path of the whole group, Reynolds gave each boid only a limited field of view and three simple steering rules computed on every animation frame:

- # Separation (Collision Avoidance) 
  Steer away from flockmates that are too close to avoid crashing into each other.

- # Alignment (Velocity Matching) 
  Steer to match the average heading and speed of nearby flockmates.

- # Cohesion (Flock Centering) 
  Steer toward the average center of mass of local flockmates to keep the group from drifting apart.

Each boid calculates a steering force for all three rules, adds them together with assigned weights, and updates its velocity. With only these local rules, complex behaviors like flowing around obstacles, splitting into sub-flocks, and rejoining appeared entirely on their own.

# Impact on Hollywood & Gaming
Reynolds' algorithm changed computer animation and artificial life forever:

- # The Hollywood Debut
  Tim Burton’s Batman Returns (1992) used a modified Boids system to animate swarms of bats and armies of marching penguins.

- # The Lion King (1994)
  Disney used flocking logic to animate the famous wildebeest stampede in 3D, creating realistic animal movement without hand-keyframing every beast.

- # Modern Games
  Nearly every modern game crowd system—from schools of fish in Subnautica to civilian crowds in Assassin's Creed uses Reynolds' steering behaviors as its core foundation.
