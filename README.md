# Follow the white ball on ROS
# In this project, the goal is to follow a white ball using the images obtained from the camera on a mobile robot. 

# It consist of two steps: 
```sh
1) my_robot

  I start by designing a custom robot using the **urdf** format.
  my_robot.xacro file that defines the robot is located in "src/my_robot/urdf".
  The robot is equipped with a camera and a LIDAR. The LIDAR mesh file can be found in "src/my_robot/meshes".
  I also add a custom world design that can be downloaded from "https://github.com/zvatansever/Gazebo-office-model.git"
```
```sh
2) ball_chaser (to-do update the white ball localization from image pixels)

   We need to use the camera subscribe to publisher "/camera/rgb/image_raw" to stream the camera image. 
   Once the camera sees the white ball, it starts following it, interested reader can find implementation details in process_image.cpp
```
