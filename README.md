# Crazyflie Monopod Perching
This repository contains a suite of code that allows the [Crazyflie quadcopter](https://www.bitcraze.io/products/crazyflie-2-1/) to perch on a monopod. It mainly consists of modifications to the [Crazyflie firmware and controller](https://github.com/bitcraze), as well as some additions to allow for data plotting to better understand the behaviour of the quadcopter.

The repository also includes code for controlling the quadcopter through a USB gamepad connected to the computer.

![image](https://github.com/f-rower/Crazyflie-monopod-perching/blob/master/Results/Pictures/2017_08_25/IMG_20170810_175315.jpg?raw=true)

# Why monopod perching?
Being able to balance on a single point provides the quadcopter with a great deal of flexibility on where to land, since a minimal perching area is required. Perching on a monopod allows the quadcopter to rotate around while perching as well, which could be helpful in the context of surveillance and reconnaisance.

Monopod perching could extend mission duration where landing areas are unavailable, such as earthquake-affected areas.

In the case of the Crazyflie quadcopter, for example, the quadcopter has a total flight time of approximately 7 minutes. However, it can perch for up to 55 minutes. For missions where perching on challenging surfaces is required, and continuous flight is not required, this could mean that mission duration could be extended almost 8 times!

The best thing is that monopod perching can be achieved through a fairly straightforward tuning of the double-loop PID controller parameters. A simple centre-of-mass model of the quadcopter was created to estimate the PID parameters, which were then fine-tuned using a custom-made test rig.

Two separate sets of parameters were used during flight and perching, which were autonomously modified by the custom quadcopter firmware.

# Report, images, and results

You can read the report of this work [here](https://github.com/f-rower/Crazyflie-monopod-perching/blob/master/Results/report/EF08_Report_2.pdf)

You can check out some images [here[(https://github.com/f-rower/Crazyflie-monopod-perching/tree/master/Results/Pictures)

Last updated: 2024 07 02
