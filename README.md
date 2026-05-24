# Assembly: Endgame (TS + Vite)

# Assembly Endgame

Assembly Endgame is a fun word guessing game built with React and TypeScript.  
The player must guess the hidden word one letter at a time before all programming languages are eliminated.

## Features

- Interactive on-screen keyboard
- Random word generation
- Win and lose game states
- Farewell messages for lost languages
- Confetti animation when winning
- Disabled keyboard after game over
- Tracks wrong guesses
- Responsive UI design

## Technologies Used

- React
- JavaScript / TypeScript
- CSS
- Vite

## Project Learning Steps

1. Project Planning  
2. Header Section  
3. Status Section  
4. Languages List  
5. Word Display  
6. Keyboard  
7. Save the guessed letters  
8. Keyboard letter styles for guesses  
9. Only display correctly guessed letters  
10. Wrong guess count  
11. Lost languages  
12. isGameOver logic  
13. Display won/lost status  
14. Farewell messages  
15. Disable keyboard when game is over  
16. Random word generation  
17. New game reset button  
18. Missed letters display  
19. Confetti animation  
20. Accessibility improvements  
21. Refactoring logic  
22. Utility functions  
23. Conditional rendering cleanup  
24. Final styling polish  
25. Final project completion



## Gameplay

1. When the page loads, the game randomly selects a `currentWord` to guess.
2. Click letters on the on-screen **keyboard**.
3. Your chosen letters are tracked in state.
4. Each wrong guess increases the number of failures.
5. The game ends when you either:
   - **Win**: all letters in the current word are guessed.
   - **Lose**: you reach the maximum allowed wrong guesses.

## What you see on screen

- **Header**: title and instructions.
- **Language chips** (`src/languages.js`): show progress/penalties as you get wrong.
- **Word display**: letters are revealed only when guessed (or after you lose).
- **Keyboard**: each letter button changes style based on whether it was guessed correctly or incorrectly.
- **Win/Lose end screen**:
  - Win shows a “You win!” message and triggers **confetti**.
  - Lose shows a “Game over!” message.
- **Farewell message**: when you’re close to losing and your last guess is wrong, the app displays a randomized message.

## How it works (key implementation ideas)

- Uses React hooks (`useState`) to store:
  - `currentWord`
  - guessed letters
- Uses derived values to compute:
  - wrong guess count
  - win/loss state
  - what letters to reveal
- Button click handlers update the guessed letters while preventing duplicate guesses.

## Output
![alt text](image.png)
![alt text](<Screenshot 2026-05-23 050321.png>)
![alt text](<Screenshot 2026-05-23 045800.png>)

## Getting started

```bash
npm install
npm run dev
```

Then open the URL shown by Vite (typically `http://localhost:5173`).

## Project scripts

Common scripts are defined in `package.json` (e.g., `dev`, `build`, `preview`).

