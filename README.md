# frlab_final_project_templates

---

foundations of robotics final project templates


## get the code and build

```bash
# in a terminal
mkdir -p catkin_ws/src
cd catkin_ws/src

git clone https://github.com/AIResearchLab/frlab_final_project_templates.git

cd ../
catkin_make
```


## running the simulation

```bash
# in a terminal
roslaunch frlab_final_project_templates ball_maze.launch
```


## moving the turtlebot

```bash
# in a terminal
export TURTLEBOT3_MODEL=waffle_pi
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
```
