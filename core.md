# Drone Core Documentation

## Table of Contents


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

Requirements
- std_msgs
- roscpp


## FC-Out
This is the Flight Controller Out Node

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