# JavaScript Mini Projects Collection

## 📖 Overview
Welcome to the JavaScript Mini Projects Collection! This repository contains a variety of beginner-to-intermediate web applications built using HTML, CSS, and Vanilla JavaScript. These projects are designed to demonstrate core web development concepts, including DOM manipulation, event handling, mathematics in JS, asynchronous operations, and modern styling techniques.

Below is a detailed explanation of every project included in this repository.

---

## 📁 File Structure

```text
JavaScript Mini Projects/
├── background_images/           # Images used for backgrounds (e.g., Digital Clock)
├── dice_images/                 # Images of dice faces (1-6) for the Dice Roller
├── weather_style.css            # External stylesheet for the Weather App
├── Calculator.html              # Calculator project
├── Counter.html                 # Counter project
├── Dice Roller.html             # Dice Roller project
├── Digital clock.html           # Digital Clock project
├── Interest Calculator.html     # Interest Calculator project
├── Number Guessing Game.html    # Number Guessing Game project
├── Radius of a Circle.html      # Radius Calculator project
├── Random Number Genarator.html # Random Number tool
├── Random Password Generator.html# Password Generator tool
├── Rock Paper Scissors Game.html# Rock Paper Scissors game
├── Stopwatch.html               # Stopwatch project
├── Temperature Conversion.html  # Temperature Converter
├── Weather App.html             # Weather App project
└── README.md                    # This documentation file
```

---

## 📂 Projects Breakdown

### ☁️ 1. Weather App (`Weather App.html`)
A dynamic application that fetches real-time weather data for any city globally.
*   **Features:** Displays temperature (Celsius), humidity, weather descriptions, and matching emojis.
*   **How it works:** It uses the **Open-Meteo Geocoding API** to convert city names to coordinates, and the **Open-Meteo Weather API** to fetch the weather without requiring a personal API Key. It handles errors gracefully if a city isn't found.
*   **Key Concepts:** Async/Await, `fetch()` API, DOM parsing, JSON data handling, CSS Flexbox & Linear Gradients.

  <img width="340" height="439" alt="image" src="https://github.com/user-attachments/assets/840b3633-5e00-4265-aebf-003713c09231" />

### 🔢 2. Calculator (`Calculator.html`)
A fully functional on-screen calculator.
*   **Features:** Basic arithmetic operations (addition, subtraction, multiplication, division), decimal support, and a clear (C) button.
*   **How it works:** Uses a grid layout for the buttons. Clicking a button appends the value to a read-only input display. The `=` button uses JavaScript's built-in `eval()` function to calculate the result safely within a `try...catch` block.
*   **Key Concepts:** CSS Grid, event handling (`onclick`), `eval()` function, error handling.

  <img width="326" height="442" alt="image" src="https://github.com/user-attachments/assets/47b1b7f7-47f4-4246-b7e8-2d467c9f1e68" />

### ⏱️ 3. Stopwatch (`Stopwatch.html`)
A precise digital stopwatch.
*   **Features:** Start, Stop, and Reset functionality, displaying Hours, Minutes, Seconds, and Milliseconds.
*   **How it works:** Uses `Date.now()` to track elapsed time accurately instead of relying solely on `setInterval` delays, ensuring precision even if the browser lags.
*   **Key Concepts:** `setInterval`, `clearInterval`, `Date.now()`, String padding (`padStart`), time mathematics.

  <img width="380" height="292" alt="image" src="https://github.com/user-attachments/assets/5671fd2c-de23-4b36-b34b-030d5ce51fbe" />

### 🕒 4. Digital Clock (`Digital clock.html`)
A beautiful transparency-styled live digital clock.
*   **Features:** 12-hour format display with AM/PM indicators updating every second. Features a glassmorphism (frosted glass) background effect.
*   **How it works:** Uses the `Date` object to get the current system time and updates the DOM every second.
*   **Key Concepts:** `Date` object methods (`getHours`, `getMinutes`, `getSeconds`), `setInterval`, CSS `backdrop-filter`.

  <img width="504" height="444" alt="image" src="https://github.com/user-attachments/assets/548b94f6-d7a0-47d2-bbd6-2d9250eebcd9" />

### 🎲 5. Dice Roller (`Dice Roller.html`)
A visual dice rolling simulator.
*   **Features:** Lets the user choose how many dice to roll (1 or more) and displays both the numerical results and visual dice images.
*   **How it works:** Collects the number input, runs a `for` loop to generate random numbers between 1 and 6, and dynamically constructs image elements pointing to local dice images (`dice_images/`).
*   **Key Concepts:** `Math.random()`, arrays (`push`, `join`), `innerHTML`, `for` loops.

  <img width="281" height="309" alt="image" src="https://github.com/user-attachments/assets/0b2a8804-ac27-46a8-8ac9-b4af41be7662" />

