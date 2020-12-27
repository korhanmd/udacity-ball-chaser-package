# `ball_chaser` Package

[![Udacity - Robotics NanoDegree Program](https://s3-us-west-1.amazonaws.com/udacity-robotics/Extra+Images/RoboND_flag.png)](https://www.udacity.com/robotics)

This is the `ball_chaser` package of [Go Chase It!](https://github.com/korhanmd/udacity-go-chase-it) project (second project of Udacity's Robotics Software Engineer Nanodegree).
It includes scripts for robot behaviour. They include `drive_bot` and `process_image` nodes. `drive_bot` node has service to publish velocities to the robot.
`process_image` node processes the image captured by camera. Checks for white ball. If it finds a white ball, requests service to move robot through the ball.

To use you need to create catkin workspace first, if it doesn't exist. To create it, go to the directory you want to create workspace and write commands below to the terminal.

```
$ mkdir -p catkin_ws/src
$ cd catkin_ws/src
$ catkin_init_workspace
```

Then create `ball_chaser` package with commands below inside src folder of the workspace.

```
$ catkin_create_pkg ball_chaser
```

Copy the content of this repository inside `ball_chaser` directory. Then go to the root folder of your workspace. Use the commands below to build sources and load robot and the world.

```
$ catkin_make
$ source devel/setup.bash
$ roslaunch ball_chaser ball_chaser.launch
```
