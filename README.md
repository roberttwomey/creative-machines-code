# Code for Creative Machines 2023
course website [cm.roberttwomey.com](http://cm.roberttwomey.com)

- [xArm Howto](#xarm-howto)
- [Tools and End Effectors](#tools)
- [Reference Drawings](#reference-drawings)
- [Python Code](#python-code)

## xArm Howto

- Install xArm software - download here [https://www.ufactory.cc/ufactory-studio/](https://www.ufactory.cc/ufactory-studio/)
- [Setup networking to communicate with xArm](howto/networking.md)
- Blockly basics xArm
- [Interactive Posing the xArm](howto/posing-xarm.md)

## Tools
Mounting tools and custom attachments to the robot.

### Custom End Effector
Follow the tutorial on: [Designing / 3D printing a custom end effector](howto/endeffector.md)

<img width="290" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/d9ee51bc-7101-486e-aa5f-d9e738194aba"><br>
[endeffector_plate_xarm5.3dm](../solids/endeffector_plate_xarm5.3dm)

### Camera Mount
- razer kiyo pro mount: [xarm_razer_holder.3dm](solids/xarm_razer_holder.3dm)
- general purpose (1/4") mount: [xarm7_toolhead.3dm](solids/xarm7_toolhead.3dm)

## Reference Drawings

### Toolhead Reference Drawing
xArm 5 LITE robot tool head (mm)<br>
<img width="524" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/433d86c3-ca2b-4b8f-8ffd-997ebab2d948"> 

### Table Mount Reference Drawing
robot base (mm)<br>
<img width="400" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/39075fb5-83c4-4c2c-af09-7e594b9c4cbd"> 

### CAD Models
xArm5 3D file<br>
<img width="400" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/d234b71b-06d4-445d-9501-6a8d30f53e9a">
[https://www.ufactory.cc/wp-content/uploads/2023/04/xArm5XF1300.zip](https://www.ufactory.cc/wp-content/uploads/2023/04/xArm5XF1300.zip)

xArm7 3D file<br>
[xArm7-3D-File-20190521.3dm](solids/xArm7-3D-File-20190521.3dm)

## Python Code
- [xArm Python SDK](https://github.com/xArm-Developer/xArm-Python-SDK)
- [Setup Python development environment for xArm](howto/python-setup)

### xArm5 python code samples: 
- [go-home_xarm5.py](xarm5-python/go-home_xarm5.py)
- [go-stretchout_xarm5.py](xarm5-python/go-stretchout_xarm5.py)
- [go-frontBack_xarm5.py](xarm5-python/go-frontBack_xarm5.py)
- [go-frontForward_xarm5.py](xarm5-python/go-frontForward_xarm5.py)

### xArm7 python code samples: 
- [go-home.py](xarm7-python/go-home.py)
- [go-stretchout.py](xarm7-python/go-stretchout.py)
- [go-corners-ikfast.py](xarm7-python/go-corners-ikfast.py)
- [look-forward-ikfast.py](xarm7-python/look-forward-ikfast.py)
- [face-ikfast.py](xarm7-python/face-ikfast.py) (requires opencv)

# Reference
- xArm User Manual: ([download](http://download.ufactory.cc/xarm/en/xArm%20User%20Manual.pdf))
- [xArm Python SDK](https://github.com/xArm-Developer/xArm-Python-SDK)
- [xArm CPP SDK](https://github.com/xArm-Developer/xArm-CPLUS-SDK)
- [xArm ROS](https://github.com/xArm-Developer/xarm_ros)
- [xArm ROS2](https://github.com/xArm-Developer/xarm_ros2)
