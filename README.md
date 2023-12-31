# MobileRobot-Openloopcontrol
## Name: Goutham.K
## Ref.No: 212223110019
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure



## Program
```python
from robomaster import robot
import time
from robomaster import camera

if name == 'main':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)


    ep_chassis.move(x=2.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0.5, y=0, z=75, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=1, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=125,effect="on")

    ep_chassis.move(x=0, y=0, z=90, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=100,b=125,effect="on")

    ep_chassis.move(x=1.6, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=100,b=125,effect="on")

    ep_chassis.move(x=0, y=0, z=-25, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=150,b=0,effect="on")

    ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=153,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=40, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=0,effect="on")

    ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=125,effect="on")

    ep_chassis.move(x=0, y=0, z=95, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=50,g=100,b=150,effect="on")

    ep_chassis.move(x=2.1, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=85,g=0,b=120,effect="on")

    ep_chassis.move(x=0, y=0, z=80, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=128,b=0,effect="on")

    ep_chassis.move(x=0.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=0,b=255,effect="on")

    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```
 



    
   
## MobileRobot Movement Image:

![Screenshot 2023-12-31 070501](https://github.com/jabajasphin/mobilerobot-openloopcontrol/assets/138971154/1fd39abd-51af-41cb-81e1-ce97ef0cdc22)




## MobileRobot Movement Video:
]My Robo Master Youtube:

https://youtu.be/xwhEB91rVo0?si=U6PpVHDyiMMAfGFf



## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```

