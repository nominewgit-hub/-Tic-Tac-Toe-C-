# Tic Tac Toe (C++)
 
  A Tic-Tac-Toe board showing Xs and Os. Tic-Tac-Toe (also known as Noughts and Crosses) is a classic two-player game played on a 3×3 grid. Players alternate turns placing their mark (X or O) in an empty cell, aiming to align three of their symbols in a row, column, or diagonal to win. With optimal play by both sides, the game always ends in a draw. Because of its simple rules and state space, Tic-Tac-Toe is often used as a teaching example in programming and artificial intelligence. This repository provides a console-based C++ implementation of the game for Windows.

## Implementation Details
The game board is represented by a 3×3 character array (for example, char board) with cells initially labeled 1–9. A variable tracks the current player’s symbol ('X' or 'O'). 
The main loop of the program repeatedly displays the board, reads a player’s move (a number 1–9), updates the board, and checks for a win or draw. Win-checking is done by examining each row, each column, and the two diagonals for three identical symbols.
If a winning line is found, that player wins; if all cells fill without a win, the game is a draw. After each round, the program updates the score and can swap players for the next round. Windows-specific calls (like system("cls") and Sleep()) are used to clear the console and pause for animations.

## Features
•	Two-player mode: Two human players alternate turns. Players can enter custom names at the start of the game.
•	Score tracking: The game keeps track of each player’s wins across multiple rounds (and displays the current scores).
•	Restart/Swap: At any time during a round, entering r or R restarts the current game. Players can also choose to swap symbols between rounds while keeping the score.
•	Help menu: An instructions menu is available that explains the controls and rules.
•	Animated title/loading screen: Simple console animations or messages are shown during the start of the game and between rounds for effect.
•	Windows console effects: The program uses system("cls") to clear the screen and Sleep() (from <windows.h>) to add brief delays. These are Windows-specific functions.

## How to Play
1.	Compile and run:
 	g++ tickcross_.cpp -o tickcross_.exe
tickcross_.exe

2.	Main menu: After launching, you see the menu with options:
3.	1. How to play: Shows this instruction screen.
4.	2. Start game: Prompts for player names and begins a new round.
5.	3. Exit: Quits the program.
6.	During a round: Players alternate turns entering a grid position (1–9) to place their mark (Player 1 = X, Player 2 = O). Enter r or R to restart the round at any time. Enter e or E to exit to the main menu.
7.	End of round: When someone wins or the board is full, the game displays a win/draw message and updates the scores. Then you can choose to play again or exit.

## Controls
•	Grid positions (1–9): Enter the number corresponding to an empty cell to place your mark. The grid is numbered as follows (top row 1–3, middle 4–6, bottom 7–9).
•	Restart (r/R): Type r or R during your turn to restart the current round (clears the board and keeps scores).
•	Exit (e/E): Type e or E during your turn to abandon the current round and return to the main menu.

## Requirements
•	Windows OS: The game uses system("cls") and Sleep(), which are Windows-specific console functions. It should be run in a Windows command prompt.
•	C++ compiler: Any standard C++ compiler (for example, MinGW/G++ or Microsoft Visual C++) is needed to compile the source.
Build Instructions

1.	Open a terminal or command prompt in the project directory.

2.	Compile the source code:

 	g++ tickcross_.cpp -o tickcross_.exe

3.	Run the game:

 	tickcross_.exe

## File Structure
•	tickcross_.cpp – The main C++ source file containing the game logic.
•	README.md – This documentation file.
•	LICENSE – (Optional) Any license file. By default, there is no license.
•	.gitignore – (Optional) Git ignore file to exclude the compiled executable and other build artifacts.

## License
By default, this code is not under an open-source license, which means it remains “all rights reserved” by the author. The author has stated that the project is free for learning and educational use. To clarify reuse rights, you may choose to add a license (for example, the MIT License) if you wish to allow others to use or modify the code more freely.

## Author
Muhammad Noman 
Creator and author of this Tic-Tac-Toe game. 

-------

Enjoy playing and learning with this project!
________________________________________
