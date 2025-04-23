Tic Tac Toe Game Logic
This is a classic 2-player Tic Tac Toe game implemented using HTML, CSS, and JavaScript. The game allows two players to take turns marking cells in a 3×3 grid, with the first player using "0" and the second using "X".

🧠 Game Logic Overview
Initial Setup:

The game board is a 3×3 grid made up of clickable boxes.

The variable turn0 is used to track the current player. It is true when it's Player 0's turn and false for Player X.

Player Turn Handling:

On each click:

The clicked box is filled with "0" or "X" based on the current player's turn.

The box is disabled to prevent overwriting.

The turn is switched to the next player.

The game checks for a winner after every move.

Winning Logic:

A list of winning patterns is defined using index combinations of the boxes (winPatterns).

After each move, the script checks all patterns to see if any match the same non-empty value (i.e., "0" or "X").

If a winning pattern is found, the game:

Displays a congratulatory message.

Disables all boxes to stop further moves.

Game Reset:

Clicking the "New Game" or "Reset" button resets the game:

Clears all box contents.

Re-enables all boxes.

Hides the winning message.

Resets the turn to Player 0.

🔄 Functions Used
checkWinner(): Scans for a winning combination.

showWinner(winner): Displays the winning message and disables the board.

enableBoxes(): Allows all boxes to be clicked.

disableBoxes(): Prevents any further moves after the game ends.

resetGame(): Resets the game to its initial state.
