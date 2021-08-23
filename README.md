---
Date : Aug 2021
Author : Phạm Quang Minh 
Gmail : Engineer.pqm@gmail.com
---

## Threads
    Move (Robot) to known coordinates X,Y and W =1.

## REQUIREMENTS
This Project requires the following :

 * [Ubuntu 18.04 or newer](https://ubuntu.com/download/desktop)
 * [Ros Melodic](http://wiki.ros.org/melodic/Installation/Ubuntu)
 * [Turtlebot3](https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/)
 
## Usage
    1. (Bringup) Connect PC to a WiFi device and find the assigned IP address 
       https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/
       
    2. (Simulation) Can use Gazebo or use Stage , In this project we use Stage (contact by gmail above)

       
Commonly used commands

- Map
Depending on the usage environment, we have different maps , If Bringup run `roslaunch turtlebot3_bringup turtlebot3_robot.launch` , If Simulation world run `roslaunch turtlebot3_gazebo turtlebot3_world.launch` ....


- Key
`roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch`

- Auto run
`roslaunch turtlebot3_gazebo turtlebot3_simulation.launch` initialization map

- Slam
`roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping`


- Save_map
`rosrun map_server map_saver -f ~/map` create 2 files named : map (map.pgm and map.yaml)

- Rviz 
` roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml` User map from Slam (map.yaml)


## Configuration



## Explain (Vietsub)

#### TOPIC : Move_base 

![Move_base](http://library.isr.ist.utl.pt/docs/roswiki/attachments/move_base/overview_tf.png)


Directory Poin : 
- Base_Move 
- Move.py and Move.cpp Advanced of file Base_move
- Move_ip(x and y coordinates entered from the keyboard)
- Move_with_case (use case replace input )

parameter storage position 

- Move_with_txt(data is stored as text)
- Move_with_dictionary(data is stored as dictionary)


Processing Muti-Poin

NOTE : There are detailed explanations in each piece of code
