# RL-Policy-Evaluation-
RL-Policy Evaluation Using Monte Carlo Methods and Temporal Difference Methods

This project implements two reinforcement learning algorithms in a **Jupyter Notebook**:
1. **Monte Carlo Policy Evaluation** for the Blackjack environment.
2. **Temporal Difference Learning with SARSA** for the Cliff Walking environment.


## Project Overview

### 1. Monte Carlo Policy Evaluation in Blackjack
- **Objective**: Estimate the state-value function \( V(s) \) for a fixed policy in the Blackjack environment.
- **Environment**: OpenAI Gym's `Blackjack-v1`.
- **Policy**: "Stick if the player's sum \(\geq 18\), otherwise hit."
- **Deliverables**:
  - Heatmap of \( V(s) \) for each state (player's sum vs. dealer's visible card).
  - Convergence plot of \( V(s) \) for a specific state over episodes.

### 2. Temporal Difference Learning with SARSA in Cliff Walking
- **Objective**: Learn the optimal policy using the SARSA algorithm in the Cliff Walking environment.
- **Environment**: OpenAI Gym's `CliffWalking-v0`.
- **Policy**: ε-greedy exploration strategy.
- **Deliverables**:
  - Plot of cumulative reward per episode.
  - Visualization of the learned policy (arrows indicating actions in each state).

---

## Dependencies

To run this project, you need the following Python libraries:
- `gym` (for the environments)
- `numpy` (for numerical computations)
- `matplotlib` (for plotting)
- `seaborn` (for heatmap visualization)
- `jupyter` (for running the notebook)

You can install the dependencies using `pip`:
```bash
pip install gym numpy matplotlib seaborn jupyter
```

---

## Notebook Structure

The project is implemented in a single Jupyter Notebook:
- **`Reinforcement_Learning_Policy_Evaluation.ipynb`**:
  - Contains all the code for both Monte Carlo Policy Evaluation and SARSA in Cliff Walking.
  - Includes explanations, visualizations, and results.

---

## Running the Notebook

1. **Install Jupyter** (if not already installed):
   ```bash
   pip install jupyter
   ```

2. **Launch the Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

3. **Open the Notebook**:
   - Navigate to the project directory and open `Temporal Difference - Cliff Walking with SARSA.ipynb` or `Monte Carlo - Blackjack Policy Evaluation.ipynb`.

4. **Run the Notebook**:
   - Execute each cell in the notebook sequentially to reproduce the results.

---

## Results

### 1. Monte Carlo Policy Evaluation in Blackjack
- **Heatmap of \( V(s) \)**: Shows the estimated value function for each state (player's sum vs. dealer's visible card).
- **Convergence Plot**: Demonstrates how the value estimate for a specific state converges over episodes.

### 2. Temporal Difference Learning with SARSA in Cliff Walking
- **Cumulative Reward Plot**: Shows the agent's learning progress over episodes.
- **Learned Policy Visualization**: Displays the optimal actions in each state as arrows on a grid.

---

## Key Learning Points

### 1. Monte Carlo Policy Evaluation
- **Episodic Tasks**: MC methods require complete episodes to compute returns.
- **Policy Impact**: The choice of policy significantly affects the value function \( V(s) \).
- **Visualization**: Heatmaps and convergence plots are essential for analyzing the results.

### 2. Temporal Difference Learning with SARSA
- **On-policy TD Control**: SARSA learns the value function for the policy it is following.
- **Exploration vs. Exploitation**: The ε-greedy strategy balances exploration and exploitation.
- **Efficiency**: SARSA is more sample-efficient than MC methods for episodic tasks.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Author

- **Mahlet Nigussie Tesfaye**
- Addis Ababa Institute of Technology, SITE
- Email: rigbe.rmn@gmail.com
- Date: February 16, 2024
