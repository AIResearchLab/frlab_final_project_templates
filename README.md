# frlab_final_project_templates

foundations of robotics final project templates

additional matlab example templates are found at [FR_Lab03_Templates](https://github.com/AIResearchLab/FR_Lab03_Templates)

## get the code and build

```bash
# in a terminal on host
mkdir -p catkin_ws/src
cd catkin_ws/src

git clone https://github.com/AIResearchLab/frlab_final_project_templates.git

cd ../
catkin_make
```

## sourcing code in terminal

```bash
# in every new terminal make sure to setup the build sources
source catkin_ws/devel/setup.bash

# followed by ros cli commands
```

## running the simulation

```bash
# in a terminal on host
roslaunch frlab_final_project_templates ball_maze.launch
```


## moving the turtlebot

```bash
# in a terminal on host
export TURTLEBOT3_MODEL=waffle_pi
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
```


## starting in a new position

Change the launch file arguments

```xml
<!--in the ball_maze.launch file-->
<!--change the x and y arguments-->

<!--for example-->
<arg name="x_pos" default="1.4"/>
<arg name="y_pos" default="2.0"/>
```

Or input command line arguments for the launch file

```bash
roslaunch frlab_final_project_templates ball_maze.launch x_pos:=1.4 y_pos:=2.0
```

