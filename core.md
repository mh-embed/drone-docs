# Drone Core Documentation


## [Control-Node](https://github.com/mh-embed/drone-core)
This is the Master Control Node

Subscribe to:
- Manual Controller Packets 
    - man_control/left_x    [Man means manual, not male :) ]
    - man_control/left_y
    - man_control/right_x
    - man_control/right_y
- CV Controller Packets
    - cv_control/roll
    - cv_control/pitch
    - cv_control/yaw
- Controller Selector Bit
    - man_control/selector

Publish to:
- Drone Control
    - drone_control/roll
    - drone_control/pitch
    - drone_control/yaw
- CV Program Selector Bit
    - cv_manager/selector

Requirements
- std_msgs
- roscpp


## [Flight Controller Node](https://github.com/mh-embed/drone-flight-controller-node)
This is the Manual Controller Receiver and Flight Controller Out Node. This node reads controller input from UART and publishes them as-is.

Subscribe to:
- Drone Control
    - drone_control/roll
    - drone_control/pitch
    - drone_control/yaw

Publish to:
- Manual Controller Packets
    - man_control/left_x
    - man_control/left_y
    - man_control/right_x
    - man_control/right_y

Requirements
- rosserial
- std_msgs
- roscpp


## [CV-Watchdog](https://github.com/mh-embed/drone-cv-watchdog)
This is the CV Watchdog/Manager Node. 

Subscribe to:
- cv_manager/selector

Publish to:
- cv_selector/<CV_UID>  (for each CV_UID registered)

Requirements
- roscpp
- rospy     (Prototyping Stage)
