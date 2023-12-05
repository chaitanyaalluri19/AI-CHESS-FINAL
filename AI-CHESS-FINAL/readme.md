Project Overview: This is a fully functional chess game implemented in Python. It allows users to play against a computer using different algorithms such as MCTS (Monte Carlo Tree Search) and Minimax. The project consists of several classes and modules:

1. ChessRepository: This class manages the chess board and pieces. Each piece in the game has its own unique class.

2. GameState: This class handles the rules and logic of the game.

3. MCTS: This class implements the Monte Carlo Tree Search algorithm for the AI player.

4. MCTSNode: This code represents a node in the MCTS tree.

5. Minimax: This class implements the Minimax algorithm for the AI player.

6. GUI: This class executes the graphical user interface for the game.

7. UI: This class implements the command line user interface for the game.

The base class for all chess pieces is called Piece. It is inherited by specific piece classes such as Pawn, Rook, Knight, Bishop, Queen, and King. Each piece class applies its own unique actions and behavior.

The project also includes a Convolutional Neural Network (CNN) class implemented in the ConvolutionalNeuralNetwork module. This class includes a TensorConverter that converts the chess board into a tensor representation.

Overall, this project provides a comprehensive implementation of a chess game with various AI algorithms and user interfaces.
