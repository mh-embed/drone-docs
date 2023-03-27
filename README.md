# drone-docs
Michigan Hackers Embedded 2023 Drone project Documentation

# ROS
We are using ROS noetic for this drone. To learn more about [ROS](https://www.ros.org/), follow the [ROS tutorials](http://wiki.ros.org/ROS/Tutorials) to learn about these topics:

Development:
- ROS filesystem / Catkin workspace
- ROS packages
- bag files / logging

Programs:
- Node
- Topic
  - stdmsg and other messages pack
- Service
- roscpp
- rospy
- Launch files

Commands:
- roscore
- rosrun
- rostopic

# Development

Development Environment is configured through Docker in our [devcontainer config](https://github.com/mh-embed/.devcontainer)

# Package List
- [Drone Core](https://github.com/mh-embed/drone-core)
  - ROS requirements documented in [core.md](https://github.com/mh-embed/drone-docs/blob/main/core.md)
- [Drone Flight Controller Communicator](https://github.com/mh-embed/drone-flight-controller-node)
- [Drone CV Watchdog](https://github.com/mh-embed/drone-cv-watchdog)
- [Drone CV Template](https://github.com/mh-embed/drone-cv-template)
