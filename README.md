# Robot Simulation: Differential Wheeled Car & Humanoid URDF

## Project Overview

This repository contains two simulation models built using ROS2 (Robot Operating System 2) and URDF (Unified Robot Description Format). The project includes a **Differential Wheeled Car** model designed to teach robot programming using ROS2 and Gazebo, and a **Humanoid Robot** model focused on inertia and collision dynamics. The goal of this repository is to provide a hands-on experience for students learning robotics programming, robot modeling, and simulation.

---

## 🚗 Differential Wheeled Car Simulation (ROS2)

### 📝 Description
The **Differential Wheeled Car** simulation is designed to help undergraduate students learn robot programming using ROS2. This project allows students to control a robot's movement in a simulated environment and interact with various "worlds" (environments) in Gazebo. The car model uses a differential drive system, where two independently controlled wheels enable the robot to move forward, backward, and turn.

This project covers essential skills for robotics, such as:
- Creating and programming robot models.
- Moving the robot in a simulated environment.
- Interacting with different types of simulated environments, including obstacles and terrain.
- Programming robot behaviors using ROS2 messages.

### 🎯 Objective
The objective of this project is to:
- Teach students how to create a robot model and move it in a simulated environment using ROS2.
- Introduce the concept of "worlds" (simulated environments) where the robot can interact with objects and obstacles.
- Provide experience in programming robot behaviors (e.g., movement, turning, avoiding obstacles).
- Enable students to experiment with different simulated worlds (e.g., mazes, outdoor terrains) and adapt robot behaviors accordingly.

### 🛠️ Project Phases
1. **Setup and Configuration**:
   - Set up a ROS2 workspace using colcon to manage your project.
   - Install necessary tools like Gazebo for simulation and RViz for visualization.

2. **Robot Model Creation**:
   - Create a robot model using URDF or SDF files to define the robot’s shape, sensors (e.g., cameras, LIDAR), and actuators (e.g., wheels).
   - Load the robot model into Gazebo to visualize it in a 3D environment.

3. **Robot Movement**:
   - Program basic movement controls for the robot using ROS2 messages like `cmd_vel` to move the robot forward, backward, or turn in place.
   - Create a simple ROS2 node that sends velocity commands to control the robot’s movement within the simulation.

4. **Creating and Modifying Worlds**:
   - Learn how to design and modify worlds in Gazebo by adding elements like obstacles, ramps, and terrain features.
   - Simulate different environments, such as indoor rooms or outdoor terrains, for the robot to navigate through.



### 🛠️ Files inside src

#### Key Directories and Files:
- **`my_robot_bringup/`**: Contains files for launching and configuring the robot.
  - **`CMakeLists.txt`**: ROS2 build configuration file.
  - **`package.xml`**: ROS2 package configuration file.
  - **`config/`**: Contains configuration files.
  - **`launch/`**: ROS2 launch files for starting simulations and robot programs.
  - **`rviz/`**: RViz configuration files for visualization.

- **`my_robot_description/`**: Contains the URDF and robot description files.
  - **`CMakeLists.txt`**: ROS2 build configuration file for the robot description.
  - **`package.xml`**: ROS2 package configuration for the robot description.
  - **`launch/`**: Launch files specific to loading and configuring the robot in the simulation.
  - **`rviz/`**: RViz files for visualization of the robot.
  - **`urdf/`**: URDF files that describe the robot’s physical structure, including links, joints, sensors, and actuators.
 
## 🤖 Humanoid Robot URDF

📝 Description
The Humanoid Robot model is designed for students and researchers to study the dynamics of human-like robots, focusing on inertia and collision properties. The humanoid robot includes multiple joints, actuators, and links that simulate human-like movements. It is used to explore more complex behaviors such as balancing, walking, and collision detection in Gazebo.

This model is typically used for:

Analyzing the physics of robot movement.

Studying the effects of joint constraints and actuator capabilities.

Investigating collision detection algorithms to avoid robot body parts colliding during movement.

🛠️ Files
humanoid_robot/: Contains the URDF files for the humanoid robot model.

humanoid.urdf: The URDF file that describes the humanoid robot’s structure, including its joints, links, and collision properties.

### 🛠️ How to Run
1. Install ROS2 and Gazebo.
2. Clone this repository into your ROS2 workspace:
   ```bash
   cd ~/ros2_ws/src
   git clone https://github.com/yourusername/repo-name.git
