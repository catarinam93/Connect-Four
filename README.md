# Connect-Four
Second assignment of the course Artificial Intelligence (2nd year, 2nd semester)

## A little context
### Overview
This assignment involves designing and implementing a program capable of playing Connect Four against a human opponent. Connect Four is a two-player strategy game similar to tic-tac-toe, where players take turns dropping tokens into a vertical grid with the goal of aligning four tokens in a row, column, or diagonal.

### Functionality
The program allows a human player to play against the computer, which uses one of two algorithms, minimax or alpha-beta, to make its moves. After each move by the human player, the computer analyzes the current board state and selects the best move based on the chosen algorithm. The game continues until one player wins or the board is full.

#### Input Format
The input to the program is provided through the interface, where the human player selects their move by entering the column number where they want to drop their token.

#### Output Format
The output of the program is displayed through the interface, showing the current state of the game board after each move, as well as prompts for the human player to make their move.

### Interface
The interface for the game displays the current state imitating the real game. Everything was made on pygame.

### Algorithms
The goal of this assignment is to implement the minimax, alpha-beta, and Monte Carlo Tree Search (MCTS) algorithms for the computer player. These algorithms analyze the game tree to determine the best move for the computer player based on the current board state.

### Evaluation Function
To evaluate the game state and determine the best move, the program uses a simple evaluation function based on the rules described next. This function assigns values to different game states based on the presence of aligned tokens and potential winning positions.
* -50 for three Os, no Xs,
* -10 for two Os, no Xs,
* - 1 for one O, no Xs,
* 0 for no tokens, or mixed Xs and Os,
* 1 for one X, no Os,
* 10 for two Xs, no Os,
* 50 for three Xs, no Os.
Note: Os and Xs represent the blue and red pieces, not specifically in this order, it will depend on the player you choose to be the first.

### Implementation Details
The program is implemented in Python and utilizes object-oriented programming principles to represent the game state, player actions, and algorithms.

## Usage
To play the game, simply run the program and click on the space you want you piece to move to. Atention: you can only play to legal places (the ones indicated by a with circunference). The computer will respond with its moves based on the algorithm you chose, if you chose to play against a human, the next play should proceed the same way as you did.
