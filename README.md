# Markov Chain Simulation Package

This Python package provides a comprehensive framework for simulating and analyzing Markov chains. It includes tools for creating transition matrices, simulating chains, calculating steady-state distributions, analyzing absorption probabilities, and visualizing results.

## Key Features

- **Transition Matrix Creation**: Allows users to define or generate random stochastic matrices.
- **Markov Chain Simulation**: Simulates chains from given initial states and transition matrices.
- **Steady-State Distribution Calculation**: Computes the steady-state distribution of a Markov chain.
- **Absorption Probability Analysis**: Calculates absorption probabilities for chains with absorbing states.
- **Visualization Tools**: Offers functions to plot transition matrices and simulate chain states over time.
- **Menu-Driven Interface**: Provides an interactive menu for users to explore different aspects of Markov chain analysis.

## Installation

To use this package, ensure you have Python installed along with the necessary libraries:

pip install numpy matplotlib seaborn


## Usage

1. Load the necessary libraries and data.
2. Run the `main` function to interact with the package's features.


## Menu Options

The menu-driven interface offers the following options:

1. **Simulate Markov Chain**: Simulates a chain from a given initial state and transition matrix.
2. **Generate Random Stochastic Matrix**: Creates a random stochastic matrix of a specified size.
3. **Plot Transition Matrix**: Visualizes a transition matrix using a heatmap.
4. **Calculate Steady-State Distribution**: Computes the steady-state distribution of a Markov chain.
5. **Analyze Absorption Probabilities**: Calculates absorption probabilities for chains with absorbing states.
6. **Simulate Multiple Chains**: Simulates multiple chains from different initial states.
7. **Analyze Convergence to Steady-State**: Plots the convergence of a Markov chain to its steady-state distribution.
8. **Compute Mean First Passage Times**: Calculates mean first passage times for a Markov chain.
9. **Exit**: Exits the menu.

## Contributing

Contributions are welcome! Please submit pull requests or issues to improve the package.

## License

This package is licensed under the MIT License.

## Acknowledgments

This package utilizes `numpy`, `matplotlib`, and `seaborn` for numerical computations and visualizations.

---

### Example Use Cases

- **Analyzing Chain Behavior**: Use the menu options to explore how different initial states and transition matrices affect chain behavior.
- **Predicting Absorption Probabilities**: Train and evaluate absorption probabilities for chains with absorbing states.

### Known Issues

- Ensure that all necessary dependencies are installed before running the package.
- The package assumes that the transition matrix is correctly formatted and does not handle incorrect input formats.

### Future Development

- Expand the model to include additional types of Markov chains (e.g., continuous-time Markov chains).
- Integrate real-time data for more accurate simulations.

### Code Structure

The code is structured around a `MarkovChain` class that encapsulates the core functionality of the package. The `main` function provides a menu-driven interface for users to interact with the package.

### API Documentation

#### MarkovChain Class

- `__init__(transition_matrix)`: Initializes a Markov chain with a given transition matrix.
- `is_stochastic()`: Checks if the transition matrix is stochastic.
- `next_state(current_state)`: Returns the next state given the current state.
- `simulate(initial_state, num_steps)`: Simulates the Markov chain for a given number of steps.
- `steady_state_distribution()`: Calculates the steady-state distribution of the Markov chain.
- `absorption_probabilities()`: Calculates absorption probabilities if there are absorbing states.

#### Utility Functions

- `generate_random_stochastic_matrix(size)`: Generates a random stochastic matrix of a given size.
- `plot_transition_matrix(transition_matrix)`: Visualizes a transition matrix using a heatmap.
- `simulate_multiple_chains(transition_matrix, initial_states, num_steps)`: Simulates multiple Markov chains from different initial states.
- `analyze_convergence(transition_matrix, initial_distribution, max_steps=1000)`: Analyzes the convergence to the steady-state distribution over time.
- `mean_first_passage_time(transition_matrix)`: Computes mean first passage times using the fundamental matrix.

### Troubleshooting

- **Input Errors**: Ensure that all inputs are valid integers or matrices.
- **Dependency Issues**: Verify that all required libraries are installed.

### Contact

For questions or suggestions, please open an issue on this repository.

