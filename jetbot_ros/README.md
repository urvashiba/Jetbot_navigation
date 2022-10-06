
### Install Adafruit Libraries

These Python libraries from Adafruit support the TB6612/PCA9685 motor drivers:

```bash
# pip should be installed
$ sudo apt-get install python-pip

# install Adafruit libraries
$ pip install Adafruit-MotorHAT
$ pip install Adafruit-SSD1306
```

Grant your user access to the i2c bus:

```bash
$ sudo usermod -aG i2c $USER
```

Reboot the system for the changes to take effect.

### Create catkin workspace

Create a ROS Catkin workspace to contain our ROS packages:

```bash
# create the catkin workspace
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws
$ catkin_make

# add catkin_ws path to bashrc
$ sudo sh -c 'echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc'

