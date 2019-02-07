# Cable Joint

## Pre-requisites
- [Ubuntu 16.04](http://releases.ubuntu.com/16.04/)
- [ROS](http://www.ros.org/)
- [catkin-command-line-tools](https://catkin-tools.readthedocs.io/en/latest/)

## How to Use it
- Clone this repo to your catkin workspace (suppose yours is `ros_ws`)

``` bash
cd ros_ws/src/
git clone https://github.com/deePurrobotics/cable_joint.git
```
- Build the packages

``` bash
cd ~/ros_ws
catkin build
```
> make sure these lines appear in your `~/.bashrc` file
>
``` bash
source /opt/ros/kinetic/setup.bash
source /home/linzhank/ros_ws/devel/setup.bash

```
>
- Launch the simulation, open a new terminal

``` bash
roslaunch cable_joint_control cable_joint_empty_world.launch
```
- A demo script is located at `this_repo/cable_joint_control/scripts/applywrench_test.py`

## Notes
- ros topic shows rgb camera image: `/cable_joint/rgb_camera/image_raw`
- forces control the upper disc: `/force_northeast`, `/force_northwest`, `/force_southwest`, `force_southeast`

