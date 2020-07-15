TurtleBot3 supports development environment that can be programmed and developed with a virtual robot in the simulation. There are two development environments to do this, one is using fake node and 3D visualization tool RViz and the other is using the 3D robot simulator Gazebo.  

The fake node method is suitable for testing with the robot model and movement, but it can not use sensors. as i need to test SLAM and Navigation, i am going to use Gazebo, which can use sensors such as IMU, LDS, and camera in the simulation.  
 
## install Gazebo :Default installation
* one-liner Install
  curl -sSL http://get.gazebosim.org | sh
* Run
  gazebo
  
## Install gazebo_ros_pkgs
sudo apt-get install ros-kinetic-gazebo-ros-pkgs ros-kinetic-gazebo-ros-control
