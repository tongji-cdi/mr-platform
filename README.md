# Template project for CDI's Collaborative MR Platform

## Basic Usage
**Note: This part of the guide is a prerequisite for any recipes below.**

Creating a project for the MR platform is simple. (But I need more time to write this tutorial.)

## Recipes
Here are some commonly used set-ups when developing a new project.

### I just want motion tracking!
Motive already provides pretty good support for tracking markers, so you will not need Unity for this recipe.
This is commonly used for experiments in wearble devices or any studies of human motion.
The full guide can be found [here]()

#### You will need:
* Motive calibrated and running.
* Markers

#### Summary of steps:
1. Place markers on places you want to track.
2. Hit RECORD in Motive software.
3. Cleanup tracks as best as you can.
4. Export the data into CSV and do further clean-up.

### Vanilla MR
This recipe is the basic setup for an interactive MR scene, consisting of virtual VR objects as well as motion-tracked physical objects.
The full guide can be found [here]()

#### You will need:
* Motive calibrated and running.
* Unity
* Markers
* An additional client PC to deploy to.

#### Summary of steps:
1. Place markers on objects you want to track.
2. Add each object as Rigid Body in Motive, and configure pivot points.
3. Copy the Unity project template. Set up project path and NetworkManager.
4. Add models into the Unity scene. Attach the OptitrackRigidBody script to objects, and fill in the User IDs.
5. Add virtual assets and do all the Unity stuff you need.
6. Package for client deployment.

### Collaborative MR
#### You will need:
* Motive calibrated and running.
* Unity
* Markers
* Multiple client PCs to deploy to.

#### Summary of steps:
1. Do steps 1-4 of Vanilla MR.
2. For dynamic virtual assets, make prefabs, then use the provided script to turn them into asset bundles.
3. Add static virtual assets and do all the Unity stuff you need.
4. Package client programs for each machine and deploy.

### Screen-based Interactions
TODO.

### Interactive Projection Mapping
TODO.


## Set up from scratch
This section describes the process of bootstrapping the MR platform from scratch. It has quite some caveats, so please follow this guide carefully. 

### Requirements
* A Windows PC with a decent enough graphics card (> 1060 3GB).
* Set up the Oculus app.
* [Install XAMPP](https://www.apachefriends.org/index.html) (preferably on the D: drive).

More TBD.
