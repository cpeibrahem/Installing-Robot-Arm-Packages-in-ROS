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




