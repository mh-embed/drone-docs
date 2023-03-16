# Drone Core Documentation


## Control-Node
This is the Master Control Node

Subscribe to:
- Manual Controller Packets
    - man-controller/left_x
    - man-controller/left_y
    - man-controller/right_x
    - man-controller/right_y
- CV Controller Packets
    - cv-controller/roll
    - cv-controller/pitch
    - cv-controller/yaw
- Controller Selector Bit
    - man-controller/selector

Publish to:
- Drone Control
    - drone-control/roll
    - drone-control/pitch
    - drone-control/yaw
- CV Program Selector Bit
    - drone-control/cv_id

Requirements
- std_msgs
- roscpp


## [MC-In](https://github.com/mh-embed/drone-flight-controller-node)
This is the Manual Controller In Node. This node reads controller input from UART and publishes them as-is.

Subscribe to:
- N/A

Publish to:
- Manual Controller Packets
    - man-controller/left_x
    - man-controller/left_y
    - man-controller/right_x
    - man-controller/right_y

Requirements
- rosserial
- std_msgs
- roscpp


## [FC-Out](https://github.com/mh-embed/drone-flight-controller-node)
This is the Flight Controller Out Node. This node takes messages published by the control node and sends them to the flight controller. 

Subscribe to:
- Drone Control
    - drone-control/roll
    - drone-control/pitch
    - drone-control/yaw

Publish to:
- N/A

Requirements
- rosserial
- std_msgs
- roscpp



## CV-Watchdog
This is the CV Watchdog/Manager Node. 

Subscribe to:
- TBD

Publish to:
- TBD

Requirements
- TBD
