
# Trajectory Planning for Autonomous Vehicles Using Hierarchical Reinforcement Learning (HRL)

## Overview

This project implements a full end-to-end framework for trajectory planning in autonomous vehicles, focusing on lane changes under noisy observation conditions. The framework employs **Hierarchical Reinforcement Learning (HRL)** to enhance decision-making, allowing vehicles to choose optimal actions based on environmental conditions and long-term goals.

---

## Features
- **Hierarchical Decision Making:** The model splits decisions into higher-level goals and low-level actions for improved efficiency in complex environments.
- **Lane Change Simulation:** Simulates autonomous vehicle lane changes under varying traffic conditions and noisy sensor observations.
- **Adaptability:** The HRL framework adapts to diverse scenarios, such as congested roads or sudden obstacles.
- **Noisy Observations:** Handles real-world issues like sensor inaccuracies and environmental noise.

---

## Prerequisites

- Python 3.x
- Required Libraries:
  - TensorFlow
  - NumPy
  - OpenAI Gym (for simulation)
  - Matplotlib (for visualizations)

---

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/kalebbennaveed/Trajectory-Planning-for-Autonomous-Vehicles-Using-HRL.git
   cd Trajectory-Planning-for-Autonomous-Vehicles-Using-HRL
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up the Simulation Environment:**
   Install OpenAI Gym if not already installed:
   ```bash
   pip install gym
   ```

---

## Usage

After installation, you can run the simulation and observe how the HRL algorithm controls lane changes in a noisy environment.

To run the main simulation script:
```bash
python run_simulation.py
```

### Configuration
- To adjust the simulation parameters (e.g., traffic density, noise level), modify the `config.json` file.
- The configuration includes:
  - Number of lanes
  - Traffic intensity
  - Noise levels for sensors
  - Simulation duration

### Output
The simulation will output:
- The autonomous vehicle's trajectory over time
- Evaluation metrics such as the success rate of lane changes, decision time, and overall safety

---

## Visualization

To visualize the vehicle’s trajectory and decision-making process, run:
```bash
python visualization.py
```
The visual output will provide a graphical representation of the vehicle's path, lane changes, and environmental dynamics.

---

## Contributing

We welcome contributions to improve the codebase and documentation. To contribute:
1. **Fork the repository.**
2. **Create a new branch for your feature:**
   ```bash
   git checkout -b feature-branch
   ```
3. **Make your changes and commit them:**
   ```bash
   git commit -m "Description of changes"
   ```
4. **Push to your branch:**
   ```bash
   git push origin feature-branch
   ```
5. **Submit a pull request.**

For detailed guidelines, see `CONTRIBUTING.md`.

---

## Citation

If you use this code in your research or work, please cite the following paper:
- **[Trajectory Planning for Autonomous Vehicles Using Hierarchical Reinforcement Learning](https://ieeexplore.ieee.org/document/XXXXX)**

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Future Improvements

- **Model Extensions:** Include more complex driving scenarios such as intersection management or roundabouts.
- **Additional Sensors:** Implement LiDAR and radar simulations to better mimic real-world sensor setups.
- **Real-world Testing:** Adapt the algorithm for real-world autonomous vehicles beyond simulation.
