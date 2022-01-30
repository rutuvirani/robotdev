# Developing with Spot

Official [Spot SDK docs](https://dev.bostondynamics.com/).

The Spot API follows a client-server model. Client applications
communicate with on-board services over a network connection.

The Spot services can be categorized into "core", "robot" and "autonomy" as follows:

![spot sdk viz](https://d33wubrfki0l68.cloudfront.net/f34bcc5ff400782c699351096b289ed9f943164a/32716/_images/api_top_level.png)

## Facts about Spot Hardware and Mechanical Design:

1. it has 5 pairs of stereo camears that provide black and white images and video.

2. A "hip" refers to the joint that connects the body and a leg, shown below

   ![hip](https://i.imgur.com/pyMhUtQ.png)

   Each hip joint has two actuators. One rotates around the X axis, and one rotates around the Y axis.

   >An [actuator](https://en.wikipedia.org/wiki/Actuator), upon receiving a control signal, converts energy (e.g. electric current, hydraulic pressure, pnumatic pressure) into mechanical motion.

    This diagram clearly defines the axes of Spot:

    ![spot axes](https://d33wubrfki0l68.cloudfront.net/dd322f87de0e52e2cf381e96d4392b135b6dca61/8fd3c/_images/spotframes.png)


3. A knee joint connects the upper leg and the lower leg. has one actuator

4.