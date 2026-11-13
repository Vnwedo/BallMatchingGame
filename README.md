# 4x4 Tally Match

A two-player strategic grid game built with vanilla HTML, CSS, and JavaScript. Unlike standard Tic-Tac-Toe, the match continues until all 16 squares are filled, with players competing to accumulate the highest point total.

## How to Play
* Players take turns placing **Red** (Player 1) and **Blue** (Player 2) pieces onto a 4×4 grid.
* Once all 16 spaces are occupied, the player with the most points wins.

### Scoring Rules
* **3-in-a-row** (horizontal, vertical, or diagonal): **20 points**
* **4-in-a-row** (horizontal, vertical, or main diagonal): **40 points**
* **Rule Variants:** Toggle between *Replace Mode* (a 4-in-a-row awards 40 pts total) and *Stack Mode* (a 4-in-a-row awards 40 pts plus 20 pts for each of its two inner 3-ball segments).

## Strategy & Game Theory
Exhaustive minimax analysis of the 4×4 state space shows that optimal play from both sides results in a **0-point tie**:
* The **four center squares** intersect the highest number of 3- and 4-tile paths.
* If Player 1 opens in the center, Player 2 must immediately claim one of the remaining center squares—otherwise, Player 1 can force a **+40 point** advantage.

## Getting Started
1. Clone the repository:
   ```bash
   git clone [https://github.com/Vnwedo/4x4-tally-match.git](https://github.com/Vnwedo/4x4-tally-match.git)