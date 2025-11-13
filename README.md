# 🚧 This repository is under internal review. Estimated release date: Nov 27 - Dec 10.

<h1 align="center">🕸️ SPIDER: Scalable Physics-Informed DExterous Retargeting</h1>

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT">
  </a>
  <a href="https://www.python.org/downloads/">
    <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="Python 3.12+">
  </a>
  <a href="https://pytorch.org/">
    <img src="https://img.shields.io/badge/PyTorch-2.0+-ee4c2c.svg" alt="PyTorch">
  </a>
  <a href="http://arxiv.org/abs/2511.09484">
    <img src="https://img.shields.io/badge/arXiv-2406.12345-b31b1b.svg" alt="arXiv">
  </a>
  <a href="https://jc-bao.github.io/spider/">
    <img src="https://img.shields.io/badge/docs-latest-blue.svg" alt="Documentation">
  </a>
  <a href="https://jc-bao.github.io/spider-project/">
    <img src="https://img.shields.io/badge/website-project-blue.svg" alt="Project Website">
  </a>
</p>

![logo](figs/teaser.png)

## Overview

Scalable Physics-Informed DExterous Retargeting (SPIDER) is a general framework for physics-based retargeting from human to diverse robot embodiments, including both dexterous hand and humanoid robot.
It is designed to be a minimum, flexible and extendable framework for human2robot retargeting.
This code base provides the following pipeline from human video to robot actions:

![pipeline](figs/pipeline_animation.gif)


## Gallery

### Simulation results:

| Inspire Pick Tea Pot (Gigahands Dataset) | Xhand Play Glass (Hot3D dataset) | Schunk Pick Board (Oakink dataset) | Allegro Pick Cat Toy (Reconstructed from single RGB video)
| ------- | ------- | ------- | ------- |
| ![](figs/sim/inspire_pick_pot.gif) | ![](figs/sim/xhand_glass.gif) | ![](figs/sim/schunk_move_board.gif) | ![](figs/sim/allegro_pick_cat.gif) |


| G1 Pick | G1 Run | H1 Kick | T1 skip |
| ------- | ------- | ------- | ------- |
| ![](figs/sim/g1_pick.gif) | ![](figs/sim/g1_run.gif) | ![](figs/sim/h1_kick.gif) | ![](figs/sim/t1_skip.gif) |


### Multiple viewer support:
| Mujoco | Rerun |
| ------- | ------- |
| ![](figs/viewers/mujoco_viewer.gif) | ![](figs/viewers/rerun_viewer.gif) |


### Multiple simulators support:

| Genesis | Mujoco Warp |
| ------- | ------- |
| ![](figs/sim/dexmachina.gif) | ![](figs/sim/mjwarp.gif) |

### Deployment to real-world robots:

| Pick Cup | Rotate Bulb | Unplug Charger | Pick Duck |
| ------- | ------- | ------- | ------- |
| ![](figs/real/pick_cup_real.gif) | ![](figs/real/rotate_bulb_real.gif) | ![](figs/real/unplug_real.gif) | ![](figs/real/pick_duck_real.gif) |


## Features

- First general **physics-based** retargeting pipeline for both dexterous hand and humanoid robot.
- Supports 9+ robots and 6+ datasets out of the box.
- Seemless integration with RL training and data augmentation for BC pipeline.
- Native support for multiple simulators (Mujoco Wrap, Genesis) and multiple downstream training pipelines (HDMI, DexMachina).
- Sim2real ready.

![](figs/embodiment_support.png)

## Citation

```bibtex
@misc{pan2025spiderscalablephysicsinformeddexterous,
      title={SPIDER: Scalable Physics-Informed Dexterous Retargeting},
      author={Chaoyi Pan and Changhao Wang and Haozhi Qi and Zixi Liu and Homanga Bharadhwaj and Akash Sharma and Tingfan Wu and Guanya Shi and Jitendra Malik and Francois Hogan},
      year={2025},
      eprint={2511.09484},
      archivePrefix={arXiv},
      primaryClass={cs.RO},
      url={https://arxiv.org/abs/2511.09484},
}
```
