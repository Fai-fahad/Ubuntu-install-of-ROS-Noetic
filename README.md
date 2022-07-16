# Ubuntu-install-of-ROS-Noetic
Download steps
# Downloads - Oracle VM VirtualBox
from this link:https://www.virtualbox.org/wiki/Downloads 
# Download Ubuntu
from this link:https://ubuntu.com/download#download
# Open Ubuntu
from  the new button
![Capture1](https://user-images.githubusercontent.com/101976302/179356444-9670ecc7-e5ef-49d9-a616-78bae1653f78.PNG)
We create  Virtual Machine
1.Add the Name like(Ubunto)
2.Select the Machine Folder
3.Select the type and version 
![Capture2](https://user-images.githubusercontent.com/101976302/179356659-b13bc13a-3a2f-4eb6-9812-2d957564fe34.PNG)
from start button we start ower Machine ! 
# Ubuntu install of ROS Noetic
Open  Terminal Ubuntu
# 1.Setup your sources.list
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
# 2.Set up your keys
sudo apt install curl # if you haven't already installed curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
# 3.Installation
sudo apt update
sudo apt install ros-noetic-desktop-full
sudo apt install ros-noetic-desktop
sudo apt install ros-noetic-ros-base
sudo apt install ros-noetic-PACKAGE
sudo apt install ros-noetic-slam-gmapping
apt search ros-noetic
# 4.Environment setup
source /opt/ros/noetic/setup.bash
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
echo "source /opt/ros/noetic/setup.zsh" >> ~/.zshrc
source ~/.zshrc
# 5.Dependencies for building packages
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
sudo apt install python3-rosdep
sudo rosdep init
rosdep update
# The End 
To follow the steps and explain them in detail, click on this link:
http://wiki.ros.org/noetic/Installation/Ubuntu
 



