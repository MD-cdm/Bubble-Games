# Bubble Game Application

## Overview

The Bubble Game Application is a simple interactive game where users click on randomly generated bubbles displayed on the screen. The user's goal is to click on bubbles that match the **"Hit"** value and score as many points as possible. The game is a **timer-based challenge**, requiring players to achieve the highest score within 60 seconds.

## Features

- **Dynamic Bubble Generation**: Bubbles are generated with random numbers each time.
- **Timer Countdown**: The game lasts for 60 seconds with a countdown timer.
- **Score System**: Clicking the correct bubble adds **+10 points** to the score.
- **Game Over Message**: The game stops when the timer reaches zero, displaying "Game Over."
- **Responsive UI**: Uses CSS and JavaScript for a visually appealing interface.

---

## File Structure

```
Bubble-Game-Application/
│── index.html  # Main HTML structure
│── style.css   # Styling of the game
│── script.js   # Game logic using JavaScript
│── README.md   # Project Documentation
```

---

## How to Run the Game

1. Open the project folder on your system.
2. Open **index.html** in any web browser (Google Chrome recommended).
3. The game will start, and the 60-second timer countdown will begin.
4. Click on bubbles that match the "Hit" value to increase your score.
5. When the timer reaches zero, the "Game Over" message will be displayed.

---

## Code Explanation

### 1. **HTML (index.html)**

- **`<div id="main">`**: The main container of the game.
- **`<div id="panel">`**: The panel containing game UI elements.
- **`<div id="ptop">`**: The top section displaying "Hit," "Timer," and "Score" values.
- **`<div id="pbtm">`**: The bottom section where bubbles are dynamically generated.

### 2. **CSS (style.css)**

- Uses gradients and box-shadow for a stylish background and panel design.
- **`.bubble`** class defines the appearance of the bubbles, making them circular with hover effects.

### 3. **JavaScript (script.js)**

#### **Variables & Functions:**

- **`var timer = 60;`** - Starts the timer at 60 seconds.
- **`var score = 0;`** - Initializes the score at 0 and increases when the correct bubble is clicked.
- **`var hitrn = 0;`** - Stores a random number that represents the "Hit" value.

#### **Functions Explanation:**

1. **`increaseScore()`** - Adds **+10** points when the correct bubble is clicked.
2. **`getNewHit()`** - Generates a new "Hit" number that users must match.
3. **`makeBubble()`** - Generates 168 bubbles with random numbers.
4. **`runTime()`** - Counts down the timer from 60 to 0 and displays "Game Over" when the time runs out.
5. **Click Event Listener (`#pbtm`)** - Detects clicks on bubbles and checks if the number matches the "Hit" value.
   - If it matches, the score increases, new bubbles are generated, and a new "Hit" value is set.
   - If it doesn't match, nothing happens.

---

## Possible Improvements

- **Difficulty Levels**: Adjusting the timer or bubble size to create different difficulty levels.
- **Sound Effects**: Adding sound effects for correct and incorrect clicks.
- **Leaderboard**: Implementing a system to store and display high scores.

---

## Conclusion

This is a **fun and interactive JavaScript-based game**, perfect for beginners to practice DOM manipulation and event handling. It can be further improved by adding new features and animations!

Happy Coding! 🚀

