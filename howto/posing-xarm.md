# Programming fixed movements with blockly and UFactory Studio

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
   - <img width="212" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/3c9619d8-0dbb-4cea-8323-9a39bd618ca1">
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

  







 
