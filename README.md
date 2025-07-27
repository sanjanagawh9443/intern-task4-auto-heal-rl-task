# intern-task4-auto-heal-rl-task
Python-based Auto-Healing Agent and RL-based Fix Optimizer.

#  Task 4: Auto-Heal + RL Optimization Agent

This repo contains two Python agents:

1. **HealingPlanner (Agent 4)** – Simulates real-time healing from deployment errors.
2. **RLPlanner (Agent 5)** – Learns the best fix strategy using Reinforcement Learning logic.

---

## 📁 Files

| File Name         | Description                                      |
|------------------|--------------------------------------------------|
| `healing_log.csv` | Logs of errors, fix actions, and results        |
| `healing_planner.py` | Randomly applies fix actions to errors         |
| `rl_planner.py`      | Learns best fix for each error type           |

---

## ⚙️ How It Works

- **healing_planner.py** simulates errors and applies a fix (`retry_deploy`, `restore_version`, `adjust_threshold`)
- The results are stored in `healing_log.csv`
- **rl_planner.py** analyzes the log and recommends the best fix per error type

---

## 🚀 How to Run

```bash
# Step 1: Generate error-fix logs
python healing_planner.py

# Step 2: Learn best fixes from logs
python rl_planner.py






