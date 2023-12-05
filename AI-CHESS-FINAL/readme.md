Project overview: This is a Python-based, fully functional chess game that lets users play against a computer using different algorithms (MCTS and Minmax). It consists of the following: - A class for managing the chess board and pieces in a repository
  - A class called game state, which manages the logic of the game; - A class called MCTS, which executes the Monte Carlo Tree Search algorithm; - A class called Minimax, which executes the Minimax algorithm; - A class called GUI, which executes the graphical user interface
  - A CNN class that implements a convolutional neural network; - A UI class that implements the command line user interface.
  


- `ChessRepository: Manages the chess board and pieces; every piece in the game has a unique class.
- {GameState}: Puts rules and logic into action.
- {MCTS}: AI Monte Carlo Tree Search algorithm implementation.
  - {MCTSNode}: This code implements the MCTS tree's node.
- {Minimax}: AI implementation of the Minimax algorithm.
- {GUI}: Executes the graphical user interface framework.
- {UI}: This command line user interface is implemented.
The base class of all chess pieces is {Piece}.
  - {Pawn}: Takes over from Piece and applies Pawn's unique actions.
  - {Rook}: Takes over from Piece and applies the unique actions of Rook.
  - {Knight}: Takes over from Piece and applies Knight's unique behavior.
  - {Bishop}: Takes over from Piece and applies Bishop's unique actions.
  - {Queen}: Takes over from Piece and applies Queen's unique actions.
  - {King}: Takes over from Piece and applies King's unique actions.
Convolutional neural networks are implemented by the `ConvolutionalNeuralNetwork` module.
  Implements a class called `TensorConverter` that converts a chess board to a tensor

