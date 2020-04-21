## Example - Husky + UR5 + Robotiq 3-Finger Gripper

- Gazebo environment: 

```
roslaunch husky_ur5_3fgripper_gazebo robot_playpen.launch
```

- Stow the robot arm

```
rosrun husky_ur5_3fgripper_gazebo stow_ur5
```

- Close the gripper

```
rosrun husky_ur5_3fgripper_gazebo close_3fgripper
```

- Open the gripper

```
rosrun husky_ur5_3fgripper_gazebo open_3fgripper
```

- Robot arm MoveIt! bringup

```
roslaunch husky_ur5_3fgripper_moveit_config husky_ur5_gripper_moveit_planning_execution.launch
```

- Mobile base Navigation stack bringup

```
roslaunch husky_ur5_3fgripper_gazebo amcl_demo.launch
```
