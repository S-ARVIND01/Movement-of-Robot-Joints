# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)
```
## Output
### 1. Generic Articulated Robot
![280908574-641708ce-1843-442e-ab31-01c623f32d72](https://github.com/S-ARVIND01/Movement-of-Robot-Joints/assets/118707337/41504bb7-8726-4a0a-af99-2b639434eefc)

### 2. robot.driveJoints(0,0,0,0,0,0)
![280908667-82256cc0-90e4-4236-a0d7-a75b1ac7f541](https://github.com/S-ARVIND01/Movement-of-Robot-Joints/assets/118707337/8c4169e2-28ef-4d1d-9ba8-7fca7e2c12f7)

### 3. Movement of Joint1
![280908705-56c52411-eda5-4e2d-a6f7-8e415ce768a3](https://github.com/S-ARVIND01/Movement-of-Robot-Joints/assets/118707337/4e61b332-7ba4-4f80-b0ec-e59d217539eb)

### 3. Movement of Joint2
![280908761-5e8560b7-066e-4d8a-9cda-b2b385bbc7ce](https://github.com/S-ARVIND01/Movement-of-Robot-Joints/assets/118707337/da0b4577-9004-4111-9053-3baf1fff92dc)

### 3. Movement of Joint3
![280908869-0397a671-9f98-4145-8939-1776e32f1efb](https://github.com/S-ARVIND01/Movement-of-Robot-Joints/assets/118707337/20ac24ae-ddf0-472e-9ccc-eaa69cf89b95)

## Result 
Thus the different robots joints are moved with the help of python list.


