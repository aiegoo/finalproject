# finalproject
All packages are built under Ubuntu 18.04 ROS1 melodic.

* (remark) All launch files just call limited_joint_robot for moveit compatibility.
 
# UR5 + Robotiq AF85 gripper
( AF85 gripper package has been imported from StanleyInnovation github repo : https://github.com/StanleyInnovation/robotiq_85_gripper )

 - AF85 + UR5 view  
```
roslaunch ur5_gripper view_ur5_robotiq.launch
```

 - AF85 gripper gazebo launch
```
roslaunch ur5_gripper ur5_gazebo_robotiq.launch
```

 - AF85 moveit launch
```
roslaunch ur5_gripper_moveit_config move_group.launch
```
 - AF85 moveit rviz

```
roslaunch ur5_gripper_moveit_config moveit_rviz.launch config:=true
```

Because of GAZEBO instability with AF85 (robot breaks down after certain amount of vibration accumulation w/r/t AF85), I changed some of continuous joints of AF85 to 'fixed' from 'continous'.

For the static AF85 GAZEBO simulation, use the following command instead.

```
roslaunch ur5_gripper ur5_gazebo_robotiq_static.launch
```

# UR5 + RG2 gripper

 - RG2 view - rviz
```
roslaunch ur5_gripper view_ur5_rg2.launch
```

 - RG2 gazebo launch
```
roslaunch ur5_gripper ur5_gazebo_rg2.launch
```

