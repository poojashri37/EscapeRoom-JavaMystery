<h1>Java Mystery Escape</h1>

<p>An interactive text-based escape room game written in Java, featuring multiple rooms, polymorphic puzzle types, custom exceptions, hints, and a persistent high-score manager.</p>

<hr>

<h2>Features</h2>

<ul>
    <li><strong>Polymorphic Puzzles:</strong> Includes word riddles, number/sequence problems, and Java-specific technical questions (<code>RiddlePuzzle</code>, <code>NumberPuzzle</code>, <code>CodeLockPuzzle</code>) inheriting from an abstract <code>Puzzle</code> base class[cite: 1].</li>
    <li><strong>Dynamic Levels:</strong> Progress through 3 distinct rooms (Study Room, Old Library, and Secret Vault) with decreasing attempt counts and increasing difficulty[cite: 1].</li>
    <li><strong>Clue Tracking & Door Codes:</strong> Solve all puzzles in a room to collect clue digits in order, then combine them to unlock the room door[cite: 1].</li>
    <li><strong>In-Game Commands:</strong> Type <code>hint</code> (costs points), <code>clues</code> (lists collected clues), or <code>quit</code> at any time[cite: 1].</li>
    <li><strong>High Scores:</strong> Automatically saves and loads the top 5 scores using local file handling (<code>ScoreManager</code>)[cite: 1].</li>
</ul>

<hr>

<h2>Project Structure</h2>

<h3>Core Logic & Execution</h3>
<ul>
    <li><strong><code>Main.java</code></strong> - Entry point that launches the game[cite: 1].</li>
    <li><strong><code>Game.java</code></strong> - Core game loop, level generation, and command handler[cite: 1].</li>
</ul>

<h3>Entities & Data</h3>
<ul>
    <li><strong><code>Player.java</code></strong> - Manages player name, score, hints used, and inventory[cite: 1].</li>
    <li><strong><code>Room.java</code></strong> - Manages room details, puzzles, and door lock verification[cite: 1].</li>
    <li><strong><code>ScoreManager.java</code></strong> - Handles loading, sorting, and saving top scores to text[cite: 1].</li>
</ul>

<h3>Puzzles & Interfaces</h3>
<ul>
    <li><strong><code>Puzzle.java</code></strong> - Abstract base class defining shared puzzle logic[cite: 1].</li>
    <li><strong><code>RiddlePuzzle.java</code></strong> - Word riddle implementation[cite: 1].</li>
    <li><strong><code>NumberPuzzle.java</code></strong> - Math and sequence puzzle implementation[cite: 1].</li>
    <li><strong><code>CodeLockPuzzle.java</code></strong> - Java technical question implementation[cite: 1].</li>
    <li><strong><code>Hintable.java</code></strong> - Interface for entities that provide hints[cite: 1].</li>
</ul>

<h3>Exception Handling</h3>
<ul>
    <li><strong><code>GameOverException.java</code></strong> - Custom checked exception for game over / quit conditions[cite: 1].</li>
    <li><strong><code>InvalidAnswerException.java</code></strong> - Custom checked exception for malformed user inputs[cite: 1].</li>
</ul>

<hr>

<h2>How to Compile and Run</h2>

<ol>
    <li>Open your terminal or command prompt and navigate to the folder containing all the source files[cite: 1].</li>
    <li>Compile all Java files together[cite: 1]:
        <pre><code>javac *.java</code></pre>
    </li>
    <li>Run the game using the <code>Main</code> class[cite: 1]:
        <pre><code>java Main</code></pre>
    </li>
</ol>
