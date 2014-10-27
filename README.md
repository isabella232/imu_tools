IMU tools for ROS
===================================

Overview
-----------------------------------

Fork from the IMU_Tools branch. The original repo has been stripped to contain only imu_filter_madgwick. This is to provide convenience when building bitbake recipes.

 * `imu_filter_madgwick`: a filter which fuses angular velocities,
accelerations, and (optionally) magnetic readings from a generic IMU 
device into an orientation. Based on the work of [1].

Installing
-----------------------------------

### From source ###

[Create a catkin workspace](http://wiki.ros.org/catkin/Tutorials/create_a_workspace)
(e.g., `~/ros-hydro-ws/`) and source the `devel/setup.bash` file.

Make sure you have git installed:

    sudo apt-get install git-core

Download the stack from our repository into your catkin workspace (e.g.,
`ros-hydro-ws/src`; use the proper branch for your distro, e.g., `groovy`,
`hydro`...):

    git clone -b <distro> https://github.com/ccny-ros-pkg/imu_tools.git

Install any dependencies using [rosdep](http://www.ros.org/wiki/rosdep).

    rosdep install imu_tools

Compile the stack:

    cd ~/ros-hydro-ws
    catkin_make

More info
-----------------------------------

http://wiki.ros.org/imu_tools

License
-----------------------------------

 * `imu_filter_madgwick`: currently licensed as GPL, following the original implementation

 * `rviz_imu_plugin`: BSD

References
-----------------------------------
 [1] http://www.x-io.co.uk/open-source-imu-and-ahrs-algorithms/
