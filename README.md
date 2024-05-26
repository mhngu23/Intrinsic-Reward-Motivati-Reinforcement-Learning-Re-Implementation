# Intrinsic Reward Motivation Reinforcement Learning Re-Implementation

This repository contains re-implementations of popular intrinsic reward motivation approaches in Reinforcement Learning (RL). These methods aim to enhance exploration by rewarding the agent for discovering novel or surprising states. The repository is organized into several Jupyter Notebooks, each dedicated to a specific intrinsic reward method.

## Notebooks Overview

### Memory for Novelty Based Exploration

1. **Count-Based Observation Bonus**
   - **Paper**: Tang, H., Houthooft, R., Foote, D., Stooke, A., Xi Chen, O., Duan, Y., ... & Abbeel, P. (2017). "# Exploration: A Study of Count-Based Exploration for Deep Reinforcement Learning". Advances in Neural Information Processing Systems, 30.
   - **Description**: This method uses a count-based approach to reward the agent for visiting less frequent states. A bonus is given to the agent based on the inverse of the visitation count of the current state.

2. **Episodic Curiosity through Reachability**
   - **Paper**: Savinov, N., Raichuk, A., Marinier, R., Vincent, D., Pollefeys, M., Lillicrap, T., & Gelly, S. (2018). "Episodic Curiosity through Reachability". arXiv preprint arXiv:1810.02274.
   - **Description**: This approach measures the agent's curiosity based on the reachability of states. The agent receives a higher reward for reaching states that are difficult to access from previously visited states.

### Memory for Surprise-driven Exploration

1. **Random Network Distillation (RND)**
   - **Paper**: Burda, Y., Edwards, H., Storkey, A., & Klimov, O. (2018). "Exploration by Random Network Distillation". arXiv preprint arXiv:1810.12894.
   - **Description**: In RND, a fixed random neural network is used to generate predictions. The difference between the predicted and actual output (prediction error) serves as the intrinsic reward, encouraging the agent to explore states that yield higher prediction errors.

2. **Curiosity-driven Exploration by Self-supervised Prediction**
   - **Paper**: Pathak, D., Agrawal, P., Efros, A. A., & Darrell, T. (2017, July). "Curiosity-driven Exploration by Self-supervised Prediction". In International Conference on Machine Learning (pp. 2778-2787). PMLR.
   - **Description**: This method incentivizes the agent to explore by predicting the consequences of its actions. The agent receives intrinsic rewards based on the error of its predictions, encouraging exploration of states where the model's predictions are less accurate.

### Advanced (Causal) Method for Exploration

1. **Causal Intrinsic Reward**
   - **Description**: This notebook implements a causal approach to intrinsic reward, where the agent is rewarded for actions that have a significant causal impact on its environment. This method aims to guide the agent towards actions that lead to meaningful and influential changes in the environment.

# References
1. Burda, Y., et al. (2018). "Exploration by Random Network Distillation". arXiv preprint arXiv:1810.12894.
2. Brockman, G., Cheung, V., Pettersson, L., Schneider, J., Schulman, J., Tang, J., & Zaremba, W. (2016). Openai gym. arXiv preprint arXiv:1606.01540.
3. Chevalier-Boisvert, M., Dai, B., Towers, M., Perez-Vicente, R., Willems, L., Lahlou, S., ... & Terry, J. (2024). Minigrid & miniworld: Modular & customizable reinforcement learning environments for goal-oriented tasks. Advances in Neural Information Processing Systems, 36.
4. Raffin, A., Hill, A., Gleave, A., Kanervisto, A., Ernestus, M., & Dormann, N. (2021). Stable-baselines3: Reliable reinforcement learning implementations. Journal of Machine Learning Research, 22(268), 1-8.
5. Huang, S., Dossa, R. F. J., Ye, C., Braga, J., Chakraborty, D., Mehta, K., & AraÃšjo, J. G. (2022). Cleanrl: High-quality single-file implementations of deep reinforcement learning algorithms. Journal of Machine Learning Research, 23(274), 1-18.
6. Pathak, D., et al. (2017). "Curiosity-driven Exploration by Self-supervised Prediction". In International Conference on Machine Learning (pp. 2778-2787). PMLR.
7. Savinov, N., et al. (2018). "Episodic Curiosity through Reachability". arXiv preprint arXiv:1810.02274.
8. Tang, H., et al. (2017). "# Exploration: A Study of Count-Based Exploration for Deep Reinforcement Learning". Advances in Neural Information Processing Systems, 30.


