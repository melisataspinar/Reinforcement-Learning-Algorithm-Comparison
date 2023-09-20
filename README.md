Imagine an RL robot that needs to learn to take freshly painted cups from a painting machine, dry them, and place the dried cups on a shelf. We assign a +10 reward for storing dry cups on the shelf and a +5 reward for storing wet cups. The robot can attempt to dry any held cup, but there is a small chance (0.1) that the cup will break during the process, incurring a high cost (-20). If the robot decides to grab a new cup from the painting machine while already having a cup, it will drop and break the held cup (-20). The robot must now try to determine which policy to use for this task.

In this notebook, I use such a model to compare the following algorithms:
- Policy Iteration (with the initial policy of a0 for all states)
- Value Iteration (with the initial value of zero for all states)
- First-Visit Monte Carlo (with the initial value of zero for all state-action pairs)
- SARSA (with the initial value of zero for all state-action pairs)
- Q-Learning
