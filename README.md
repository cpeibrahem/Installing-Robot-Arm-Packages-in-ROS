### Installing Robot Arm Packages in ROS
## Steps of installing robot arm packages in Robot Operating System (ROS):
# Step-1: Open Oracle VM VirtualBox

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/01.PNG?raw=true)

# Step-2:Open Ubuntu 


![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/02.PNG?raw=true)

# Step-3: Install ROS Melodic packages with the following steps:

### `sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`


![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/02.PNG?raw=true)

###   `sudo apt install curl`


![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/03.PNG)


### `  curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add - `


![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/04.PNG)

### `  sudo apt update`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/05.PNG)

### `  sudo apt install ros-melodic-desktop-full`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/06.PNG)
![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/07.PNG)

### `  echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc`


![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/08.PNG)

### `  source ~/.bashrc`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/09.PNG)

### `  sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/10.PNG)
![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/11.PNG)


### `  sudo apt install python-rosdep`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/12.PNG)

### `  sudo rosdep init`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/13.PNG)


### `  rosdep update`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/14.PNG)


### `  source /opt/ros/melodic/setup.bash`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/15.PNG)

### `  mkdir -p ~/catkin_ws/src`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/16.PNG)

### `  cd ~/catkin_ws/`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/17.PNG)


### `  catkin_make`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/18.PNG)


### `  echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc`
![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/19.PNG)
![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/20.PNG)

### `  source ~/.bashrc`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/21.PNG)


### `  cd ~/catkin_ws/src`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/22.PNG)


### `  sudo apt install git`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/23.PNG)


### `git clone https://github.com/smart-methods/arduino_robot_arm `

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/24.PNG)


### `cd ~/catkin_ws`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/25.PNG)


### `  rosdep install --from-paths src --ignore-src -r -y`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/26.PNG)

### `  sudo apt-get install ros-melodic-moveit`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/27.PNG)


### `  sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/28.PNG)


### `  sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/29.PNG)


### `  sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control `

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/30.PNG)


### `catkin_make`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/31.PNG)

###  ` roslaunch robot_arm_pkg check_motors.launch`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/32.PNG)



### `rqt_graph`

![](https://github.com/cpeibrahem/Installing-Robot-Arm-Packages-in-ROS/blob/main/image/33.PNG)
