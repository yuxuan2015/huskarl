<img align="left" src="https://github.com/danaugrs/huskarl/blob/master/logo.png">

# Huskarl

Huskarl is a framework for deep reinforcement learning focused on research and fast prototyping.
It's built on TensorFlow 2.0 and uses the `tf.keras` API when possible for conciseness and readability.

Huskarl makes it easy to parallelize computation of environment dynamics across multiple CPUs.
This is useful for speeding up on-policy learning algorithms that benefit from multiple concurrent sources of experience such as A2C or PPO.
It is specially useful for computationally intensive environments such as physics-based ones.

Huskarl works seamlessly with [OpenAI Gym](https://gym.openai.com/) environments.

There are plans to support multi-agent environments and [Unity3D environments](https://unity3d.ai).

## Algorithms

Several algorithms are implemented already and many more are planned.

* [x] Deep Q-Learning Network (DQN)
* [x] Multi-step DQN
* [x] Double DQN
* [x] Dueling Architecture DQN
* [x] Advantage Actor-Critic (A2C)
* [ ] Deep Deterministic Policy Gradient (DDPG)
* [ ] Proximal Policy Optimization (PPO)
* [ ] Prioritized Experience Replay
* [ ] Curiosity-Driven Exploration


## Installation

Since TensorFlow 2.0 is not officially out yet you need to install it and other dependencies manually for now:
```
pip install -r requirements.txt
```

## Test
```
    git clone https://github.com/danaugrs/huskarl
    cd huskarl/examples
    python a2c-cartpole.py
or
    python dqn-cartpole.py
```

## Citing

If you use Huskarl in your research, you can cite it as follows:
```
@misc{salvadori2019huskarl,
    author = {Daniel Salvadori},
    title = {huskarl},
    year = {2019},
    publisher = {GitHub},
    journal = {GitHub repository},
    howpublished = {\url{https://github.com/danaugrs/huskarl}},
}
```

## About

_hùskarl_ in Old Norse means a warrior who works in his/her lord's service.
