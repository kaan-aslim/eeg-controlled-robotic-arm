# EEG-Based Control of a 3-Axis Robotic Arm

##  Overview

This project presents the end-to-end design and implementation of a mechatronic system where a 3-axis robotic arm is controlled using EEG (brainwave) signals.

The objective is to demonstrate the feasibility of Brain-Computer Interface (BCI) applications in industrial systems, beyond medical prosthetics.

The system enables a user to generate movement commands through mental states, which are processed and classified to control a robotic arm in real time.

---

##  Objectives

* Design and build a 3-axis robotic arm from scratch
* Develop a full mechatronic system including mechanical, electrical, and control layers
* Acquire and process EEG signals for command generation
* Classify brain signals into discrete robot control actions
* Demonstrate BCI-based control for industrial applications

---

##  System Architecture

The system consists of four main layers:

1. **Mechanical System**

   * Custom-designed 3-axis robotic arm
   * Gear transmission system (custom gear ratios)
   * Structural validation via FEA

2. **Electrical System**

   * Stepper motors and motor drivers
   * Power supply and protection systems (relay, E-stop)
   * PLC-based control infrastructure

3. **Control System**

   * PLC (Siemens S7-1200) with TIA Portal
   * Ladder logic & function block programming
   * HMI interface via WinCC for manual control

4. **EEG & Machine Learning**

   * EEG data acquisition using NeuroSky MindWave Mobile 1
   * Dataset creation from mental commands
   * Signal processing (FFT, Wavelet Transform experiments)
   * Classification using:

     * K-Nearest Neighbors (KNN)
     * Decision Tree

---

##  Technologies Used

* SolidWorks (CAD design)
* ANSYS (Static Structural Analysis)
* MATLAB (Kinematics, Workspace analysis, ML)
* Siemens TIA Portal (PLC programming)
* WinCC (HMI)
* EEG acquisition (NeuroSky + EEGID)
* Machine Learning (KNN, Decision Tree)

---

##  Mechanical Design

* Full robotic arm designed from scratch in SolidWorks
* Custom gears designed instead of off-the-shelf reducers
* Manufacturing methods considered:

  * CNC machining
  * Laser cutting
  * Bending (Abkant)
* Material selection based on corrosion and mechanical properties
* Lubrication and coating applied for durability

---

##  Engineering Analysis

* Torque calculations for each joint
* Motor selection based on required torque
* Static structural analysis in ANSYS
* Design iteration based on stress & deformation results
* Workspace estimation using Monte Carlo method in MATLAB

---

##  Control System

* PLC-based control using Siemens S7-1200
* Ladder logic and function blocks for multi-axis motion control
* Motor parameters:

  * Speed
  * Direction
  * Acceleration
* HMI interface for real-time manual control

---

##  EEG & Machine Learning

* EEG signals collected for different mental commands:

  * Left / Right (base rotation)
  * Up / Down (arm joints)
  * Gripper open / close
  * Neutral state

* Dataset preparation:

  * CSV formatting
  * Labeling and segmentation

* Signal processing:

  * FFT and Wavelet Transform (evaluated)

* Classification:

  * KNN
  * Decision Tree

* Achieved classification accuracy:

  * ~80%

---

##  Results

* Successfully designed and built a functional robotic arm
* Achieved real-time manual control via PLC and HMI
* Demonstrated EEG-based command classification
* Validated feasibility of BCI-based industrial control systems

---

##  Limitations

* Real-time EEG-to-robot control integration not completed
* Limited dataset size
* Noise in EEG signals affected classification performance

---

##  What I Learned

* End-to-end mechatronic system design
* Mechanical design and manufacturing processes
* PLC-based industrial control systems
* Robot kinematics and workspace analysis
* EEG signal acquisition and preprocessing
* Machine learning basics for classification
* System-level engineering thinking

---

##  Future Work

* Real-time EEG control integration
* Improved signal processing and filtering
* Deep learning-based classification
* ROS2 integration for advanced control
* Expansion to multi-DOF robotic systems

---
