#### This is Ernie Su's quadopter project.

I write this blog to record my processing.

### Components in Quadcopter :
***
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
   * V2 Radio Telemetry
***

Before the build up of quadcopter, we need to set orientation, compass,  etc. by 
using micro USB  or the telemetry to connect flight controller with PC, using QGroundControl.
It's easy to calibrate with a small flight controller rather than a big quadcopter,
since you have to rotate the compass during calibration.
However, you can use a function in QGC called **Level Horizon** to calibrate pixhawk after you biult up.

### Build-up tips :
***
   1. Flight controller's direction must be the same as GPS's, 
      so it's good to arrange the components' wiring and placement after every part is fixed with the frame.

   2. Cable tie and 3M tape are helpful when your're stablizing all the components.

   3. The power wiring is important, too. This is mine here.

      <img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/power_wiring_1.JPG" width="400" height="400">

      I avoid the frame and make a 3.3V division from 12V by paralleling a 39k ohm resistor and a 13.3k one.

   4. B6AC has a function called **Balance Charge**, to use it you have to connect both two wires on battery to B6AC.

   5. Battery at high energy is **4.2V**,    low energy is **3.7V**,    overcharge is **3.2V**

   6. Propellers have 2 directoins, clockwise and counterclockwise.
      The **rising** surface is hitting the air so that quadcopter can go up.
      Find the rising surface and then you'll know if this prop is clockwise or not.
      Also, the tip is at the opposite direction to the prop, which makes it tighter.
***

### Notice :
***
* V2 Telemetry's **TX and RX are reverse** to those on flight controller because IN receives OUT and so on.
* FS-IA6's receiver's first 3 pins need to connect to pixhawk's **RC IN** and **left SBUS alone**.

<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/RC.JPG" width="400" height="400">

***

### References

Flight Controller pixhawk 2.4.8 Datasheet : <https://docs.px4.io/v1.9.0/en/flight_controller/pixhawk.html>

F330 Quadcopter Manual(Simplified Chinese) : <https://zhuanlan.zhihu.com/p/34909126>

I'll keep my blog updated.


<!---<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/frame_1.JPG" width="250" height="250">-->

<!---<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/2212_motor_1.JPG" width="250" height="250">-->

<!---<img src ="https://github.com/Ernie-Su/Quadcopter_F330/blob/master/Image/frame_with_prop_1.JPG" width="250" height="250">-->

