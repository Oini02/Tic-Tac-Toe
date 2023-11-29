# Tic-Tac-Toe
Tic Tac Toe game for two players.

Board Representation:

The game board is represented as a 3x3 grid using a 2D vector of characters (vector<vector<char>>).
The initial state of the board is filled with empty spaces (' ').
Functions:

printBoard:

This function takes the current state of the board and prints it to the console in a user-friendly format.
checkWin:

Checks if the specified player has won the game.
Iterates through rows and columns, checking for three consecutive symbols of the same player.
Also checks both diagonals for a win.
isBoardFull:

Checks if the board is completely filled, indicating a tie.
It iterates through each cell; if any cell is empty, the board is not full.
makeMove:

Allows a player to make a move on the board by specifying the row and column.
Checks if the chosen cell is empty before placing the player's symbol.
If the chosen cell is already taken, it prompts the player to try again.
Main Game Loop (main function):

Initializes the game board and sets the starting player as 'X'.
Enters a loop that continues until the game is won or ends in a tie.
In each iteration:
The current state of the board is displayed using the printBoard function.
The current player is prompted to enter their move (row and column).
Input validation is performed to ensure the entered values are within the valid range.
The move is made using the makeMove function.
The code checks if the current player has won using the checkWin function.
If a win is detected, it displays a message and exits the loop.
The code checks if the board is full (a tie) using the isBoardFull function.
If the board is full, it displays a tie message and exits the loop.
