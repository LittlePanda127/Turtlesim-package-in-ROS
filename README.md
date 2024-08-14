turtlesim-package-in-ROS

We will walk you through the process of modifying the turtle package in ROS-noetic after installing and configuring ROS.

To begin, open a terminal. It's crucial to use the following command to launch the ROS master node:
```
roscore
```
![image](https://github.com/user-attachments/assets/9041bf63-28fd-45b0-9345-fb9573cc6d8f)


I started up a second terminal. I'll give it another go at running Ros Master to see what happens. 







We already have nodes that you can start when we install ROS; you have standard nodes for instructional nodes and multiple nodes for various functions.
 1. In order to launch a node, we will use the command, which appears to be a program that prints "hello world" along with a date to the terminal.

```
rosrun rospy_tutorials talker
```
![image](https://github.com/user-attachments/assets/6e3a6dcb-7dd6-4c7b-abbd-1204e94c9e39)

You can use the keyboard shortcut Ctrl + C to halt the node, but avoid doing so in order to avoid seeing an error or shortcoming.

 2-To see a graphical representation of the real ROS (nodes, topics, and connections that are operating on your computer), open a second terminal and enter this command.

```
rqt_graph
```
![image](https://github.com/user-attachments/assets/048b014a-ccc2-497b-9d9d-04194d329c9f)


As you can see, there is just ONE node here, called "talker."

3-This is an additional application that will print something to the terminal and (hear) the timestamp along with "hello world." in fact, this info is coming from the node (talker)

![image](https://github.com/user-attachments/assets/55ea6517-f348-4f3c-9a4f-15abea8fbd66)
![image](https://github.com/user-attachments/assets/02f51a7a-3045-4752-ad1d-c03bc516d32f)
![image](https://github.com/user-attachments/assets/499f210b-7555-4a45-964d-3a3a80e5fe3d)


As you can see, we have a token node here. Both a (talker) and a (listener) node are present here. The listener node receives some messages from the talker node.


Turtlesim 1: This command will display a turtle in a graphical window.
```
rosrun turtlesim turtlesim_node
```
![image](https://github.com/user-attachments/assets/cbb95aa9-e215-4f4b-86da-4bf3f0b2c1da)
![image](https://github.com/user-attachments/assets/0d68e6cc-d56f-4efd-bdf5-37aa124a5434)


2. Using the arrow keys on your keyboard, you can manipulate the turtle with this command.
```
rosrun turtlesim turtle_teleop_key
```

![image](https://github.com/user-attachments/assets/ea2f3ff3-dfd4-4820-bf77-10c18018c6da)

