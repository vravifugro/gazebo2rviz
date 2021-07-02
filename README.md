# Gazebo2RVIZ Package 

## Overview 

This package mainly aims to translate gazebo-ROS based SDF models into RVIZ via 'tfs' and 'marker-based' references. 

## Documentation 

Refer this article for a better overview on the work-logic behind it 
`http://andreasbihlmaier.github.io/2014/02/19/gazebo2rviz.html`

## Run Instructions 

- Create a ros workspace, `mkdir ros_ws && cd ros_ws`
- Create a src folder, `mkdir src && cd src`
- Clone this repo by using `git@github.com:vravifugro/gazebo2rviz.git`
- cd `~/ros_ws` && run `catkin_make`
- In a new terminal, Spin up a gazebo instance, `rosrun gazebo_ros gazebo` and start adding sdf parts from the 'Insert' panel 
- In a new terminal, Spin up RVIZ `rosrun rviz rviz` and change `global frame -> world` and include the `marker` plugin from 'Add'.
- Then, `cd  ~/ros_ws`, spin up a terminal and run 
  `roslaunch gazebo2rviz gazebo2rviz.launch`, now you will see the Gazebo parts translated in RVIZ with relative update based on addition/movement/deletion and morphing of the objects.
  

