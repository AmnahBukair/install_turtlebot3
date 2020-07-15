# Pre_installation
intall ubuntu 16.04 and ROS Kinetic  

## Create a workspace 
cd Documents  
mkdir turtle_ws    
cd turtle_ws   
mkdie src   
cd src  
catkin_init_workspace  
cd ..    
catkin_make  

## Install the TurtleBot3 simulator

Open a terminal window and install the dependent packages. Enter the following commands, one right after the other:

cd ~/catkin_ws/src/  
git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git  
git clone https://github.com/ROBOTIS-GIT/turtlebot3.git  
cd ~/catkin_ws && catkin_make  

* TurtleBot3 has three models, Burger, Waffle, and Waffle Pi, so you have to set which model you want to use before you launch TurtleBot3. Type this command to open the bashrc file to add this setting:  

gedit ~/.bashrc  
Add this line at the bottom of the file:  

export TURTLEBOT3_MODEL=burger  
Save the file and close it.  

Now reload .bashrc so that you do not have to log out and log back in.  

source ~/.bashrc  


## Refrences:
https://www.udemy.com/course/ros-basics-program-robots/learn/lecture/8892582#overview  
https://automaticaddison.com/how-to-launch-the-turtlebot3-simulation-with-ros/#gazebo  
