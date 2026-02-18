# ROS2 Humble Installation Guide

## Overview
This repository explains the complete step-by-step process of installing:

- VirtualBox
- Ubuntu 22.04
- ROS2 Humble
- Running the Turtlesim package

---

# Step 1: Install VirtualBox

1. Download VirtualBox from:
   https://www.virtualbox.org/wiki/Downloads

2. Install VirtualBox on your system (Windows / macOS).

---

# Step 2: Install Ubuntu 22.04

1. Download Ubuntu 22.04 Desktop (Jammy):

   https://releases.ubuntu.com/jammy/
   OR
   https://cdimages.ubuntu.com/ubuntu-mate/releases/22.04/release/

2. Open VirtualBox.
3. Create a New Virtual Machine.
4. Select:
   - Type: Linux
   - Version: Ubuntu (64-bit)
5. Allocate RAM (recommended: 4GB or more).
6. Create a virtual hard disk (recommended: 20GB or more).
7. Attach the Ubuntu ISO file.
8. Start the VM and complete Ubuntu installation.
9. Install Guest Additions (optional but recommended).

---

# Step 3: Install ROS2 Humble

Make sure you are using Ubuntu 22.04.

1. Update system:
   sudo apt update && sudo apt upgrade

2. Follow official installation guide:
   https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debs.html

3. Install ROS2 Humble Desktop:
   sudo apt install ros-humble-desktop

4. Source ROS:
   source /opt/ros/humble/setup.bash

(Optional) Add to .bashrc:
   echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc

---

# Step 4: Install and Run Turtlesim

1. Install turtlesim:
   sudo apt install ros-humble-turtlesim

2. Run turtlesim node:
   ros2 run turtlesim turtlesim_node

3. Open another terminal and run:
   ros2 run turtlesim turtle_teleop_key

Now you can control the turtle using keyboard arrows.

---

# Task Explanation

The task required:

- Installing VirtualBox.
- Installing Ubuntu 22.04.
- Installing ROS2 Humble.
- Running the Turtlesim package.

All steps were successfully completed and documented in this repository.

---

# 👤 Author
Completed as part of ROS2 training and learning practice.
