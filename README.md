# Reinforcement Learning: An Applied Evaluation through Grid World and Random Walk Scenarios

This repository contains implementations of reinforcement learning algorithms applied to two specific problems: navigating a grid world and performing a random walk on a 7x7 grid. The project includes code, results, and analysis to evaluate the performance of these techniques.

## Assignment Description

### Grid World Problem

The agent starts at the blue square and moves to a neighboring state with equal probability. If the agent moves to a red state, it receives a reward of -20 and goes back to the start, i.e., the blue square. A move between any two other states receives a reward of -1. A move that attempts to move outside of the grid receives a reward of -1. The black squares serve as terminal states. The goal is to pass through the opening in the red “wall” and reach one of the black squares to terminate the episode.

![Grid World](./1.png)

### Random Walk on a 7x7 Grid

The agent starts at the center of the grid and is equally likely to move up, down, left, or right. The lower left and upper right corners are terminal states with rewards -1 and 1, respectively. All other transitions receive a reward of 0. Attempts to move outside the grid result in the agent staying in place with a reward of 0.

## Implemented Algorithms

1. **Grid World**:
   - **SARSA**: On-policy TD control algorithm to estimate the Q-values and plot the resulting trajectory.
   - **Q-Learning**: Off-policy TD control algorithm to estimate the Q-values and plot the resulting trajectory.

2. **Random Walk**:
   - **Gradient Monte Carlo Method**: Computes the value function for the random walk policy.
   - **Semi-Gradient TD(0) Method**: Uses an affine function approximation to compute the value function.

## Project Structure

- `LICENSE`: License for the project.
- `README.md`: This file.
- `R_L_A3.ipynb`: Jupyter notebook containing the implementation of the assignment.
- `Reinforcement Learning Assignment 3.pdf`: The original assignment description.
- `1.png`: The grid world image included in the assignment description.

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/mrw-soumik/Reinforcement-Learning-An-Applied-Evaluation-through-Grid-World-and-Random-Walk-Scenarios.git
   cd Reinforcement-Learning-An-Applied-Evaluation-through-Grid-World-and-Random-Walk-Scenarios
   ```

2. **Open the Colab Notebook**:
   You can run the code directly in Google Colab by following [this link](https://colab.research.google.com/drive/1NW05u7otnbaNKk0g3d51fJ99NvK_9m1s?usp=sharing).

3. **Install Dependencies**:
   Ensure you have Python 3 installed. Install the required libraries:
   ```bash
   pip install numpy matplotlib
   ```

4. **Run the Notebook**:
   Open `R_L_A3.ipynb` in Jupyter Notebook or Jupyter Lab and run the cells to execute the code and generate the results.

## Results

The repository includes plots and analysis of the trajectories and reward trends for the SARSA and Q-Learning algorithms in the grid world, as well as the value function estimations for the random walk problem.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or additional features.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Feel free to make any further adjustments as needed.
