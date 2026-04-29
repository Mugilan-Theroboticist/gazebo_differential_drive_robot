# 🤖 Gazebo Differential Drive Robot (ROS 2)

A ROS 2-based differential drive robot simulated in Gazebo, with keyboard teleoperation support. This project demonstrates robot modeling, simulation, and basic control using ROS 2 Jazzy and Gazebo Harmonic.


---

## ⚙️ Requirements

* Ubuntu 24.04
* ROS 2 Jazzy Jalisco
* Gazebo Harmonic

---

## 📦 Dependencies

Install the required ROS 2 packages:

```bash
sudo apt install -y \
    ros-jazzy-ros-gz \
    ros-jazzy-ros-gz-bridge \
    ros-jazzy-joint-state-publisher \
    ros-jazzy-xacro \
    ros-jazzy-teleop-twist-keyboard \
    ros-jazzy-teleop-twist-joy
```

---

## 📁 Project Structure

```
gazebo_differential_drive_robot/
 ├── config/        # Configuration files
 ├── launch/        # Launch files
 ├── model/         # Robot model (URDF/Xacro)
 ├── package.xml
 ├── CMakeLists.txt
```

---

## 🚀 Installation

Clone the repository into your ROS 2 workspace:

```bash
git clone https://github.com/Mugilan-Theroboticist/gazebo_differential_drive_robot.git
cd ros_ws
```

Build the workspace:

```bash
colcon build
```

Source the workspace:

```bash
source install/setup.bash
```

---

## ▶️ Run the Simulation

Launch the robot in Gazebo:

```bash
ros2 launch gazebo_differential_drive_robot robot.launch.py
```

---

## 🎮 Teleoperation (Keyboard Control)

Control the robot using keyboard:

```bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```

---

## 🧠 Features

* Differential drive robot model
* Gazebo simulation using Harmonic
* Keyboard teleoperation
* ROS 2 Jazzy compatible
* Modular package structure

---

## 🛠️ Future Improvements

* Add SLAM (mapping)
* Integrate Nav2 navigation
* Add sensors (LiDAR / Camera)
* Real robot deployment

---

## 📜 License

This project is open-source. You can add an MIT License if you plan to share it publicly.

---

## 🙌 Acknowledgment

Built as part of learning and development in ROS 2 and robot simulation.
