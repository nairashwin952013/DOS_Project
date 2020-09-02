# Internet Of Things in Xinu

### Overview

Designing and implementing a device driver for a thing in the Internet of Things (IoT) is different from what is traditionally done in a computer. 
This is because in the latter, the objective is to allow processes in an OS to access and utilize devices that are either connected directly to the computer, 
or remotely through the network. In an IoT, things should utilize and use each others. Hence, both processes internal to a thing (e.g., 
Xinu processes running on a Beagle Bone Black platform) as well as other nearby things (e.g., other Beagle Bone Black or Dragon platforms) should be able 
to access and utilize each others as devices. Here, we use device and thing loosely interchangeably. 

### Objectives

This project aims to engage in a challenge based learning experience in which each group will design and implement Xinu device drivers for things that can 
connect into a Beagle Bone Black (BBB), and for the BBB itself as a whole platform (as a thing)!

### Technology Scope

Coverage should include GPIO as minimally abstracted low-level I/O devices, covering several sensors/actuators and analog/digital interfaces. One combination 
of GPIO should be supported as a higher-level abstracted device. Finally, applications running on the BBB that utilize GPIO should be supported as high-level 
abstracted device. 

### Concerns:

- In which way does the high-level interface need to change? 
- What are the needed I/O operations? and are there any new operation abstractions that need to be introduced and supported? 
- Would the high-level I/O interface (even the one you would design for Xinu processes) be appropriate for other external things and devices? 
- Or the same physical device should have multiple interfaces?
- One for local access by Xinu processes, and others for access by external things?
