---
layout: page
title: Osprey Drone
---

### Background
I realized that it would be a cool project to make my own VTOL drone with the ability to swivel it's wings during takeoff and landing. The benefits would be a small takeoff footprint, while taking advantage of the energy efficiency of a fixed-wing aircraft (versus a quadcopter).
The drone for starters will be remote controlled using a standard radio remote control, however, will hopefully act as a platform for future projects.

### Features and Completed Work
Mechanical work:
  - Designed the drone from scratch in Solidworks using the Bell Boeing Osprey as a reference
  - 3D printed all parts of the drone and glued using interlocking joints and a lightweight resin
  - Created mounts for motors/servos compatible with various available fasteners
  - Started Covering the drone with covering film
Firmware/Electrical work:
  - Used an STM32F0 to convert the 6-channel input from the radio receiver Using a 6channel receiver to control mode specific surfaces/features (7+ channels) 
  - Prototyped a small board to mux the radio receiver outputs to the STM32F0, which in turn controlled all servos and motors connected
  
### Demos
The following pictures are stages in the mechanical development of the drone
![](images/Aerobody1.jpg)
![](images/Aerobody2.jpg)
![](images/Aerobody3.jpg)

The following video is a demonstration of the wing/servo controls routed through the STM32F0 micro.

<iframe width="643" src="https://www.youtube.com/embed/ZOA1hxlcov8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Future Work
Mechanical:
  - Covering film needs to be completely applied without as many wrinkles (may need to slightly re-design fuselage/wings)
  - Create internal mounts for computers/receivers
  
Software: 
  - Add a Raspberry Pi camera/compute to enable the drone to do more advanced tasks (such as stream heads-up video back to base controller)