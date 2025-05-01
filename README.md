# 🎰 Terminal Slot Machine Game (JavaScript)

This is a simple **command-line slot machine game** built with **JavaScript** (Node.js). It simulates a 3x3 slot machine where users can deposit money, place bets across multiple lines, and spin to win based on matching symbols. The game continues until the user either chooses to stop or runs out of money.

---

## Features

- 💰 Deposit system to fund your game session
- 🎯 Bet on 1 to 3 lines
- 🎲 Randomized 3x3 slot machine spin
- 🏆 Winnings calculated based on matching rows
- 🔁 Play again option until you run out of money

---

## Game Logic

The game follows these steps:
1. Prompt user to **deposit money**
2. Ask how many **lines** to bet on (1-3)
3. Prompt for **bet amount per line**
4. **Spin** the slot machine with randomly chosen symbols
5. **Check for wins** (all 3 symbols in a line match)
6. Calculate and **credit winnings**
7. Ask to **play again**

---

## Technologies Used

- JavaScript (ES6)
- Node.js
- [`prompt-sync`](https://www.npmjs.com/package/prompt-sync) for synchronous input handling

---

## Setup Instructions

### Prerequisites

- [Node.js](https://nodejs.org/en/) installed

### Installation

1. Clone the repository or copy the files:
   ```bash
   git clone <repository-url>
   cd slot-machine
   ```

2. Install dependencies:
   ```bash
   npm install prompt-sync
   ```

3. Run the game:
   ```bash
   node index.js
   ```

---

## Example Gameplay

```bash
Enter a deposit amount: 50
Enter the number of lines to be on (1-3): 3
Enter the bet per line: 5
A | A | A
C | D | B
B | C | D
You won, $75
Do you want to play again (y/n)? y
...
```

---

## 🎰 Symbol Details

| Symbol | Frequency | Value Multiplier |
|--------|-----------|------------------|
| A      | 2         | 5x               |
| B      | 4         | 4x               |
| C      | 6         | 3x               |
| D      | 8         | 2x               |

The game ensures a weighted probability for each symbol based on their frequency.

---

## File Structure

```
slot-machine/
│
├── index.js           # Main game logic
├── package.json       # NPM configuration for prompt-sync
└── README.md          # Project documentation
```

---
