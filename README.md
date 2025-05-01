# DOOMgame-using-RLagent
DoomRL (Doom Roguelike) is a unique fusion of the classic first-person shooter, Doom, and the roguelike genre, presenting a challenging environment for AI agents to navigate. In DoomRL, players explore procedurally generated levels, battling hordes of monsters while managing resources and navigating treacherous terrain.



# Game Configuration for DoomRL Agent

Episode Start Time: 20 tics (after unholstering the gun)
Episode Timeout: 300 actions (tics)
Available Buttons:
Move Left
Move Right
Attack
Game Variables in State:
Ammo2
Mode: Player
Doom Skill: 5

Rewards and Penalties in doom basic config. :
+101 reward for killing a monster
-5 penalty for missing a shot
-1 penalty for each step taken
Rewards and Penalties in doom defend config. :
+1 reward for killing a monster
-1 penalty for each step taken




Train the agent using the provided training script.
Evaluate the trained agent's performance in the game environment.


## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.




[![PyPI version](https://badge.fury.io/py/vizdoom.svg)](https://badge.fury.io/py/vizdoom) [![Build and test](https://github.com/Farama-Foundation/ViZDoom/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/Farama-Foundation/ViZDoom/actions/workflows/build-and-test.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

<p align="center">
  <img src="https://raw.githubusercontent.com/Farama-Foundation/ViZDoom/master/docs/_static/img/vizdoom-text.png" width="500px"/>
</p>

ViZDoom allows developing AI **bots that play Doom using only visual information** (the screen buffer). It is primarily intended for research in machine visual learning, and deep reinforcement learning, in particular.

ViZDoom is based on [ZDoom](https://zdoom.org) engine to provide the game mechanics.

![ViZDoom Demo](https://raw.githubusercontent.com/Farama-Foundation/ViZDoom/master/docs/_static/img/vizdoom-demo.gif)


## Features
- Multi-platform (Linux, macOS, Windows),
- API for Python and C++,
- [Gymnasium](https://gymnasium.farama.org/)/Gym environment wrappers (thanks to [Arjun KG](https://github.com/arjun-kg) [Benjamin Noah Beal](https://github.com/bebeal), [Lawrence Francis](https://github.com/ldfrancis), and [Mark Towers](https://github.com/pseudo-rnd-thoughts)),
- Easy-to-create custom scenarios (visual editors, scripting language, and examples available),
- Async and sync single-player and multiplayer modes,
- Fast (up to 7000 fps in sync mode, single-threaded),
- Lightweight (few MBs),
- Customizable resolution and rendering parameters,
- Access to the depth buffer (3D vision),
- Automatic labeling of game objects visible in the frame,
- Access to the audio buffer (thanks to [Shashank Hegde](https://github.com/hegde95)),
- Access to the list of actors/objects and map geometry,
- Off-screen rendering,
- Episodes recording,
- In-game time scaling in async mode.

ViZDoom API is **reinforcement learning** friendly (suitable also for learning from demonstration, apprenticeship learning or apprenticeship via inverse reinforcement learning, etc.).

Julia (thanks to [Jun Tian](https://github.com/findmyway)), Lua, and Java bindings are available in other branches but are no longer maintained.







If you have a cool project that uses ViZDoom or could be interesting to ViZDoom community, feel free to open PR to add it to this list!


## Contributions
This project is maintained and developed in our free time. All bug fixes, new examples, scenarios, and other contributions are welcome! We are also open to feature ideas and design suggestions.

We have a roadmap for future development work for ViZDoom available [here](https://github.com/Farama-Foundation/ViZDoom/issues/546).


## License
The code original to ViZDoom is under MIT license. ZDoom uses code from several sources with [varying licensing schemes](http://zdoom.org/wiki/license).

