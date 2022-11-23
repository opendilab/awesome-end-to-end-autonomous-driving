# Awesome End-to-End Autonomous driving

This is a collection of research papers for **End-to-End Autonomous driving**.
And the repository will be continuously updated to track the latest update of E2E driving.

Welcome to follow and star!

## Table of Contents

- [A Overview of End-to-End Driving Method](#a-Overview-of-End-to-End-Driving-Method)
- [Papers](#papers)

  - [ECCV 2022](#ECCV-2022) 
  - [ICLR 2022](#ICLR-2022) 
  - [CVPR 2022](#CVPR-2022) 
  - [CVPR 2021](#CVPR-2021) 
  - [CVPR 2020](#CVPR-2020) 
  - [ICCV 2021](#ICCV-2021) 
  - [NeurIPS 2022](#NeurIPS-2022) 
  - [CoRL 2022](#CoRL-2022) 
  - [CoRL 2021](#CoRL-2021) 
  - [T-PAMI](#T-PAMI) 
  - [Arxiv](#arxiv)
- [Contributing](#contributing)


## An Overview of End-to-End Driving Method

The end-to-end driving methods aim at building a drive model that at each timestamp maps sensor readings (RGB & LiDAR), high-level navigational command, and vehicle state to raw control command. Most of the works are realized on the CARLA which is an open-source urban simulator for autonomous driving research. The other simulators include [Sumo](https://www.eclipse.org/sumo/) , [MetaDrive](https://github.com/metadriverse/metadrive) and [SMARTS](https://simfactor.pl/our-offer/driver-training-solutions/smart-simulator/?lang=en) . The end-to-end driving methods can be divided into two mainstreams: imitation learning and reinforcement learning.

<img src="assets/pipeline.png" height="350">


## Papers

```
format:
- [title](paper link) [links]
  - author1, author2, and author3.
  - key 
  - experiment environment
```


### ECCV 2022
- [KING: Generating Safety-Critical Driving Scenarios for Robust Imitation via Kinematics Gradients](https://arxiv.org/abs/2204.13683)
	- Niklas Hanselmann, Katrin Renz, Kashyap Chitta, Apratim Bhattacharyya, Andreas Geiger
	- Key: scenarios generation, proxy model, optimization 
	- Env: [CARLA](https://carla.org/)
- [Learning to Drive by Watching YouTube Videos: Action-Conditioned Contrastive Policy Pretraining](https://arxiv.org/pdf/2204.02393.pdf)
	- Qihang Zhang, Zhenghao Peng, and Bolei Zhou
	- Key: learning from unlabeled data, feature pretraining
	- Env: [CARLA](https://carla.org/)

### ICLR 2022
- [Efficient Learning of Safe Driving Policy via Human-AI Copilot Optimization](https://arxiv.org/abs/2202.10341)
	- Quanyi Li, Zhenghao Peng, Bolei Zhou
	- Key: human intervention, safety, demonstration
	- Env: [MetaDrive](https://github.com/metadriverse/metadrive)

### CVPR 2022
- [Learning from All Vehicles](https://arxiv.org/abs/2203.11934)
	- Dian Chen, Philipp Krähenbühl
	- Key: supervisory task, viewpoint invariant intermediate representation
	- Env: [CARLA](https://carla.org/)
- [COOPERNAUT: End-to-End Driving with Cooperative Perception for Networked Vehicles](https://arxiv.org/abs/2205.02222)
	- Jiaxun Cui, Hang Qiu, Dian Chen, Peter Stone, Yuke Zhu
	- Key: cooperative driving, cross-vehicle perception, communication
	- Env: [CARLA](https://carla.org/) , [AUTOCASTSIM](https://github.com/hangqiu/AutoCastSim)


### CVPR 2021
- [Multi-Modal Fusion Transformer for End-to-End Autonomous Driving](https://arxiv.org/abs/2104.09224)
	- Aditya Prakash, Kashyap Chitta, Andreas Geiger
	- Key: multi-modal fusion, transformer, imitation learning
	- Env: [CARLA](https://carla.org/)
- [Learning by Watching](https://arxiv.org/abs/2106.05966)
	- Jimuyang Zhang, Eshed Ohn-Bar
	- Key: imitation learning,  demonstration, intermediate representation
	- Env: [CARLA](https://carla.org/)


### CVPR 2020
- [Learning situational driving](https://openaccess.thecvf.com/content_CVPR_2020/papers/Ohn-Bar_Learning_Situational_Driving_CVPR_2020_paper.pdf)
	- Eshed Ohn-Bar, Aditya Prakash, Aseem Behl, Kashyap Chitta, Andreas Geiger
	- Key: situational driving policy, mixture model, behavior cloning
	- Env: [CARLA](https://carla.org/)
- [Exploring the Limitations of Behavior Cloning for Autonomous Driving](https://arxiv.org/abs/1904.08980)
	- Felipe Codevilla, Eder Santana, Antonio M. López, Adrien Gaidon
	- Key: behavior cloning, visuomotor policy, driving benchmark
	- Env: [CARLA](https://carla.org/)
- [End-to-End Model-Free Reinforcement Learning for Urban Driving using Implicit Affordances](https://arxiv.org/abs/1911.10868)
	- Marin Toromanoff, Emilie Wirbel, Fabien Moutarde
	- Key: implicit affordance, reinforcement learning, data efficiency
	- Env: [CARLA](https://carla.org/) , [TORCS](https://sourceforge.net/projects/torcs/)

### ICCV 2021
- [End-to-End Urban Driving by Imitating a Reinforcement Learning Coach](https://arxiv.org/abs/2108.08265)
	- Zhejun Zhang, Alexander Liniger, Dengxin Dai, Fisher Yu, Luc Van Gool
	- Key: imitation learning, reinforcement learning
	- Env: [CARLA](https://carla.org/)
- [NEAT: Neural Attention Fields for End-to-End Autonomous Driving](https://arxiv.org/abs/2109.04456)
	- Key: attention map, iterative generation, auxiliary semantics
	- Env: [CARLA](https://carla.org/)
- [Learning to drive from a world on rails](https://arxiv.org/abs/2105.00636)
	- Dian Chen, Vladlen Koltun, Philipp Krähenbühl
	- Key: model-based, offline reinforcement learning, policy distillation
	- Env: [CARLA](https://carla.org/)


### NeurIPS 2022
- [Trajectory-guided Control Prediction for End-to-end Autonomous Driving: A Simple yet Strong Baseline](https://arxiv.org/abs/2206.08129)
	- Penghao Wu, Xiaosong Jia, Li Chen, Junchi Yan, Hongyang Li, Yu Qiao
	- Key: multi-step prediction, trajectory guidance, connected branches
	- Env: [CARLA](https://carla.org/)

### CoRL 2022
- [Safety-Enhanced Autonomous Driving Using  Interpretable Sensor Fusion Transformer](https://arxiv.org/abs/2207.14024) (**<font color="red">Ours!!!</font>**)
	- Hao Shao, Letian Wang, RuoBing Chen, Hongsheng Li, Yu Liu
	- Key: autonomous driving, sensor fusion, transformer, safety
	- Env: [CARLA](https://carla.org/)
- [PlanT: Explainable Planning Transformers via Object-Level Representations](https://arxiv.org/abs/2210.14222)
	- Katrin Renz, Kashyap Chitta, Otniel-Bogdan Mercea, A. Sophia Koepke, Zeynep Akata, Andreas Geiger
	- Key: autonomous Driving, transformers, explainability
	- Env: [CARLA](https://carla.org/)

### CoRL 2020
- [Learning by cheating](https://arxiv.org/abs/1912.12294)
	- Dian Chen, Brady Zhou, Vladlen Koltun, Philipp Krähenbühl
	- Key:  imitation learning, sensorimotor control
	- Env: [CARLA](https://carla.org/)
- [SAM: Squeeze-and-Mimic Networks for Conditional Visual Driving Policy Learning](https://arxiv.org/abs/1912.02973)
	- Albert Zhao, Tong He, Yitao Liang, Haibin Huang, Guy Van den Broeck, Stefano Soatto
	- Key: conditional imitation learning, side task
	- Env: [CARLA](https://carla.org/)


### T-PAMI
- [MetaDrive: Composing Diverse Driving Scenarios for Generalizable Reinforcement Learning](https://arxiv.org/abs/2109.12674)
	- Quanyi Li, Zhenghao Peng, Lan Feng, Qihang Zhang, Zhenghai Xue, Bolei Zhou
	- Key : reinforcement learning, procedural generation, real data import
	- Env: [MetaDrive](https://github.com/metadriverse/metadrive)
- [TransFuser: Imitation with Transformer-Based Sensor Fusion for Autonomous Driving](https://arxiv.org/abs/2205.15997)
	- Kashyap Chitta, Aditya Prakash, Bernhard Jaeger, Zehao Yu, Katrin Renz, Andreas Geiger
	- Key: imitation learning, sensor fusion, transformers, attention
	- Env: [CARLA](https://carla.org/)

### arXiv
- [GRI: General Reinforced Imitation and its Application to Vision-Based Autonomous Driving](https://arxiv.org/abs/2111.08575)
	- Raphael Chekroun, Marin Toromanoff, Sascha Hornauer, Fabien Moutarde
	- Key: demonstration, multi-view input, offline learning
	- Env: [CARLA](https://carla.org/)
- [Nocturne: a scalable driving benchmark for bringing multi-agent learning one step closer to the real world](https://arxiv.org/abs/2206.09889)
	- Eugene Vinitsky, Nathan Lichtlé, Xiaomeng Yang, Brandon Amos, Jakob Foerster
	- Key: high-speed simulator, obstruction, complex scene
	- Env: [Nocturne](https://github.com/facebookresearch/nocturne)
- [Accelerating Reinforcement Learning for Autonomous Driving using Task-Agnostic and Ego-Centric Motion Skills](https://arxiv.org/abs/2209.12072) (**<font color="red">Ours!!!</font>**)
	- Tong Zhou, Letian Wang, Ruobing Chen, Wenshuo Wang, Yu Liu
	- Key: reinforcement learning, exploration, motion primitive
	- Env: [MetaDrive](https://github.com/metadriverse/metadrive)

## Contributing
Our purpose is to make this repo even better. If you are interested in contributing, please refer to [HERE](CONTRIBUTING.md) for instructions in contribution.

## License
Awesome End-to-End Autonomous driving is released under the Apache 2.0 license.
