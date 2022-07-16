Welcome to the task1-Ros-Installation-In-Ubunto wiki!

>**1. Setup your sources.list**
> > sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

>**2. Set up your keys**
> > sudo apt install curl
> > curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

>**3. Installation (Desktop-Full Install)**
> > sudo apt update
> > sudo apt install ros-noetic-desktop-full

> **4. Environment setup**
> > echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
> > source ~/.bashrc

> **5. Dependencies for building packages**
> > sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

> **6. Initialize rosdep**
> > sudo apt install python3-rosdep
> > sudo rosdep init
> > rosdep update

> **Managing Your Environment (check is to ensure that environment variables are set)**
> > printenv | grep ROS

> **Create a ROS Workspace**
> > mkdir -p ~/catkin_ws/src
> > cd ~/catkin_ws/
> > catkin_make
