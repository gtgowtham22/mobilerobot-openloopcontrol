# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

 

1. **Initialization**:
   - Establish connection with the RoboMaster EP robot
   - Get access to the chassis control module

2. **Movement Definition**:
   - Created a list of movement commands with parameters for:
     - x: forward/backward speed (m/s)
     - y: left/right speed (m/s)
     - z: rotation speed (deg/s)
     - time: duration of movement (seconds)

3. **Movement Execution**:
   - Loop through each movement command
   - Set the specified speeds using `drive_speed()`
   - Maintain the movement for the specified duration
   - Briefly stop between movements for cleaner transitions

4. **Cleanup**:
   - Ensure robot stops completely
   - Close the connection properly

## Program
```python
from robomaster import robot
import time

if __name__ == '__main__':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis

    ## Write your code here



    
    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

Insert image here


<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
