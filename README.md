# PacmanDQN
Deep Reinforcement Learning in Pac-man
## Overview

This project is part of the **Reinforcement Learning (RL)** course in the **M.Sc. Artificial Intelligence and Machine Learning** program at **Christ (Deemed to be University), Bangalore**. The exercise is based on the **UC Berkeley RL Exercise**, which includes a Pacman game framework designed to train RL agents to play the game (or a simplified version of it).

## Team Members

- **Samson Sabu**  
- **Guhan S.**

## Demo

[![Demo](https://github.com/tychovdo/PacmanDQN/blob/master/videos/PacmanDQN_wingif.gif)](https://youtu.be/QilHGSYbjDQ)

## Example usage

Run a model on `smallGrid` layout for 6000 episodes, of which 5000 episodes
are used for training.

```
$ python3 pacman.py -p PacmanDQN -n 6000 -x 5000 -l smallGrid
```

### Layouts
Different layouts can be found and created in the `layouts` directory

### Parameters

Parameters can be found in the `params` dictionary in `pacmanDQN_Agents.py`. <br />
 <br />
Models are saved as "checkpoint" files in the `/saves` directory. <br />
Load and save filenames can be set using the `load_file` and `save_file` parameters. <br />
 <br />
Episodes before training starts: `train_start` <br />
Size of replay memory batch size: `batch_size` <br />
Amount of experience tuples in replay memory: `mem_size` <br />
Discount rate (gamma value): `discount` <br />
Learning rate: `lr` <br />
 <br />
Exploration/Exploitation (ε-greedy): <br />
Epsilon start value: `eps` <br />
Epsilon final value: `eps_final` <br />
Number of steps between start and final epsilon value (linear): `eps_step` <br />

## Citation

Please cite this repository if it was useful for your research:

```
@article{van2016deep,
  title={Deep Reinforcement Learning in Pac-man},
  subtitle={Bachelor Thesis},
  author={van der Ouderaa, Tycho},
  year={2016},
  school={University of Amsterdam},
  type={Bachelor Thesis},
}

```

* [van der Ouderaa, Tycho (2016). Deep Reinforcement Learning in Pac-man.](https://moodle.umons.ac.be/pluginfile.php/404484/mod_folder/content/0/Pacman_DQN.pdf)

## Requirements

- `python==3.5.1`
- `tensorflow==0.8rc`

## Acknowledgements

DQN Framework by  (made for ATARI / Arcade Learning Environment)
* [deepQN_tensorflow](https://github.com/mrkulk/deepQN_tensorflow) ([https://github.com/mrkulk/deepQN_tensorflow](https://github.com/mrkulk/deepQN_tensorflow))

Pac-man implementation by UC Berkeley:
* [The Pac-man Projects - UC Berkeley](http://ai.berkeley.edu/project_overview.html) ([http://ai.berkeley.edu/project_overview.html](http://ai.berkeley.edu/project_overview.html))
