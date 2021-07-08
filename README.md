# rclshark-smi:turtle::shark:

Doing recursive clone from [rclshark](https://github.com/Ar-Ray-code/rclshark) is recommended

You can use rclshark to check the hardware status of multiple computers. You don't even need to bother opening htop. Good for you! :blush:

IP addresses are sorted in ascending order and are dynamically added and removed. See Usage 2 for installing rclshark-smi. If you want to use only rclshark-smi, type `sudo systemctl disable rclshark.service`. to use only rclshark-smi.

![rclshark-smi-docker](https://raw.githubusercontent.com/Ar-Ray-code/rclshark/main/images_for_readme/rclshark-smi-docker.png)

## Install & RUN

```bash
$ source /opt/ros/foxy/setup.bash
$ git clone https://github.com/Ar-Ray-code/rclshark-smi.git ~/ros2_ws/src
$ git clone https://github.com/Ar-Ray-code/computer_msgs.git ~/ros2_ws/src
$ cd ~/ros2_ws/ && colcon build --symlink-install
$ source ~/ros2_ws/install/setup.bash
$ ros2 run rclshark-smi rclshark_smi.py
```
