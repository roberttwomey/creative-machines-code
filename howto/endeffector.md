# How to Fabricate an End Effector for a Robot
1. [Determine your bolt pattern](#bolt-pattern)
2. [Model your part](#model-your-part)
3. [Fabricate](#fabricate) (3d print, laser cut, hand drill)
   
## Bolt Pattern

From ufactory, the measurements for the xArm 5 LITE robot tool head (mm) are here:<br>
<img width="524" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/433d86c3-ca2b-4b8f-8ffd-997ebab2d948"> 

Lets interpret those dimensions... 

The end effector plate is a circle 75mm in diameter. 

We are going to use M6 (metric) screws to attach our end effector. 

We can attach to:
- 2 M6 screw holes, 10mm deep, on a circle 63mm across (63 P.C.D. or Pitch Circle Diameter), 
located at top and bottom
- 4 M6 screw holes, 10mm deep, on a circle 50mm across
- 1 M6 screw hole, 10mm deep, on a circle 50mm across located on RH side

## Model Your Part
1. We need to make a part that has **clearance holes** that match two or more of the mounting holes above.
   - A clearance hole is wide enough to accomodate a screw of a given size, and can fit with a close fit, medium fit, or free fit.
   - According to [this Tap and Drill chart](https://littlemachineshop.com/images/gallery/PDF/tapdrillsizes.pdf):
   - M6 screw *free fit*: 6.6mm hole
2. Recreate your dimensioned drawing showing the location of the screwholes.
3. Create two **clearance holes** at the desired size (7mm), centered on those screw holes.
4. Create an exterior profile that pleasingly matches with the size of the end effector mounting point (75mm circle). Or doesn't... you
're an artist!
5. Model up your end effector. 

### End Effector Plate
<img width="290" alt="image" src="https://github.com/roberttwomey/creative-machines-code/assets/1598545/d9ee51bc-7101-486e-aa5f-d9e738194aba">
<br> [endeffector-plate-xarm5.3dm](../solids/endeffector-plate-xarm5.3dm)

### 3D Printed Plate


## Fabricate
Either (A) export your model as a **.STL** file and 3d print it, or (B) export it as a vector image (**.SVG**) and laser cut it.

## Reference
- See the camera mounts on the main page:
  - razer kiyo pro mount: [xarm_razer_holder.3dm](solids/xarm_razer_holder.3dm)
  - general purpose (1/4") mount: [xarm7_toolhead.3dm](solids/xarm7_toolhead.3dm)
- Tap and Drill Chart https://littlemachineshop.com/images/gallery/PDF/tapdrillsizes.pdf