### rps 6. Rock Paper Scissors Game (`Rock Paper Scissors Game.html`)
The classic game against a computer opponent.
*   **Features:** Emoji-based buttons for input, real-time win/loss/tie evaluation, and score tracking for both the player and the computer. Color-coded results (green for win, red for loss).
*   **How it works:** The computer randomly selects an item from an array. A series of `if/else` and `switch` statements determine the winner, and CSS classes are dynamically added/removed to style the result text.
*   **Key Concepts:** Arrays, `Math.random()`, `switch` statements, `classList` (`add`, `remove`).

  <img width="418" height="344" alt="image" src="https://github.com/user-attachments/assets/29c55b1e-12b8-46b0-91d0-158ee56a761f" />

### ➕ 7. Counter (`Counter.html`)
A simple number incrementer/decrementer.
*   **Features:** Three buttons to Increment (+1), Decrement (-1), or Reset (back to 0) a large central number.
*   **How it works:** Maintains a `count` variable that is updated based on button clicks and immediately reflected in the DOM.
*   **Key Concepts:** Variables, basic arithmetic, `addEventListener`, DOM text updates.

  <img width="305" height="174" alt="image" src="https://github.com/user-attachments/assets/3628a604-b05d-41a6-947b-af6621139e66" />

### 💰 8. Interest Calculator (`Interest Calculator.html`)
A basic compound interest calculator.
*   **Features:** Inputs for Principal Amount, Interest Rate, and Years, calculating the final total formatted as USD currency.
*   **How it works:** Takes input values, sanitizes them (handles negatives or empty inputs), and applies the compound interest formula: `A = P * (1 + r/n)^(nt)`.
*   **Key Concepts:** Number validation (`isNaN`), `Math.pow()`, `Number.toLocaleString()` for currency formatting.

  <img width="319" height="377" alt="image" src="https://github.com/user-attachments/assets/42c7772a-35bf-4a01-894a-72a45f29825c" />

### 🌡️ 9. Temperature Conversion (`Temperature Conversion.html`)
Converts temperatures between Celsius and Fahrenheit.
*   **Features:** A text input for the temperature value and radio buttons to select the conversion direction (C to F, or F to C).
*   **How it works:** Checks which radio button `.checked` property is true, applies the appropriate mathematical formula, and displays the result rounded to one decimal place.
*   **Key Concepts:** Radio buttons state checking, basic algebra, `.toFixed()`.

  <img width="235" height="284" alt="image" src="https://github.com/user-attachments/assets/f20df511-8780-4e67-9363-163a7c07ebee" />

### 📏 10. Radius of a Circle (`Radius of a Circle.html`)
Calculates the properties of a circle.
*   **Features:** Takes a radius input and outputs both the Area and the Circumference.
*   **How it works:** Uses mathematical constants and powers to calculate the results. Handles invalid inputs (zero or text).
*   **Key Concepts:** `Math.PI`, `Math.pow()`, input validation.

  <img width="232" height="100" alt="image" src="https://github.com/user-attachments/assets/fc16f605-8f24-4047-8cce-5961c8b63292" />

### ❓ 11. Number Guessing Game (`Number Guessing Game.html`)
A browser prompt-based game.
*   **Features:** Uses `window.prompt` and `window.alert` for a simple pop-up game interface where the user tries to guess a number between 1 and 100.
*   **How it works:** Generates a random answer and uses a `while` loop to keep asking for guesses until the user gets it right, tracking the number of attempts.
*   **Key Concepts:** `window.prompt`, `window.alert`, `while` loops, conditional logic.

  <img width="340" height="148" alt="image" src="https://github.com/user-attachments/assets/5f147c3c-1b45-4d9c-b2f5-40c62489b9e2" />

### 🎲 12. Random Number Generator (`Random Number Genarator.html`)
A very basic random number tool.
*   **Features:** A single button that rolls a random number between 1 and 100 and displays it on screen.
*   **Key Concepts:** `Math.random()`, `Math.floor()`.

  <img width="146" height="104" alt="image" src="https://github.com/user-attachments/assets/92106b89-4cdd-4082-99db-d1ec206f5e74" />

### 🔐 13. Random Password Generator (`Random Password Generator.html`)
A customizable strong password creation tool.
*   **Features:** *Currently implemented as a console-only script.* It generates a password based on desired length and included character types (lowercase, uppercase, numbers, symbols).
*   **How it works:** Builds a string of allowed characters based on true/false flags, then randomly selects characters from that string in a loop until the desired length is reached.
*   **Key Concepts:** Functions with multiple parameters, string concatenation, loops.

  <img width="483" height="77" alt="image" src="https://github.com/user-attachments/assets/debe33e3-c24e-49b7-a531-db402a1505c7" />

---

## 💻 How to Run
All projects are Vanilla HTML/CSS/JS. To run any of them:
1. Clone or download this repository.
2. Double-click any `.html` file to open it directly in your web browser. No server setup is required!

---

## ✍️ Author
### Vijayapandian T
