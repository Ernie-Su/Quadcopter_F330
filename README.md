### This is Ernie Su's quadopter project.

I write this blog to record my processing.

First, I use the follwing components in my quadcopter:
* F330 Frame
* 2212 Motor x 4
* 8045 Propellers x 4
* ESC x 4
* UBEC
* B6AC (Charger)
* 3S, 4000mah Battery
* Pixhawk 2.4.8
* M8N GPS
* PPM Encoder
* 6S FLY-SKY Telecontroller

Before the build up of quadcopter, we need to set orientation, compass,  etc. by 
using micro USB to connect flight controller with PC, using QGroundControl.
It's easy to calibrate with a small flight controller rather than a big quadcopter,
since you have to rotate the compass during calibration.

There are some tips when it comes to quadcopter's build-up:
1. Flight controller's direction must be the same as GPS's, 
   so before every part is fixed with the frame, 
   it's good to arrange the components' wiring and placement.

2. Cable tie and 3M tape are helpful when your're stablizing all the components.

3. The power wiring is important, too. This is mine here.
   <img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/power_wiring_1.JPG" width="400" height="400">
   I avoid the frame and make a 3.3V division from 12V by paralleling a 39k ohm resistor and a 13.3k one.
   <!--<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/frame_1.JPG" width="250" height="250">-->

4.

I'll keep my blog updated.


<!---<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/frame_1.JPG" width="250" height="250">-->

<!---<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/2212_motor_1.JPG" width="250" height="250">-->

<!---<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/frame_with_prop_1.JPG" width="250" height="250">-->

