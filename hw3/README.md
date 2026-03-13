## Setup

You can run this code on your own machine or on Google Colab. 

1. **Local option:** If you choose to run locally, you will need to install MuJoCo and some Python packages; see [installation.md](../hw1/installation.md) from homework 1 for instructions.

2. **Colab (recommended if you don't want to use GPU locally):** The notebooks install dependencies and run on Colab's CPU/GPU. To use your **local code** in Colab either:
   - **Option A:** Push your code to a GitHub fork, then in the notebook's "clone homework repo" cell change the URL to your fork (e.g. `https://github.com/YOUR_USERNAME/16831-S26-HW.git`), or  
   - **Option B:** After cloning and installing (cells 1–5), upload your modified files from your Mac: use the Colab file browser (left sidebar) and upload `dqn_agent.py`, `dqn_critic.py`, `argmax_policy.py` into `hw_16831/16831-S26-HW/hw3/rob831/agents/`, `.../critics/`, `.../policies/` respectively, overwriting the cloned files.

   Then run the rest of the notebook. **Part I (DQN):** use the "run all DQN experiments" cell to run both DQN and Double DQN on LunarLander in one go. **Part II:** run the actor-critic cells as usual.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cmuroboticsdrl/16831-S26-HW/blob/main/hw3/rob831/scripts/run_hw3_dqn.ipynb) **Part I (Q-learning)**  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cmuroboticsdrl/16831-S26-HW/blob/main/hw3/rob831/scripts/run_hw3_actor_critic.ipynb)     **Part II (Actor-critic)** 


For `fatal error: GL/osmesa.h: No such file or directory`, see [this](https://github.com/ethz-asl/reinmav-gym/issues/35).

## Complete the code

You will then need to implement new routines in the following files for homework 3 part 1 (Q-learning):
- [agents/dqn_agent.py](rob831/agents/dqn_agent.py)
- [critics/dqn_critic.py](rob831/critics/dqn_critic.py)
- [policies/argmax_policy.py](rob831/policies/argmax_policy.py)

and in the following files for part 2 (actor-critic):
- [agents/ac_agent.py](rob831/agents/ac_agent.py)
- [critics/bootstrapped_continuous_critic.py](rob831/critics/bootstrapped_continuous_critic.py)
- [policies/MLP_policy.py](rob831/policies/MLP_policy.py)

The relevant sections are marked with `TODO`.

You may also want to look through [scripts/run_hw3_dqn.py](rob831/scripts/run_hw3_dqn.py) and [scripts/run_hw3_actor_critic.py](rob831/scripts/run_hw3_actor_critic.py) (if running locally) or [scripts/run_hw3_dqn.ipynb](rob831/scripts/run_hw3_dqn.ipynb) and [scripts/run_hw3_actor_critic.ipynb](rob831/scripts/run_hw3_actor_critic.ipynb) (if running on Colab), though you will not need to edit this files beyond changing runtime arguments in the Colab notebook.

See the assignment PDF for more details on what files to edit.
