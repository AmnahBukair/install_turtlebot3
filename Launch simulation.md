TurtleBot3 supports development environment that can be programmed and developed with a virtual robot in the simulation. There are two development environments to do this, one is using fake node and 3D visualization tool RViz and the other is using the 3D robot simulator Gazebo.  

The fake node method is suitable for testing with the robot model and movement, but it can not use sensors. as i need to test SLAM and Navigation, i am going to use Gazebo, which can use sensors such as IMU, LDS, and camera in the simulation.  
 
## Install Gazebo :Default installation  
* one-liner Install  
  curl -sSL http://get.gazebosim.org | sh  
* Run  
  gazebo  
  
## Install gazebo_ros_pkgs
sudo apt-get install ros-kinetic-gazebo-ros-pkgs ros-kinetic-gazebo-ros-control

## TurtleBot3 World
TurtleBot3 world is a map consists of simple objects that makes up the shape of TurtleBot3 symbol. TurtleBot3 world is mainly used for testing such as SLAM and Navigation.  
inside workspace:  
$ source devel/setup.bash  
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch  

Then the simulation was launched [click here](https://github.com/AmnahBukair/install_turtlebot3/blob/master/launch%20Turtlebot%20World.png)


## Refrences:
https://emanual.robotis.com/docs/en/platform/turtlebot3/simulation/#turtlebot3-simulation-using-fake-node  
http://gazebosim.org/tutorials?tut=ros_installing&cat=connect_ros  
