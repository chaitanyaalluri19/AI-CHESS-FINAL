### Project overview
- This project is a fully functional chess game implemented in Python, that allows the users to play against a computer using various algorithms (MCTS and Minmax). It includes:
  - A chess repository class that manages the game board and the pieces
  - A game state class that handles the game logic
  - A MCTS class that implements the Monte Carlo Tree Search algorithm
  - A Minimax class that implements the Minimax algorithm
  - A GUI class that implements the graphical user interface
  - A UI class that implements the command line user interface
  - A CNN class that implements a convolutional neural network.
  


- `ChessRepository`: Handles the game board and pieces, each chess piece has its own class.
- `GameState`: Implements game logic and rules.
- `MCTS`: Implements Monte Carlo Tree Search algorithm for AI.
  - `MCTSNode`: Implements the node of the MCTS tree.
- `Minimax`: Implements Minimax algorithm for AI.
- `GUI`: Implements the graphical user interface.
- `UI`: Implements the command line user interface.
- `Piece`: Base class for all chess pieces.
  - `Pawn`: Inherits from Piece, implements Pawn's specific behavior.
  - `Rook`: Inherits from Piece, implements Rook's specific behavior.
  - `Knight`: Inherits from Piece, implements Knight's specific behavior.
  - `Bishop`: Inherits from Piece, implements Bishop's specific behavior.
  - `Queen`: Inherits from Piece, implements Queen's specific behavior.
  - `King`: Inherits from Piece, implements King's specific behavior.
- `ConvolutionalNeuralNetwork`: Implements a convolutional neural network.
  - `TensorConverter`: Implements a class that converts a chess board to a tensor.


- The Minimax algorithm on low depth tends to get stuck in local optimums, resulting in it playing the same move over and over again. For example, it might move the rook back and forth until the end of the game.
- The HashTable implementation for the Minimax algorithm is not working properly, so it is not used in the current version of the project.
- The CNN has a limited dataset, therefore it is not as accurate as it could be.