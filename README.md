This file describes all nodes and launchfiles used within the package homework4, as well as any expected results. 

Note: I included a .rosinstall file because I made some minor, but important, changes to the darknet_ros package. Changes I made are listed in the sections below. 

**Launch Files**
web.launch: This is the launch file created for the Image Processing section of homework4 4. This launch file contains the node for the linux webcam, rviz, and the yolo_v3 launch file. The yolo_v3 launch file was also changed within the darknet_ros package because the default camera needed to be adjusted. Running this launch file will launch rviz and a pop up window from rviz, which will display images from the webcam along with object detection/labeling from the yolo_v3 launch file.

 Screenshot of example image when running this launch file:
 ![YOLO Image](YOLO1)
