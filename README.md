# 5-DOF-Robotic-Arm
This repository contains the design and control software for a 5-degree-of-freedom robotic arm that I designed, modeled, and built from scratch. The mechanical structure was created entirely in SolidWorks, 3D printed, and actuated using servo motors. Control is implemented on an ESP32.

The arm is currently coordinate controlled using an analytical inverse kinematics solver. Ongoing work focuses on extending the system to vision-based control and implementing pick-and-place operations.

## Overview
- 5 DOF serial manipulator
- Designed completely in SolidWorks
- 3D printed and assembled
- ESP32-based control system

# Actuation
- 3 × MG995 servos for base yaw, base pitch, and elbow
- 2 × micro servos for wrist and gripper

# Control
- Cartesian control using X Y Z + wrist angle
- Analytical inverse kinematics (non-iterative)
- Elbow-up / elbow-down configurations
- Smooth incremental joint motion
- Safe startup (no servo movement on boot)
- Servo calibration stored persistently

#Current Work
- Coordinate control: completed
- Calibration and motion control: completed
- Vision-based control: in progress
- Pick-and-place implementation: in progress
