This file describes all nodes and launchfiles used within the package homework4, as well as any expected results. 

Note: I included a .rosinstall file because I made some minor, but important, changes to the darknet_ros package. Changes I made are listed in the sections below. 

**Launch Files**
web.launch: This is the launch file created for the Image Processing section of homework4 4. This launch file contains the node for the linux webcam, rviz, and the yolo_v3 launch file. The yolo_v3 launch file was also changed within the darknet_ros package because the default camera needed to be adjusted. Running this launch file will launch rviz and a pop up window from rviz, which will display images from the webcam along with object detection/labeling from the yolo_v3 launch file.

command to launch: roslaunch homework4 turtlebot3_load.launch 

 Screenshot of example image when running this launch file:
 ![YOLO Image](YOLO1)
 
 turtlebot3_load.launch: Loads turtlebot3 in the house environment, loads rviz and visualizes it's laser scan, starts a teleoperation node, and gmapping. This launch file is comprised of embedded launch files within the turtlebot3 packages. In addition to the packages, the slam gmapping was installed on the system prior to launching file. 
 
 command to launch this launch file: roslaunch homework4 turtlebot3_load.launch slam_methods:=gmapping

Robot was manually driven to gmap the map using the following commands:
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch

turtlebot3_localize.launch: Launch file is derived from the turtlebot3_navigation launch file, which loads rviz, the map server, amcl, move_base launch file, and turtlebot3 burger robot. The amcl is resonsible for localizing the robot and the move_base launch file part of the move_base package responsible for moving the turtlebot3 to a goal via pose messages. 

Command to run this:




