# Number Guessing Game

A small interactive number guessing game written in Python. The computer picks a secret number and you try to guess it. After every wrong guess you get hints, and your score goes down, so try to guess in as few attempts as possible.

It runs in Google Colab and uses buttons and a dropdown (no typing in the console).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NoorFatima77/number-guessing-game/blob/main/number_guessing_game.ipynb)

## How the game works

1. Choose a difficulty from the dropdown:
   - **Easy:** a number between 1 and 10
   - **Hard:** a number between 1 and 100
2. Click **Start Game**. The computer picks a secret number.
3. Type your guess in the box and click **Submit Guess**.
4. If the guess is wrong, you lose 15 points (you start with 100) and see:
   - how far your guess is from the secret number
   - a hint whether the secret number is greater or smaller than your guess
   - a hint that the secret number is divisible by a certain number (when it is divisible by one of 2 to 9)
5. If you guess correctly, the game shows your final score and the number of attempts.
6. If your score drops to 0 or below, the game is over and the secret number is revealed.

## Features

- Two difficulty levels
- Score system (100 points, minus 15 for every wrong guess)
- Distance, greater/smaller and divisibility hints
- Check that the guess is inside the allowed range
- Button-based interface built with `ipywidgets`

## Tools used

Python, `random`, `ipywidgets`, `IPython.display`, Google Colab

## How to run

1. Click the **Open in Colab** badge above (or upload `number_guessing_game.ipynb` to Google Colab).
2. Run the cell.
3. Pick a difficulty, click **Start Game**, and start guessing.

## Files in this repository

- `number_guessing_game.ipynb`: the game code
- `README.md`: this file

## Possible improvements

- Add a "Play Again" button
- Add a high score list
- Let the computer guess the number that the player thinks of
