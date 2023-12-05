### ChessRepository - The pieces and game board are managed by the ChessRepository class.

#### Properties
- {board}: The game board is represented by a 2D array. Every element in the array is either {None} or a piece object.
- {pieces}: An inventory of every piece on the board.
- {history}: A rundown of every move made during the game.
- {turn}: A string designating who is taking the turn. It might be {w} or {b}.
- {half_moves}: An integer representing how many half moves have been made since the previous pawn or capture move.
- {number_of_moves}: An integer representing the total number of moves made during the game.
- {game_over}: A boolean indicating whether or not the game has ended.
#### Example
```python
chess_repository = ChessRepository()
chess_repository.initialize_board()
print(chess_repository.board)
# Output: [[wR,   wN,   wB,   wQ,   wK,   wB,   wN,   wR  ],
#          [wP,   wP,   wP,   wP,   wP,   wP,   wP,   wP  ],
#          [None, None, None, None, None, None, None, None],
#          [None, None, None, None, None, None, None, None],
#          [None, None, None, None, None, None, None, None],
#          [None, None, None, None, None, None, None, None],
#          [bP,   bP,   bP,   bP,   bP,   bP,   bP,   bP  ],
#          [bR,   bN,   bB,   bQ,   bK,   bB,   bN,   bR  ]]

print(chess_repository.fen())
# Output: rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - 0 1

chess_repository.remove_piece(chess_repository.board[0][0])
print(chess_repository.board)
# Output: [[None, wN,   wB,   wQ,   wK,   wB,   wN,   wR  ],
#          [wP,   wP,   wP,   wP,   wP,   wP,   wP,   wP  ],
#          [None, None, None, None, None, None, None, None],
#          [None, None, None, None, None, None, None, None],
#          [None, None, None, None, None, None, None, None],
#          [None, None, None, None, None, None, None, None],
#          [bP,   bP,   bP,   bP,   bP,   bP,   bP,   bP  ],
#          [bR,   bN,   bB,   bQ,   bK,   bB,   bN,   bR  ]]
```
