# Tic-Tac-Toe

A two-player Tic-Tac-Toe game that runs in a Jupyter notebook or a command-line
interface. Players take turns entering a board position, the board redraws after
each move, and the program announces a win or a tie.

## Demo

<video src="https://github.com/swathidbhat/starter-projects/raw/main/tic-tac-toe/tic-tac-toe-demo.mp4" controls width="600"></video>

If the video does not play above, [download or watch it here](tic-tac-toe-demo.mp4).

## Setup

Install Python 3, then pick one of the two ways to run the game.

### Run in a Jupyter notebook

1. Install Jupyter:

   ```bash
   pip install jupyter
   ```

2. Open the notebook:

   ```bash
   jupyter notebook Tic-Tac-Toe.ipynb
   ```

3. Run all cells from top to bottom.

### Run from the command line

1. Convert the notebook to a Python script:

   ```bash
   jupyter nbconvert --to script Tic-Tac-Toe.ipynb
   ```

2. Run the script:

   ```bash
   python Tic-Tac-Toe.py
   ```

The game reads your moves from the prompt and prints the board to the terminal.

## How to play

1. The board shows nine numbered cells:

   ```
   1|2|3
   4|5|6
   7|8|9
   ```

2. Two players share the keyboard and alternate turns. Player O moves first,
   then player X.
3. On your turn, type the number of the cell you want and press Enter. The
   program places your mark and redraws the board.
4. If you enter anything other than a number from 1 to 9, the program asks
   again.
5. The game ends when one player fills a row, column, or diagonal with their
   mark, or when all nine cells are full and no one has won. The program then
   prints the result.
