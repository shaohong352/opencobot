# What is OpenCobot?

OpenCobot is an Intelligent Cobot with AI assistant to do multipule tasks autonamously. Contrasted to the classic cobot which using teach pendant or offline programming,OpenCobot using sensors like camera and force torque sensor to percept the surrounding enviroment and make decision of trajectory and actuation in real time. This will tremenslly save the programming work for the robot to do new task.

# How does it work?

We using a [ROS](https://ros.org) based controller to munipulate the Cobot. An policy agent sending the planed trajectory and actuations perodically to the controller. To get a practical usable agent will take serveral steps:

* 3D and force perception of the enviroment as well as the intrinsic joints state of the robot to build a state space.
* A model-free agent will be trainning in a simulator using a reinforcement learning to get a policy can mapping the state space to action space on the best policy.
* A dense reward will be tranning end2end in advance with no pendant demo or just one shot demo.
* sim2real enhancement to migrate the policy in the real world.

# Sensors

OpenCobot support multimodality sensors. 
