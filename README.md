# ecse373_f23_ech89__navvis_description

Code is ran by doing the following:

Setting up the project:

`source /opt/ros/noetic/setup.bash`

`source devel/setup.bash`

`roscore &`

Then setting the robot_description and the my_robot:

`rosparam set /robot_description urdf_from_xacro.urdf`

`rosparam set /my_robot -t robot.xacro`

Then running the launch file:
`roslaunch navvis_description display.launch use_xacro:=true use_joint_state_publisher_gui:=false & `
