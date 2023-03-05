# Ms-Thesis-en
This repository contains some of my master thesis reports and codes.

My thesis was about balance control of humanoid robots using deep reinforcement learning.

In this project, a hierarchical deep reinforcement learning algorithm is proposed to control a humanoid robot against exerted pushes. The algorithm is shown in the following figure:

![image](https://user-images.githubusercontent.com/79801992/222974189-d17e9f3a-3395-412c-b5ab-587223a1efa4.png)

In the high level control, an actor-critic neural network is designed for the policy learning. The networks architecture is shown here:

![image](https://user-images.githubusercontent.com/79801992/222975254-4b1832f6-df28-4992-9943-4b5e9b9e49cf.png)

For exploration, the Beta distribution is used. For policy optimization the PPO method is used.
Our method is evaluated on a simulation model of a humanoid robot provided in MuJoCo which is shown here:

![image](https://user-images.githubusercontent.com/79801992/222974028-ed88e6dd-6821-44ee-9914-87c59901e04a.png)


The robot is 84 cm high and weights 5.2 kg. It possesses 20 degrees of freedom: six on each leg, three for each hand and two for head. The joints at hands and head are fixed and do not contribute in balance control in this simulation. For each leg, roll and pitch motions on hip, pitch on knee, and pitch and roll on ankle are considered.

The two codes, one is for pure PID controller and the other is for full control algorithm in which the PPO method is implemented.


