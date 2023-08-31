# Programming fixed movements with blockly and UFactory Studio
- Recording joint positions (coordinates) with [Manual Movement](#manual-movement)
- Writing [Blockly Code](#blockly-code) to move between those positions.
- Code to [Move a Can](#move-a-can) from one position on the table to another.
- [Additional tips and tricks](#additional-materials)

## Manual Movement
Using manual mode in UFactory studio to record joint (and gripper) positions with the xArm,
then using those positions to create motion programs with blockly.

1. Turn on the control box and wait for it to boot and assign IP address (double beep after 30 seconds).
2. Connect to the xArm in UFactory Studio.
3. Once connected, "Enable Robot"
   - <img width="286" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/db51daf4-c6ed-4987-99ee-8a6e299c7ecc">
5. Click "Live Control"
   - <img width="212" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/f90ee0ec-061e-4ad9-80ae-cb596aab76f6">
6. Hold "Zero Position" button to return to home position, if it is not already there.
   - [image]
7. Press "Manual Mode" to enable manual posing:
   - <img width="147" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/73b77583-ff89-4f35-8bb1-58d8b8317d27"> <img width="155" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/02505694-1f47-4fba-bb86-7db9f669ee81">
8. Move the robot to your desired first position, and click the clipboard icon to copy the joint positions. Save those in a local file:
   - <img width="366" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/d0cfdaa3-8a3b-4da9-a8e5-18b1b0d1ecab">
   - NOTE: if connected, the gripper will have to be posed manually using the slider. Note the gripper position.
   - <img width="365" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/cfd49a10-0f8a-4750-8e8c-63ed49e2dbc9">
9. Save those joint positions in a local file:
   - `[-60.9,49.0,-11.9,46.4,110.1,93.7,0.5]`
   - together with gripper position, if necessary: `649`
10. Repeat steps 7-8 until you have saved all of your robot positions.
11. Write the blockly code.

## Blockly Code
1. Select Blockly from the main menu
   - <img width="208" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/6fa5b153-4255-4a5a-a4f8-d0916093d381">
2. Create a new file and give it a descriptive name:
   - <img width="46" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/6bbbfb78-41c9-4f85-ae5d-a3f3254767e7">
   - **can_gripper_demo**
3. Add block for starting settings.
   - [move joint]
   - [sleep]
   - [set gripper]
   - [zero position]
4. Set the gripper to your initial position at default speed:
   - [set gripper]: use `650` for **Pos**. 
5. Move to your first position at the default speed:
   - [move joint]: use these coordinates `[-60.9,49.0,-11.9,46.4,110.1,93.7,0.5]` for J1-J7
6. Pause if you want:
   - [sleep] `1` second.     
7. Repeat steps 4-6 to move through any additional positions, rotate joints, etc. Adding pauses where you want them.
   - **NOTE**: Be sure to add entry and exit points. I will explain this in class.

## Move a Can
Here is code I wrote to pick up a can and move it to another position:

<img width="636" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/6e3a69f6-557c-4552-a763-a75787a4e146">

[blockly-can_gripper_demo.tar.gz](blockly-can_gripper_demo.tar.gz)

This took about 1 hour.

## Additional Materials
- [JointSpeed]
