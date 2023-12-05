### GameState  -  GameState class implements  game logic and  rules.   #### Features  - `board': Object of the ChessRepository class, which manages the  board and  pieces.   #### Methods  - `make_move(move)`: makes a move on the board.  - `back(board, pieces)`: Returns the board and  pieces to their previous state.  - `get_board()`: Returns a ChessRepository object.  - `get_legal_moves(start)`: returns the legal moves of the button on the start screen. - `possible_moves()`: returns all  possible moves of the current player.  - `play_random_move([moves])`: Plays a random legal move from a list of moves, otherwise it first gets a list of all  possible moves and then plays a random move from that list.  - `get_value()`: returns the value of the current position. The value is positive if white wins and negative if black wins. - `get_result()`: returns the game result. It can be either "1" (white wins), "0" (black wins), "0.5" (tie) or "nothing" (game  not over).  - "is_insufficient_material()": Returns "True" if the game is tied due to insufficient material, and returns "False" otherwise.  - `fen()`: returns the FEN string of the current location. - "game_over()": Returns "True" if the game is over and "False" otherwise.

#### Example
```python
chess_repository = ChessRepository()
chess_repository.initialize_board()
game_state = GameState(chess_repository)
print(game_state.get_value())
# Output: 0

print(game_state.get_legal_moves("d2")
# Output: [(2, 3), (3, 3)]

game_state.make_move("d2d4")
print(game_state.get_board())
# Output: A ChessRepository object with the board after the move
```
