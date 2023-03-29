# Drone Core Documentation

## CV-Node
This is the requirements for a CV Node

Subscribe to:
- CV Program Selector Bit
    - cv_selector/<UID>

Publish to:
- CV Controller Packets
    - cv_roll/<UID>
    - cv_pitch/<UID>
    - cv_yaw/<UID>

Requirements
- std_msgs
- rospy
- opencv (cv2)
    
### Make Your Custom CV Node
    To build your own CV node, follow instructions documented in the [Template](https://github.com/mh-embed/drone-cv-template)
