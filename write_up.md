# Path-Planning-Project Write Up
bolin zhao (bolinzhao@yahoo.com)

## Overview
To generate a smooth trajectories
- add spline.h

To determine whether change lane and the target vehicle
- add BehaviorPlanner in behavior_hpp/cpp

### main.cpp

### Behavior Planner
#### Current lane
Utlizie the d value in Fernet coordinate to judge currently the car in which lane.
#### Closest vehicle
To give the current vehicle information in Frenet coordinate and lane, get the closet vehicle's distance and velocity in this lane.
#### Lane Score
Based on the Sensor fusion data to get a score over three lanes. The score takes the distance and velocity information into account and the higher the score is, the better choice for that lane.
#### Lane planner
The lane planner give back a gain on d value to tell the car whether change lane or not.
