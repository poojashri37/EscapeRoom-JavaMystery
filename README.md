# 🔐 Java Mystery Escape

An interactive, text-based escape room game developed in **Java**. Solve puzzles, uncover hidden clues, and unlock doors to escape through three challenging rooms!

## 🎮 Features

- **Polymorphic Puzzles:** Three different puzzle types — `RiddlePuzzle`, `NumberPuzzle`, and `CodeLockPuzzle` — inherit from an abstract `Puzzle` base class.
- **Dynamic Levels:** Explore three rooms with increasing difficulty and decreasing attempts:
  - Study Room
  - Old Library
  - Secret Vault
- **Clue Tracking & Door Codes:** Solve all puzzles in each room to collect clue digits. Combine them in the correct order to unlock the door.
- **In-Game Commands:**
  - `hint` – Get a hint at the cost of points.
  - `clues` – View collected clue digits.
  - `quit` – Exit the game.
- **High Score System:** Automatically saves and loads the top 5 scores using file handling.
- **Custom Exception Handling:** Uses custom checked exceptions to handle invalid answers and game-over conditions.

## 📁 Project Structure

```text
Java-Mystery-Escape/
│
├── Main.java
├── Game.java
├── Player.java
├── Room.java
├── ScoreManager.java
│
├── Puzzle.java
├── RiddlePuzzle.java
├── NumberPuzzle.java
├── CodeLockPuzzle.java
│
├── Hintable.java
│
├── GameOverException.java
├── InvalidAnswerException.java
│
└── README.md
```

## 🛠️ Concepts Used

This project demonstrates several core Java programming concepts:

- Object-Oriented Programming (OOP)
- Abstraction
- Inheritance
- Polymorphism
- Interfaces
- Exception Handling
- File Handling
- Collections and Sorting
- Loops and Conditional Statements

## 🚀 How to Compile and Run

### Prerequisites
- Java Development Kit (JDK) installed.
- A terminal or command prompt.

### Steps

**1. Clone the repository**

```bash
git clone <your-repository-link>
```

**2. Navigate to the project directory**

```bash
cd Java-Mystery-Escape
```

**3. Compile all Java files**

```bash
javac *.java
```

**4. Run the game**

```bash
java Main
```

## 🏆 Objective

Escape all three rooms by solving puzzles, collecting clue digits, and unlocking each door. Use hints wisely, manage your attempts, and aim for the highest score!

---

**Developed with Java ☕**
