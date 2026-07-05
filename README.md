# 🚀 RL Optimizers Project

A comparative study on the impact of optimization algorithms on **Deep Q-Network (DQN)** training in the **CartPole-v1** reinforcement learning environment.

This project was developed as part of the **Optimization Algorithms** course in the Master's Program in Artificial Intelligence (DSBD & IA), Hassan II University of Casablanca.

---

# 📖 Project Overview

The objective of this project is to analyze how different optimization algorithms influence the learning performance, convergence behavior, stability, and computational efficiency of a DQN agent.

To ensure a fair comparison, all experiments were conducted under identical conditions. The **optimizer** is the only parameter that changes between experiments.

---

# 🧠 Optimizers Compared

- SGD
- SGD with Momentum
- RMSprop
- Adam
- AdamW

---

# ⚙️ Experimental Setup

### Environment

- CartPole-v1 (Gymnasium)

### Deep Reinforcement Learning Algorithm

- Deep Q-Network (DQN)

### Neural Network

```
Input (4)
      │
      ▼
Dense (128) + ReLU
      │
      ▼
Dense (128) + ReLU
      │
      ▼
Output (2 Q-values)
```

### Hyperparameters

| Parameter | Value |
|----------|-------|
| Episodes | 500 |
| Batch Size | 64 |
| Learning Rate | 0.001 |
| Discount Factor (γ) | 0.99 |
| Replay Buffer | 10,000 |
| Target Network Update | Every 10 episodes |
| Random Seeds | 42, 123, 999 |

---

# 📊 Evaluation Metrics

The optimizers were evaluated using:

- Episode Reward
- Final Reward
- Maximum Reward
- Training Loss
- Training Time
- GPU Memory Usage
- Stability across multiple random seeds

---

# 📈 Main Results

- 🥇 **SGD** achieved the highest peak reward but showed the highest variance across runs.
- ⚖️ **SGD with Momentum** obtained the best final reward while maintaining good stability.
- ✅ **Adam** delivered the most consistent performance across different random seeds.
- ⚡ **RMSprop** provided a good balance between convergence speed and stability.
- 🔄 **AdamW** performed similarly to Adam but without a significant advantage in this study.

The experiments highlight that **no optimizer is universally superior**, emphasizing the trade-off between performance and reproducibility in reinforcement learning.

---

# 📂 Repository Contents

```
RL_Optimizers_Project/
│
├── rl-optimizer-comparison_Code.ipynb
├── rl-optimizer-comparison_Rapport.pdf
├── rl-optimizer-comparison_Presentation.pptx
└── README.md
```

---

# 🛠️ Technologies

- Python
- PyTorch
- Gymnasium
- NumPy
- Matplotlib
- CUDA GPU
- Kaggle Notebooks

---

# 👥 Authors

- Amina Bouazza
- Hafsa Elhilali
- Jihed El Betti

**Supervisor:** Pr. Faouzia Benabbou

---

*Master's Program in Artificial Intelligence  – Hassan II University of Casablanca (2025–2026).*
