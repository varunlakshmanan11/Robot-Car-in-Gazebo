### Getting Started

1. **Unzip the Package File**
   - Unzip the provided package file.

2. **Copy Package Contents**
   - Copy the contents of the unzipped package and paste them into your ROS2 workspace.

3. **Build the Package**
   - Navigate to the root of your workspace and build the package using the following command:
     ```
     colcon build
     ```

4. **Source the Workspace**
   - Source your workspace by running:
     ```
     source install/setup.bash
     ```

### Running the Package

5. **Launch a Desired File**
   - To run the desired launch file, use the following command:
     ```
     ros2 launch pr1 <launchfile.launch.py>
     ```

6. **Using Teleoperation**
   - To run the teleoperation package, execute:
     ```
     ros2 run teleop top
     ```

7. **Open-Loop Controller**
   - To run the open-loop controller, use the following command:
     ```
     ros2 run tb_control tb_closedLoop
     ```

### Additional Notes

8. **Open-Loop Controller Configuration**
   - If you intend to use the open-loop controller, make sure to edit the `spawn_robot_ros2.launch.py` file and adjust the position and orientation values as follows:
     - Position: [X, Y, Z] = [0.0, 0.0, 1.0]
     - Orientation: [Roll, Pitch, Yaw] = [0.0, 0.0, 4.712]

9. **Competition Launch Configuration**
   - When using the `competition.launch.py` file, ensure you modify the `spawn_robot_ros2.launch.py` with the following values:
     - Position: [X, Y, Z] = [1.6, 2.0, 1.0]
     - Orientation: [Roll, Pitch, Yaw] = [0.0, 0.0, 1.57079633]

These instructions will help you set up and run the ROS2 package effectively. Please follow the steps carefully to ensure proper functionality.
