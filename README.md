# Tic-Tac-Toe

### Tic-Tac-Toe Game Using Python and Tkinter

This project is a simple **Tic-Tac-Toe** game built using Python and the **Tkinter** library for the graphical user interface. The game allows two players to play on a 3x3 grid, taking turns to place their symbols (X or O) until one player wins or the game ends in a tie.

#### Key Features:
1. **Graphical User Interface**: The game board is created using Tkinter's `Canvas` widget, with clear lines dividing the grid into 3 rows and 3 columns.
2. **Interactive Gameplay**: Players can interact with the game by clicking on the grid to place their mark. X and O symbols are drawn in different colors.
3. **Score Tracking**: After each round, the scores of both players and ties are displayed on the canvas.
4. **Game Logic**:
   - Players alternate between placing X and O.
   - The game automatically checks for winning conditions (three in a row, column, or diagonal) or a tie after each move.
5. **Play Again**: Once a game ends, players are prompted to click the screen to play again, and the board resets for a new round.

#### How the Game Works:
- The game starts with Player 1 (X), and the turns alternate between Player 1 (X) and Player 2 (O).
- Players place their marks by clicking on an empty cell in the grid.
- The game checks for a winner or tie after every move.
- If a player wins, the game displays the winner and updates the score. In case of a tie, the game declares a tie and updates the tie score.
- Players can click to reset the board and play another round.

#### Code Structure:
- **Game Initialization**: The `Tic_Tac_Toe` class initializes the game window, creates the grid, and manages the game state.
- **Board Drawing**: The `initialize_board()` function sets up the grid lines, and the `draw_X()` and `draw_O()` functions handle the drawing of symbols on the canvas.
- **Game Logic**: The game checks for a win or tie using the `is_winner()` and `is_tie()` functions. If the game ends, the `display_gameover()` function is called to display the result and scores.
- **Event Handling**: Mouse clicks are handled through the `click()` method, which places the symbol in the clicked grid and updates the game state.

