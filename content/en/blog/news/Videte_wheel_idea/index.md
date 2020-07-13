---
date: 2020-07-08
title: "Videte Wheel to climb Stairs"
linkTitle: "Robot tries to climb stairs"
description: "This is the second version of my self balancing robot"
author: powJ2 ([@J2pow](https://twitter.com/j2pow))
---

Originally published on [discourse.ros.org](https://discourse.ros.org/t/self-balancing-robot-tries-to-climb-stairs/14545)

There was some encouragement to post about my balancing robot here on discourse. So I decided to write my first entry. If you want to know more, feel free to leave a comment below :) Please also write about your ideas and whether you would like to build one of these robots yourself.

# WHY

Currently, due to current global situation, I have some free time to focus on fun projects. And this is a project which I had in mind for several years now. My goal is to build a small robot, which is capabale to ride stairs elegant [(Not so elegant but simple solution)](https://youtu.be/9NsLqvjIIIM) and simple [(Not so simple but actually quite good solution](https://youtu.be/-u7Y6kz7S8w) and [much less simple but awesome solution)](https://youtu.be/B4D1hpGiQ_k)

Most solutions I found were different from what I wanted to do. But there is one video, which must be mentioned here. Because it helped me to come up with my design. [(Clever design linked here)](https://youtu.be/gs_H3TOrLxw)

The benefit of this construction is, that the balancing capabilities of the robot are available even, if the wheel is "stuck" next to a wall/staircase/etc. Due to this benefit the robot won't be pushed away by the wall but can start to push against it and (if it has enough power) climb it [(Not yet climbing things)](https://twitter.com/J2Pow/status/1268248880422010881)

As you have seen it is the **goal** to climb stairs and the robot is not yet able to do it.

But: Utilizing only a single, simple PID controller to make the robot balance, shows - in my opinion - some potential, which is enabled by this design choice.

# WHAT

I am using **ROS 2.0** [*(Play cheering background sound here)*](https://youtu.be/IxAKFlpdcfc) on a Raspberry PI 3b with a Navio2 board for the orientation measurement. Two brushless gimbal motors and two quite simple brushless gimbal motor controllers to drive the robot around. And there are a lot of 3d printed parts to form the robot itself. I hope to make these parts open source soon. [(Go here to find out more)](https://printed-robots.github.io/)

The current performance of the robot shows in my opinion some potential, but I feel there is first and foremost not enough power available in the drive train.

# PLANS

So my plan is to update the simple unregulated brushless controllers with the **ODrive** board and add some encoders to have more power while not overheating the motors.

As soon as it can drive around safely. I would like to add some autonomous driving capabilities utilizing the lidar on top (and maybe giving the lidar some more space to better observe the environment) with the ros2 planner package. And of course I want to ride stairs (.. in matching scale)

Thats it for now :) Feel free to comment below and ..

**THANKS FOR READING!**

Enjoy making fun stuff with ros!