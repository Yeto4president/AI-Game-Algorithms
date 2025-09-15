# 🎮 AI Game Algorithms: Tic-Tac-Toe and Connect 4

<div align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?logo=python" alt="Python version">
  <img src="https://img.shields.io/badge/License-MIT-green" alt="License">
  <img src="https://img.shields.io/badge/Status-Production-brightgreen" alt="Status">
</div>

## 📖 Overview
Implementation of Minimax algorithm with Alpha-Beta pruning for two classic strategy games.

## ✨ Features
### Core Algorithms
- **Minimax** decision-making
- **Alpha-Beta pruning** optimization
- **Heuristic evaluation** functions
- **Depth-limited search**

### Game Specifics
| Feature               | Tic-Tac-Toe       | Connect 4         |
|-----------------------|------------------|------------------|
| Board Size            | 3×3              | 6×12             |
| Win Condition         | 3 in a row       | 4 in a row       |
| Max Decision Time     | < 1s             | ≤ 9s             |
| Search Depth          | 6 ply            | 3 ply            |

### 🕹️ Game Controls

---

**Quick Start:**
1. **Choose first player** - Human or AI at launch
2. **Enter moves** - Simple format depending on the game

| Game | Input Format     | Valid Range |
|------|-----------------|-------------|
| Tic-Tac-Toe | `row,column` | 0-2 |
| Connect 4   | `column`     | 0-11 |

> 💡 *Example for Tic-Tac-Toe: `1,2` for row 1, column 2*

---

### 🏆 Performance Metrics

<div align="center">

| Metric | Tic-Tac-Toe | Connect 4 |
|--------|------------|-----------|
| **Win Rate** | 100% | ~85% |
| **Decision Time** | < 100ms | 5-8s |
| **Search Depth** | 6 ply | 3 ply |
| **Terminal States** | 9 squares | 42 pieces |

</div>

---

### 🛠 Technical Implementation

#### 🔧 Key Functions
```python
minimax_ab()          # Main algorithm with pruning
evaluate_position()   # Heuristic evaluation
Terminal_Test()       # End-of-game detection
get_valid_moves()     # Generate valid moves
Roadmap items
```
### ⚡ Connect 4 Optimizations
- 🎯 Immediate detection - Win/lose in 1 move
- 🎯 Center bonus +3 points for central control
- 🎯 Pattern recognition - Threat detection
- 🛡️ Defensive weighting ×1.2 for opponent threats
