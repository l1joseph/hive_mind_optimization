# hive_mind_optimization

## Warehouse Location Optimizer using Particle Swarm Optimization

Implements a Particle Swarm Optimization algorithm to solve the problem of optimal warehouse placement. The goal is to find the best locations for a set number of warehouses, considering the positions of stores and residential areas.

## How It Works

1. **Initialization**: The algorithm creates a swarm of particles, each representing a potential solution.

2. **Fitness Evaluation**: Each particle's position is evaluated using a fitness function that considers:

   - Maximizing the minimum distance from residential areas
   - Minimizing the maximum distance to stores

3. **Optimization**: In each iteration, particles update their velocities and positions based on:

   - Their own best known position
   - The swarm's global best position
   - Inertia, memory, and social influence factors

4. **Convergence**: The process continues for a set number of iterations, gradually improving the solution.

## Customization

- Adjust the weights (`i_weight`, `m_weight`, `s_weight`) to change the behavior of the particles
- Modify the `fitness_function` in `particle_swarm.py` to change how solutions are evaluated
- Edit `plot_results.py` to customize the appearance of the output visualization
