
#  FactoryRobot

## Section 1: Introduction
This project details the deployment of an end-to-end autonomous robot utilizing an autonomous software stack. The system architecture features an onboard computer serving as the central processing unit for the autonomous functionalities. Communication are facilitated through a Controller Area Network (CAN) bus cable which is further connected to the motor ,forming a complete autonomous robotic system. We have to intoduce a CAN to ROS interface because the signals(steering angle, velocity) are CAN messages that  we send to the Robot, and the robot understands it only in ROS framework.

### Section 2: Prerequisite


* **Sensor Integration:** The robot utilizes a Velodyne Lidar sensor for environmental perception. Proper integration necessitates configuring the Lidar's IP address to be compatible with the robot's onboard computer's network settings.

* **Map Making:** The autonomous navigation of the robot depends on specific map data files:
    * **Lanelet Map (lanelet.osm):** This file provides semantic information about the environment, including lane structures and traffic regulations. Further details are available in point 2 of the project's readme file.
    * **Point Cloud Map (pcd):** This file contains a 3D point cloud representation of the environment's geometry. Further details are available in point 2 of the project's readme file.

