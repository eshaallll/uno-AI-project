# UNO Game AI – Adversarial Search Simulation
 Simulation Link: https://drive.google.com/file/d/1NwT4Mruw_qf3hy7E_KazLmzEUaelQ0FD/view?usp=drive_link
---


## 🎯 Project Overview
This project is a high-fidelity UNO game simulation featuring three distinct players governed by specialized AI strategies. It demonstrates the application of **Minimax** and **Expectimax** algorithms in a stochastic environment with hidden information.

### Player Configurations
* **Player 1 (AI - Minimax):** Implements a **Defensive Strategy**. It assumes optimal opponent play to minimize the AI's risk, prioritizing "Skip" cards to defend against opponents close to winning.
* **Player 2 (AI - Expectimax):** Implements an **Offensive Strategy**. It models the draw pile as a **Chance Node**, calculating real-time probabilities based on the remaining deck to maximize card-shedding efficiency.
* **Player 3 (User/AI):** A dual-mode player. 
    * **Manual Mode:** Allows the user to interactively click cards to play.
    * **Simulation Mode:** Acts as an AI agent using Minimax logic.

---

## 🧠 AI & Evaluation Function
The "intelligence" of the agents is driven by a tuned evaluation formula:
$$Score = 50 - 5(C_{AI}) + 2(C_{opp}) + 3(S)$$

* **Minimax (Defensive):** Simulates 3 turns ahead, alternating between MAX (AI) and MIN (Opponent) nodes.
* **Expectimax (Offensive):** Uses actual deck ratios ($P = \text{playable} / \text{total}$) to determine the Expected Value of drawing a card.

---

## 🎨 GUI & Simulation (Bonus Features)
This submission includes a **Casino-themed GUI** developed in Tkinter, featuring:
* **Interactive Manual Play:** Users can click on beautiful, custom-designed cards to make moves.
* **Auto-Play Simulation:** A step-by-step automated mode for observing AI vs. AI interactions.
* **Real-time Game Log:** A "Thinking Log" that displays AI decisions and search scores.
* **Custom Assets:** Stylized card designs and a casino felt background.

---

## 🚀 How to Run
1. Clone this repository.
2. Ensure you have the `Pillow` library installed:  
   `pip install Pillow`
3. Ensure `casino.jpg` is in the same directory as the notebook.
4. Run all cells in `i242509-A02.ipynb`.

---

## 📁 Required Deliverables in Repo
* `i242509-A02.ipynb`: Main source code, Search Tree Demo, and Algorithm Comparison.
* `Search_Tree_Handwritten.jpg`: Handwritten design of the Minimax/Expectimax trees.
* `README.md`: Project documentation.
* `casino.jpg`: GUI background asset.
---
