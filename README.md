# A barebones implementation of the PPO algorithm

NOTE: The training is unstable and does not always manage to converge within a reasonable amount of time.
If it appears stuck, restarting the training might be a good idea.
On a good run it should solve the environment in about 300-400 episodes.

The model is trained every 5 episodes for 30 training iterations.
The process will terminate if the agent has achieved 500 reward for the previous 20 episodes or if it reaches 1000 total episodes.
GAE is used for calculating the advantages.
