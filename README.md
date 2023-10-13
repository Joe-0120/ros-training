# ros-training
Training task for space concordia robotics team

To run the nodes, clone this repository to the src directory in a ros workspace.
In the root of the workspace, run rosdep to check for missing dependecies: ```rosdep install -i --from-path src --rosdistro humble -y```
Build the new packages:
```colcon build --packages-select cpp_publisher```
```colcon build --packages-select py_subscriber```
Open 2 new terminals and source the setup files:
```source install/setup.bash```
Run the talker node in a terminal and a listener node in another terminal:
```ros2 run cpp_publisher talker```
```ros2 run cpp_listener listener```
