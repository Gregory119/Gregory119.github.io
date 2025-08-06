---
layout: page
title: Deep Reinforcement Learning for Set-Point Motion of Robot Arm
description: Trained a PPO policy with Stablebaselines3 to move the end-effector of a robot arm to an arbitrary position in a custom made Mujoco based Gymnasium environment.
img: assets/img/sim-arm.png
importance: 1
category: work
---

Source Code: [https://github.com/Gregory119/RBE501-RL-arm-project](https://github.com/Gregory119/RBE501-RL-arm-project)

Skills: Python, Mujoco, Gymnasium, Stablebaselines3, PPO, Reward Shaping, Dynamics

The primary goal was to train a deep reinforcement learning policy (eg. PPO) to move the end-effector of the SO-101 robot arm to a goal position (excluding orientation) as fast as possible. The secondary goal was to investigate how the trained policy is affected by changes in the underlying dynamics model. This second goal is important for sim-to-real transfer, whereby the simulated model has differences to the physical model. The dynamics were modified by scaling the mass and inertia of every link. Please see the detailed report below as well as the demonstration and presentation videos.


<div class="row justify-content-sm-center">
{% include youtubePlayer.html id='6Wg1nTYCRAI' %}
</div>
<div class="caption">
    Example visual performance of the trained PPO policy for several trajectories without any modifications to the dynamics model. The goal was reached within 0.6 s and a final positional error of 0.007 m.
</div>

<div class="row justify-content-sm-center">
{% include youtubePlayer.html id='ZvdFMUgYHx0' %}
</div>
<div class="caption">
    Presentation video with the first speaker Gregory Jones, and the second speaker Nathaniel Bernal.
</div>

<iframe src="https://drive.google.com/file/d/1G2tplMlQSXy_Byd5qggdpWS8j8BTN_dG/preview" width="1000" height="1000"></iframe>
