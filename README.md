# Ludo Dice Roller

A web-based, visually appealing 3D dice roller designed for Ludo and other board games, built entirely with HTML, CSS, and vanilla JavaScript. Supports a dynamic number of players.

## Features

* Smooth 3D dice rolling animation using CSS transforms.
* Standard Ludo dice pip (dot) layouts.
* **Dynamic Players:** Easily add or remove player sections using '+' and '-' buttons.
* **Editable Names:** Click on player names (e.g., "Player 1") to edit them directly.
* **Individual Controls:** Each player can set their desired number of dice (1-6).
* **Score Display:** Shows the total score for each roll per player.
* **Sound Effect:** Includes playback for a dice rolling sound (requires user setup).
* **Standalone:** No external libraries or frameworks needed. Runs directly in the browser.

## How to Use

1.  **Get the Code:**
    * Download the `index.html` file (or clone the entire repository).
2.  **(Optional) Get Sound:**
    * Find a dice rolling sound effect file (e.g., `.mp3`, `.wav`).
3.  **Configure Sound (IMPORTANT!):**
    * Open the `index.html` file in a text editor.
    * Find the `<audio>` tag near the bottom:
        ```html
        <audio id="dice-sound" src="path/to/your/dice-roll.mp3" preload="auto"></audio>
        ```
    * **Replace `"path/to/your/dice-roll.mp3"`** with the correct path to YOUR sound file.
        * If it's in the same folder: `src="dice-roll.mp3"`
        * If it's in a subfolder named `sounds`: `src="sounds/dice-roll.mp3"`
4.  **Open in Browser:**
    * Double-click the modified `index.html` file to open it in your web browser.
5.  **Play:**
    * Use the '+' and '-' buttons to set the number of players (1-8).
    * Click on "Player X" names to rename them.
    * Adjust the number of dice for each player using their input field.
    * Click the "Roll Dice" button for the desired player.

## How It Works

* **Structure:** Semantic HTML defines the layout for player areas and controls.
* **Styling:** CSS handles layout (Flexbox, Grid for pips), appearance, and 3D cube construction/animation (`perspective`, `transform-style: preserve-3d`, `@keyframes`).
* **Logic:** Vanilla JavaScript manages:
    * Adding/removing player elements dynamically.
    * Handling button clicks (using event delegation for roll buttons).
    * Simulating dice rolls (`Math.random`).
    * Updating scores and dice visuals.
    * Playing the sound effect.

## Contributing

Feel free to fork this repository, submit issues, or create pull requests if you have suggestions for improvements!

## License

This project is open source. Consider adding a license file (e.g., MIT License). *(Suggestion: Create a file named `LICENSE` and paste the MIT license text into it)*
