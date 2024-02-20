## Create and Compiling the package

mkdir -p assignment_ws/src
cd assignment_ws/src
<---- Copy & paste the pacakges here --->
catkin_make


## Enabling webcam using ros script
Terminal 1: Running ROS master
cd assignment_ws
roscore

Terminal 2: Launching webcam
cd assignment_ws
source devel/setup.bash
rosrun webcam_pkg webcam.py

Terminal 3: Visualizing webcam images
cd assignment_ws
source devel/setup.bash
rosrun image_view image_view image:=/camera/image_raw


## Launch YOLO V2 model
cd assignment_ws
source devel/setup.bash
roslaunch yolo_v2_ros assignment.launch



