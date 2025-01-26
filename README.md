# CowBull-Word-Guessing-Game
CowBull is a fun and interactive word guessing game, built with a combination of HTML, CSS, Vanilla JavaScript, Node.js, Express, Webpack, and Babel. The game challenges players to guess a secret word within a limited number of attempts. The secret word is generated randomly, and the player receives feedback on each guess, represented as cows (correct letters in the wrong position) and bulls (correct letters in the correct position).

This project demonstrates the integration of both front-end and back-end technologies, where the front-end provides an engaging user interface and the back-end handles the generation of words and validation of guesses.

## Key Features:
* Word Guessing: Players guess a secret word by entering letters into a grid.
* Feedback System: Feedback is provided in the form of "cows" and "bulls" to help players adjust their guesses.
* Responsive Layout: The game is fully responsive, making it playable on both desktop and mobile devices.
* Dynamic Word Generation: Words are generated dynamically via external APIs to provide a new challenge each time.
* Virtual Keyboard: Users can interact with the game using either a physical or a virtual on-screen keyboard.
* Game Rules Reference: The game includes a built-in rules modal for quick reference.

This project leverages Webpack for module bundling and Babel to ensure compatibility across modern browsers. The back-end, powered by Node.js and Express, manages API calls for word generation and validation, ensuring a seamless and dynamic gameplay experience.

## Demo
Here are screenshots from the CowBull game page:

### Screenshots


<div align="center">
  <p><strong>Game Page</strong></p>
  <img src="/screenshots/homepage.PNG" alt="Game Page" width="500">
</div>
<br>



<div align="center">
  <p><strong>Game Options Display</strong></p>
  <img src="/screenshots/game-options-display.PNG" alt="Game Options Display" width="500">
</div>
<br>


<div align="center">
  <p><strong>Game Guessing Grid with Virtual Keyboard and Result Display</strong></p>
  <img src="/screenshots/guessing-grid.PNG" alt="Game Guessing Grid with virtual keyboard and result display" width="500">
</div>
<br>


<div align="center">
  <p><strong>Game Grid Page</strong></p>
  <img src="/screenshots/game-grid.PNG" alt="Game Grid Page" width="500">
</div>
<br>


<div align="center">
  <p><strong>Game Rules Reference Display</strong></p>
  <img src="/screenshots/game-rules-display.PNG" alt="Game Rules Reference Display" width="500">
</div>
<br>


<div align="center">
  <p><strong>Victory Display</strong></p>
  <img src="/screenshots/game-victory-display.PNG" alt="Victory Game Display" width="500">
</div>
<br>

## Installation

To run CowBull locally, follow these steps:

1. Clone the repository to your local machine.

   ```bash
   git clone 
   ```
2. Install the required dependencies.
   ```bash
   npm install
   ```
3. Create a .env file in the project root and add your API key for dictionary lookup. You can obtain an API key from [dictionaryapi.com](https://www.dictionaryapi.com/register/index).
   ```bash
   API_KEY=your-api-key-here
   ```
4. Start the development server.
   ```bash
   npm start
   ```
5. Open your web browser and visit http://localhost:3000 to play CowBull.

## How to Play
Welcome to CowBull, the word-guessing game!

1. Enter your guesses using either the virtual keyboard or your physical keyboard.
2. Submit your guess by clicking the Enter button.
3. Based on your guess:
    * **Cows** indicate correct letters in the wrong position.
    * **Bulls** indicate correct letters in the correct position.
4. Use the feedback to refine your guesses.
5. Guess the secret word before running out of attempts!

## API Usage
This project utilizes two APIs:

### Random Word API
The Random Word API is used to generate random words of a specific length. You can use the following URL to request a random word:
https://random-word-api.herokuapp.com/word?number=1&length={wordLength}

### Dictionary API
The Dictionary API is used to check if a word is valid and in the dictionary. You should obtain an API key from dictionaryapi.com and store it in your .env file as API_KEY.
