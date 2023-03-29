# drone-docs
Michigan Hackers Embedded 2023 Drone project Documentation

# Development

Development Environment is configured through Docker in our [devcontainer config](https://github.com/mh-embed/.devcontainer)

# Package List
- [Drone Core](https://github.com/mh-embed/drone-core)
  - ROS requirements documented in [core.md](https://github.com/mh-embed/drone-docs/blob/main/core.md)
- [Drone Flight Controller Communicator](https://github.com/mh-embed/drone-flight-controller-node)
  - Communication with Flight Controller and Remote is documented in [technical-references.md](https://github.com/mh-embed/drone-docs/blob/main/technical-references.md)
  - ROS requirements documented in [core.md](https://github.com/mh-embed/drone-docs/blob/main/core.md)
- [Drone CV Watchdog](https://github.com/mh-embed/drone-cv-watchdog)
  - ROS requirements documented in [core.md](https://github.com/mh-embed/drone-docs/blob/main/core.md)
- [Drone CV Template](https://github.com/mh-embed/drone-cv-template)
  - ROS requirements documented in [cv.md](https://github.com/mh-embed/drone-docs/blob/main/cv.md)

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


