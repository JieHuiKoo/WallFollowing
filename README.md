# Wall Following Algorithm
Exploration of wall following algorithm with P control.

This project was implemented with the powerful CoppeliaSim (Edu version) simulator for design & analysis of robots. 
Scripting was done in Lua, a high-level programming language, with great API support by CoppeliaSim.

## Desired outcome
1) The robot will point its Sonar sensor at an angle toward its left
2) The robot will closely circle around one of the pillars, maintaining a desired distance from the wall

## Implementation
The control algorithm makes use of only proportional control, Kd.
The vital 2 lines of code are as shown.
```
speedBaseL = VC - .5*KP*(noisyDistance - DESIRED_DISTANCE)
speedBaseR = VC + .5*KP*(noisyDistance - DESIRED_DISTANCE)
```

## Video Demonstration
![wallfollowing](https://user-images.githubusercontent.com/31171083/160491822-509e210e-c7e1-4399-8ae0-57d10ceb4bfb.gif)
