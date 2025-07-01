# TigerStripes - AI for Engineers Project

This project explores reinforcement learning concepts using the Gymnasium library. It includes examples of environment interaction, agent training, and evaluation.

## Project Overview

The primary goal of this project is to demonstrate the fundamentals of reinforcement learning, including:

- Understanding reinforcement learning environments (action space, observation space, rewards).
- Interacting with environments programmatically.
- Training reinforcement learning agents using libraries like Stable-Baselines3.
- Evaluating the performance of trained agents.

The project currently includes a Jupyter Notebook (`TigerStripes.ipynb`) which contains the code and explanations for these concepts.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab

### Installation

1.  **Clone the repository (if applicable):**
    ```bash
    git clone <repository-url>
    cd <repository-name>
    ```
2.  **Install dependencies:**
    The necessary Python packages are listed in `TigerStripes.ipynb` and should be installed to run the notebook. A `requirements.txt` file will be added to streamline this process.

    ```bash
    pip install gymnasium ale-py pyvirtualdisplay matplotlib torch stable-baselines3[extra] swig gymnasium[box2d]
    ```
    *(Note: The installation commands are also present at the beginning of the `TigerStripes.ipynb` notebook.)*

### Running the Notebook

1.  Launch Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook
    # or
    jupyter lab
    ```
2.  Open the `TigerStripes.ipynb` notebook and run the cells sequentially.

## Project Structure

-   `TigerStripes.ipynb`: The main Jupyter Notebook containing the code, explanations, and examples.
-   `TigerStripes`: An empty file (its purpose is unclear and might be removed or repurposed).
-   `README.md`: This file, providing an overview of the project.
-   `video/`: Directory created by the notebook to store recorded videos of agent interactions.
-   `eval_logs/` & `eval_logs_lunarlander/`: Directories created by the notebook to store training logs and evaluation results.

## Key Concepts Demonstrated

-   **Environment Interaction:** Using `gymnasium` to create, reset, step through, and render environments like `ALE/Atlantis-v5` and `CartPole-v1`.
-   **Environment Properties:** Querying action space, observation space, maximum episode steps, and reward thresholds.
-   **Agent Training:** Utilizing `stable-baselines3` (specifically the DQN agent) to train an agent on the `CartPole-v1` and `LunarLander-v3` environments.
-   **Hyperparameter Tuning:** Defining and using a set of hyperparameters for the DQN agent.
-   **Callbacks:** Using `EvalCallback` and `StopTrainingOnRewardThreshold` to monitor training progress and save the best model.
-   **Agent Evaluation:** Evaluating the trained agent's performance using `evaluate_policy`.
-   **Visualization:** Plotting learning curves and recording videos of the agent's behavior.

## Future Improvements (Planned)

-   Add a `requirements.txt` file for easier dependency management.
-   Organize the project into a more standard Python project structure (e.g., `src` directory for scripts, `notebooks` directory).
-   Add more detailed comments and docstrings to the code within the notebook.
-   Explore other reinforcement learning agents and environments.
-   Refine hyperparameters for better agent performance.

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## License

(To be added - consider an open-source license like MIT or Apache 2.0 if appropriate)
