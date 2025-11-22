# MENACE

Inspired by Donald Michie’s mechanical reinforcement learning experiment, [MENACE](https://en.wikipedia.org/wiki/Matchbox_Educable_Noughts_and_Crosses_Engine) (Machine Educable Noughts And Crosses).

![Status](https://img.shields.io/badge/status-beta-green)
![Python](https://img.shields.io/badge/python-3.11+-blue)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
<!--[![Tests](https://img.shields.io/badge/tests-%20none-lightgrey)]()-->
<br>

---
<br>

## Overview

<p align="center">
  <img src="MENACE_matchboxes.png" alt="Original MENACE Matchboxes" width="400"/>
</p>

MENACE is a machine learning algorithm designed for very small, discrete state spaces (e.g. Hexapawn or Tic-Tac-Toe). It requires the entire state space and the set of all legal actions from each state to be generated before learning can begin. Each state is assigned a probability distribution over its possible moves, and this distribution is updated over many repeated games based on the outcomes.

Originally, MENACE was implemented physically using matchboxes and colored beads. Each matchbox represented a game state; each bead color corresponded to a possible move. On each turn, a bead was drawn at random to select an action. After a game finished, the bead counts were adjusted. The beads that were drawn throughout the game were increased to reward winning moves or decreased to punish losing ones. Over time, this reinforcement process biases the distribution toward stronger moves, allowing the system to learn an approximately optimal policy.


## Project Status

### Planned
- Improve JSON readability
- Test on Tic-Tac-Toe

### Known Limitations
- **Testing**: This project lacks automated unit tests. Edge cases may not be fully covered.
- **Compatibility**: Some considerations have been made to generalize this implementation, but this project has only been used on [Hexapawn](https://github.com/POACH3/Hexapawn) gameplay.
<br><br>

---
<br>

## Project Info
**Status:** Beta (usable, but lacks unit testing)  
**Author:** T. Stratton  
**Start Date:** 1-NOV-2025  
**License:** MIT License – see [LICENSE](./LICENSE)  
**Language:** Python 3.11+ (tested on 3.11)   
**Topics:** menace, ai, reinforcement-learning, machine-learning