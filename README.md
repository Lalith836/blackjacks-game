# 🃏 Blackjack Game in Python

A console-based Blackjack card game developed using **Python and Object-Oriented Programming (OOP)**. The game allows players to play multiple rounds of Blackjack against a dealer using a randomly shuffled deck.

## 📌 About the Project

This project is a beginner-friendly implementation of Blackjack designed to practice Python classes, objects, lists, dictionaries, loops, conditional statements, and randomization.

The game follows basic Blackjack rules, where the objective is to get as close to 21 as possible without exceeding it.

## ✨ Features

* 🃏 Creates a standard deck of 52 playing cards.
* 🔀 Shuffles the deck randomly before each game.
* 🎮 Allows the player to play multiple rounds.
* 👤 Supports player and dealer hands.
* 🏆 Detects Blackjack, busts, wins, and ties.
* 🎯 Supports `Hit` and `Stand` choices.
* 🤖 Dealer automatically draws cards until reaching a value of 17 or higher.
* 🙈 Hides one of the dealer's cards during gameplay.
* 🅰️ Supports Ace values of 1 or 11 when the hand exceeds 21.

## 🛠️ Technologies Used

* **Python 3**
* `random` module
* Object-Oriented Programming (OOP)

## 📂 Project Structure

```text
BLACKJACK/
│
├── blackjack.py
└── README.md
```

## 🧱 Classes Used

### 1. `card`

Represents an individual playing card.

**Attributes:**

* `suit` – The suit of the card.
* `rank` – A dictionary containing the card's rank and value.

### 2. `Deck`

Creates and manages a standard deck of 52 cards.

**Methods:**

* `shuffle()` – Randomly shuffles the deck.
* `deal(number)` – Deals the requested number of cards.

### 3. `Hand`

Represents the player's or dealer's hand.

**Methods:**

* `add_card()` – Adds cards to the hand.
* `calculate_value()` – Calculates the hand's total value.
* `get_value()` – Returns the current hand value.
* `is_blackjack()` – Checks whether the hand value is 21.
* `display()` – Displays the cards in the hand.

### 4. `Game`

Controls the overall game logic.

**Methods:**

* `play()` – Starts and manages multiple rounds.
* `check_winner()` – Checks for busts, Blackjack, wins, and ties.

## 🎮 How to Play

1. Run the Python program.
2. Enter the number of rounds you want to play.
3. The player and dealer receive two cards each.
4. Choose an action:

   * `Hit` or `H` – Draw another card.
   * `Stand` or `S` – Stop drawing cards.
5. The dealer draws cards until the hand value reaches at least 17.
6. The final results are displayed, and the winner is determined.

## 📜 Game Rules

* The goal is to get as close to 21 as possible without exceeding it.
* Number cards have their face value.
* J, Q, and K are worth 10 points.
* An Ace is initially worth 11 points and is reduced to 1 if the hand exceeds 21.
* A hand exceeding 21 is called a **bust**.
* A Blackjack is a hand with a value of 21 according to the program's rules.
* The dealer draws cards while the hand value is below 17.
* The player with the higher valid score wins.

## 🚀 How to Run the Project

### Step 1: Clone the repository

```bash
git clone https://github.com/your-username/blackjack.git
```

### Step 2: Open the project folder

```bash
cd blackjack
```

### Step 3: Run the program

```bash
python blackjack.py
```

## 💻 Example Gameplay

```text
how many games do you want to play ? 2

******************************
1 of 2
******************************
your hand
A of spades
10 of hearts
value: 21

dealers hand
hidden
7 of clubs

you have a blackjack you win!

******************************
2 of 2
******************************
your hand
8 of diamonds
5 of clubs
value: 13

dealers hand
hidden
10 of spades

please choose 'hit' or 'stand' : hit

your hand
8 of diamonds
5 of clubs
4 of hearts
value: 17

please choose 'hit' or 'stand' : stand
```

*Note: The gameplay output is an illustrative example.*

## 📚 Concepts Learned

* Classes and objects in Python
* Constructors using `__init__()`
* Instance methods
* Lists and dictionaries
* Nested loops
* Conditional statements
* Exception handling
* Randomization using `random.shuffle()`
* Basic game development logic
* Working with multiple interacting classes

## 🔮 Future Improvements

* [ ] Add a graphical user interface (GUI).
* [ ] Add betting and virtual chips.
* [ ] Add score tracking across rounds.
* [ ] Improve Ace handling for hands containing multiple Aces.
* [ ] Add replay options.
* [ ] Add animations and sound effects.
* [ ] Add automated tests for game logic.

## 👨‍💻 Author

**Lalith Vardhan**

B.Tech Computer Science Engineering Student

---

⭐ If you enjoyed this project, consider giving the repository a star!
