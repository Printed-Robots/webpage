---
date: 2020-06-06
title: "Watch this cute robot explore the world!"
linkTitle: "Cute robot explores the world"
description: "This is the initial version of my selfbalancing robot"
author: powJ2 ([@J2pow](https://twitter.com/j2pow))
---

## Watch it explore the world!

{{< youtube id="p-f6EHCXiaI" autoplay="false" >}}

## Details

### For the technical enthusiast

This is a ROS 2.0 based robot using a Raspberry Pi 3b with a Navio2 Sensor board. To balance the robot there are two PID controllers in use - one for velocity and one for the angle. While I can measeure the angle, I currently have no sensor to measure the velocity. This makes it hard for the robot to stand on uneven ground. But fear not: Sensors are on their way :)


### For the hardware fan

The structural parts are 3d printed. To move the robot there are two brushless gimbal motors, which are awesomly quiet! And .. there is a small fan to cool the robot ;)


### For the open source lover

The code used to make this robot balance can be found here
- https://github.com/jsqu4re/balance_robot
- https://github.com/jsqu4re/balance_robot_msgs
- https://github.com/jsqu4re/n2r2
