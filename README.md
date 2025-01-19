### README for "Q-Learning Process Optimization"

---

# Q-Learning Implementation for Process Optimization

This project demonstrates a Q-Learning implementation to optimize routes between locations in a predefined environment. It uses the principles of reinforcement learning to determine the shortest path between locations while considering rewards for each state transition.

## Features
- **Environment Definition**: States, actions, and reward matrices define the system's environment.
- **Reinforcement Learning**: Implements the Q-Learning algorithm to learn and optimize routes.
- **Shortest Route Calculation**: Calculates the shortest route between a starting location, intermediary location, and ending location.

## Getting Started

### Prerequisites
- Python 3.x
- Numpy library (`pip install numpy`)

### Installation
1. Clone the repository:  
   ```bash
   git clone <repository_url>
   ```
2. Navigate to the project directory:
   ```bash
   cd q-learning-process-optimization
   ```
3. Run the script:
   ```bash
   python q_learning_optimization.py
   ```

## Usage

1. Define your starting, intermediary, and ending locations.
2. Use the `best_route` function to calculate the optimal route:
   ```python
   print(best_route('E', 'K', 'G'))
   ```
3. Modify the reward matrix (`R`) to represent different environments as needed.

## Example
To calculate the optimal route from location `E` to `K` to `G`:
```python
print(best_route('E', 'K', 'G'))
```
Output:
```
Route:
['E', 'I', 'J', 'K', 'G']
```

## How It Works
1. **Q-Learning Algorithm**:  
   - Randomly explores the environment.
   - Updates the Q-Table using the Temporal Difference (TD) formula.
2. **Route Calculation**:  
   - Starts from the initial state.
   - Iteratively selects the next state with the highest Q-value until reaching the destination.

## Customization
- Adjust `gamma` (discount factor) and `alpha` (learning rate) to fine-tune the learning process.
- Modify the reward matrix (`R`) to represent different environments.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

