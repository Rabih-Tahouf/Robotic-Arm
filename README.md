# Robotic-Arm

Program the industrial robot (Mitsubishi MELFA RV-2AJ) to perform a simple industrial task.  
Video Demonstration: https://drive.google.com/file/d/1ESsd7e1LMePoNf8_xQvZqT_W42ccoyQs/view?usp=sharing

# About the robotic arm:

The RV-2AJ 5-axis robot assembly has the robot arm, sensors, the controller, manuals, power/signal cables, and the teach pendant.  This robot is compact with high accuracy and precision. Furthermore, its repeatability is about ±0.02mm, and it features open network capability.  The RV-2AJ is compatible with MoveMaster that uses MELFA-BASIC IV and MoveMaster language as standard robot programming languages (MoveMaster Command). 

# Program Aim:

The aim of this project, was to mimic an industrial function done by an industrial robot in a real factory. The function chosen, was for the robot to pick a part place it in a certain orientation, then take it and place it in a specific location, drop it, check if its faulty or not. Here, the fault was taken to be if the part came without a cap or a cover, after checking if it’s faulty or not it takes to the production line if it’s not faulty and if it’s faulty it takes back to a storage area. This is a common task done by industrial robots in many present factories, which was one of the reasons this task was chosen. 

The robot is firstly programmed to wait for an object to come on the conveyer, it picks the object, puts it on a light sensor that detects the openings at the bottom of the object, and change the orientation as desired after that.  After placing the object in the pocketed area that has a pin, the height of the object is checked by the light sensor that is placed on the side of the end effector, in order to determine whether the object has a cover on top of it or no. Finally, an “if-statement” is used to put the piece in the correct place based on the previous condition; “covered” or “uncovered”.  This step could be continued if the application was real; for example, the “uncovered” pieces can be covered in further steps and vice versa.

# Program Procedure:

1. The robot and the computer are turned on.
2. The software is launched “Circos”
3. A small code is generated to test the logic 
4. The code is downloaded to the robot
5. The undefined positions in the code are specified after switching the robot to the teaching mode. In the teaching mode, the robot is no longer controlled by the computer, it is controlled manually by the teach pendant, in order to specify the position and orientation of each point in the computer.
6. The taught positions and orientations are uploaded back to the computer. Now, the code in the computer can be understood by the robot, and it will do the required task.
7. The program is run to check if everything is going as desired.
8. The steps 3 to 7 are repeated until the code is finished.

# Program logic:

![alt text](https://github.com/Rabih-Tahouf/Robotic-Arm/blob/main/Program%20Architecture.jpg)

