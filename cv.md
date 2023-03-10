# Drone Core Documentation

## CV-Node
This is a Template for a CV Node

Subscribe to:
- Manual Controller Packets

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
