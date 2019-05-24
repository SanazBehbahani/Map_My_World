# Map_My_World

Create a 2D occupancy grid and 3D octomap from a simulated environment using a robot with the RTAB-Map package.

## Project Flow

The project flow will be as follows:

1. A package is developed to interface with the rtabmap_ros package.

2. Where_Am_I (https://github.com/SanazBehbahani/Where_Am_I.git) will be used as the base. 
Changes are made to interface it with RTAB-Map (e.g. adding an RGB-D camera).

3. Ensure that all files are in the appropriate places, all links are properly connected, naming is properly setup and topics are correctly mapped. 
Furthermore, the appropriate launch files are created to launch the robot and map its surrounding environment.

4. After launching the robot, teleop around the room to generate a proper map of the environment.

## RTAB-Map Pacakge

According to the documentation, the recommended robot configuration requires:

- A 2D Laser, providing sensor_msgs/LaserScan messages
- Odometry sensors, providing nav_msgs/Odometry messages
- 3D Camera, compatible with openni_launch, openni2_launch or freenect_launch ROS packages

I use a simulated Kinect camera for RTAB-Map.

 ## Visualization
 
 Example of database visualized through RTAB-Map's database viewer.
 
 ![Capture](https://user-images.githubusercontent.com/7389485/58361084-0e55f880-7e41-11e9-8a93-9a918ffcba7e.JPG)

## Link to Rtabmap database in my Google Drive 

https://drive.google.com/open?id=1KvL0CzVFU8shR1xh9HuEGlmED5dxrq9p
