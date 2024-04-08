# Server_simulation
Simulation For Server Bot
The following is a package showcasing simulation for the server bot on Ros2 using nav2. 

Clone the repository to src in your ros2 workspace 
```bash
git clone https://github.com/pranavmenon2408/Server_simulation.git
```
Build the package
```bash
colcon build --packages-select urdf_base_description
```
Export the Gazebo model path to models folder in package
```bash
export GAZEBO_MODEL_PATH=/path/to/urdf_base_description/models:$GAZEBO_MODEL_PATH
```
Add above command to .bashrc to avoid running it in every new terminal 

Source the workspace and run the launch file

```bash
source install/setup.bash
ros2 launch urdf_base_description gazebo.launch.py
```
