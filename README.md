# Code for Creative Machines 2023
course website [cm.roberttwomey.com](http://cm.roberttwomey.com)

- [xArm Howto](#xarm-howto)
- [Tools](#tools)
- [Python Code](#python-code)

## xArm Howto

- Install xArm software - download here [https://www.ufactory.cc/ufactory-studio/](https://www.ufactory.cc/ufactory-studio/)
- [Setup networking to communicate with xArm](howto/networking.md)
- Blockly basics xArm
- [Interactive Posing the xArm](howto/posing-xarm.md)

## Tools
Mounting things to the toolhead

- [Designing / 3D printing a custom tool]
- Camera Mount
  - razer kiyo pro mount: [xarm_razer_holder.3dm](solids/xarm_razer_holder.3dm)
  - general purpose (1/4") mount: [xarm7_toolhead.3dm](solids/xarm7_toolhead.3dm)
- 3D model of arm: [xArm7-3D-File-20190521.3dm](solids/xArm7-3D-File-20190521.3dm)


### Reference Drawings
### Toolhead Reference Drawing
robot tool head (mm)
<img width="524" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/433d86c3-ca2b-4b8f-8ffd-997ebab2d948"> 




### Table Mount Reference Drawing
robot base (mm)
<img width="250" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/39075fb5-83c4-4c2c-af09-7e594b9c4cbd"> 

## Python Code
- [xArm Python SDK](https://github.com/xArm-Developer/xArm-Python-SDK)
- [Setup Python development environment for xArm](howto/python-setup)

Python code samples: 
- [go-home.py](xarm-python/go-home.py)
- [go-stretchout.py](xarm-python/go-stretchout.py)
- [go-corners-ikfast.py](xarm-python/go-corners-ikfast.py)
- [look-forward-ikfast.py](xarm-python/look-forward-ikfast.py)
- [face-ikfast.py](xarm-python/face-ikfast.py) (requires opencv)

# Reference
- xArm User Manual: ([download](http://download.ufactory.cc/xarm/en/xArm%20User%20Manual.pdf))
- [xArm Python SDK](https://github.com/xArm-Developer/xArm-Python-SDK)
- [xArm CPP SDK](https://github.com/xArm-Developer/xArm-CPLUS-SDK)
- [xArm ROS](https://github.com/xArm-Developer/xarm_ros)
- [xArm ROS2](https://github.com/xArm-Developer/xarm_ros2)
