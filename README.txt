# Java Mystery Escape

An interactive text-based escape room game written in Java, featuring multiple rooms, polymorphic puzzle types, custom exceptions, hints, and a persistent high-score manager.

## Features
* **Polymorphic Puzzles:** Includes word riddles, number/sequence problems, and Java-specific technical questions (`RiddlePuzzle`, `NumberPuzzle`, `CodeLockPuzzle`) inheriting from an abstract `Puzzle` base class.
* **Dynamic Levels:** Progress through 3 distinct rooms (Study Room, Old Library, and Secret Vault) with decreasing attempt counts and increasing difficulty[cite: 1].
* **Clue Tracking & Door Codes:** Solve all puzzles in a room to collect clue digits in order, then combine them to unlock the room door[cite: 1].
* **In-Game Commands:** Type `hint` (costs points), `clues` (lists collected clues), or `quit` at any time[cite: 1].
* **High Scores:** Automatically saves and loads the top 5 scores using local file handling (`ScoreManager`)[cite: 1].

## Project Structure
* `Main.java` - Entry point that launches the game[cite: 1].
* `Game.java` - Core game loop, level generation, and command handler[cite: 1].
* `Player.java` - Manages player name, score, hints used, and inventory[cite: 1].
* `Room.java` - Manages room details, puzzles, and door lock verification[cite: 1].
* `Puzzle.java` - Abstract base class defining shared puzzle logic[cite: 1].
* `RiddlePuzzle.java`, `NumberPuzzle.java`, `CodeLockPuzzle.java` - Specific puzzle implementations[cite: 1].
* `Hintable.java` - Interface for entities that provide hints[cite: 1].
* `GameOverException.java`, `InvalidAnswerException.java` - Custom checked exceptions for game flow and input validation[cite: 1].
* `ScoreManager.java` - Handles loading, sorting, and saving top scores to text[cite: 1].

## How to Compile and Run

1. Open your terminal or command prompt and navigate to the folder containing all the source files[cite: 1].
2. Compile all Java files together[cite: 1]:
   ```bash
   javac *.java
