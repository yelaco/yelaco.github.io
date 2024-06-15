# [Devlog] Robinhood Chess #1  

## 13/06/2024

When I started writing this post, I had already completed 70% of the core game logic. So, I’ll begin by explaining what I've done so far.

I got some fundemental blocks for the game:

- ```board``` and ```spots``` structs. The chessboard consists of 64 spots, each representing a position that can either hold a piece or be empty.

![board_spot](/images/2024-06-13-robinhood_chess/board_spot.png)

- A ```move``` struct stores information about each move made by the players, including the starting and ending positions and other information.

![move](/images/2024-06-13-robinhood_chess/move.png) 

- A ```piece``` interface which can be implemented by concrete pieces like ```knight```, ```rook```, ```pawn```... The ```toUnicode()``` method is like ```toString()``` in Java to get the string representation to display on GUI later. 

![piece](/images/2024-06-13-robinhood_chess/piece.png)

- A ```game``` struct encapsulates the game logic and will be exported to other packages for use.

![game](/images/2024-06-13-robinhood_chess/game.png)


The full details of the source code will be on this [blog](https://minhquang053.github.io/2024/06/13/robinhood_chess.html). In the future, I will document my progress, detailing what I’ve accomplished each day, over a few days, or maybe weeks (if i get too busy).
