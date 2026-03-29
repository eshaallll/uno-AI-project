# UNO Game AI – Adversarial Search Simulation

**Name:** Eshaal Hussain  
**Roll No:** 24i-2509  
**Assignment:** 02  

---

## 🎯 Project Overview
This project is a simplified UNO game simulation featuring three players governed by different AI strategies. It demonstrates the application of **Minimax** and **Expectimax** algorithms in a stochastic environment.

### Player Configurations
* **Player 1 (AI - Minimax):** Uses a **Defensive Strategy** to block opponents using "Skip" cards.
* **Player 2 (AI - Expectimax):** Uses an **Offensive Strategy**, calculating the probability of the draw deck to shed cards aggressively.
* **Player 3 (User/AI):** Supports **Manual Mode** for user play and **Simulation Mode** using Minimax logic.

---

## 🧠 AI & Evaluation Function
The core "intelligence" of the agents is based on the following evaluation formula:
$$Score = 50 - 5(C_{AI}) + 2(C_{opp}) + 3(S)$$

* **Minimax (Defensive):** Assumes opponents play to minimize the AI's score. Focuses on turn control.
* **Expectimax (Offensive):** Models the "Draw" action as a **Chance Node**, using the actual ratio of playable cards left in the deck to calculate Expected Value.

---

## 🛠️ Implementation Details
* **Search Depth:** Both algorithms look **3 moves ahead** to find the optimal card.
* **Rules:** Includes Color/Value matching, "Skip" card turn-skipping, and automatic drawing when no moves are available.
* **GUI (Bonus):** A stylized Tkinter interface with "Auto-Play" functionality and a real-time game log.

---

## 🚀 How to Run
1. Clone this repository.
2. Install dependencies: `pip install Pillow`.
3. Open `i242509-A02.ipynb` in Jupyter or VS Code and run all cells.
4. (Optional) Run the GUI cell to watch the AI simulation in real-time.

---

## 📁 Required Deliverables in Repo
* `i242509-A02.ipynb`: Main source code and algorithm comparisons.
* `Search_Tree_Handwritten.jpg`: Handwritten design of the Minimax/Expectimax trees.
* `README.md`: Project documentation and setup instructions.
