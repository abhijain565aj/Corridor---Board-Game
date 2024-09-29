## Corridor - Board Game (2 Players)
The current working file is corridor.cpp, some other verisons with more features which I was trying are in other files.

To compile it and use the game, one needs the simplecpp library - provided to us as part of the CS101 course at IIT Bombay. The library includes support for elementary graphics


### **Game Overview**
Corridor is a two-player strategy board game played on a 9x9 grid. Each player aims to move their piece from their starting position on one side of the board to the opposite side. However, players can also place walls to block their opponent's progress, making it harder for the opponent to reach their goal.

The game is won when a player successfully moves their piece to any of the squares on the opponent's side of the board.

### **Game Components**
- **Board:** A 9x9 grid of squares.
- **Players:** 2 players.
- **Pieces:** Each player has one piece (denoted as Player 1 and Player 2).
- **Walls:** Each player starts with 10 walls. Each wall is 2 blocks long and can be placed between two squares to block movement.

### **Objective**
The objective is to be the first player to move your piece from your starting row to any square in the opponent's starting row (the opposite side of the board).

### **Game Setup**
- The board consists of a 9x9 grid.
- Player 1's piece starts on the middle square of the first row (position `(5, 1)`).
- Player 2's piece starts on the middle square of the last row (position `(5, 9)`).
- Each player starts with 10 walls that can be placed during the game to block the opponent.

### **Gameplay**
The game is turn-based. On each player's turn, they can either:

1. **Move their piece** to an adjacent square (up, down, left, or right), or
2. **Place a wall** to block their opponent's movement.

#### **Movement Rules:**
- Pieces move one square at a time.
- A player can move to any adjacent square (horizontally or vertically), unless a wall blocks the path.
- If both pieces are adjacent to each other and there’s no wall between them, the player can "jump" over the opponent’s piece.
- If a wall is behind the opponent's piece, the player can move to one of the squares adjacent to the opponent's piece.

#### **Placing Walls:**
- Walls are placed between two squares and must be exactly 2 blocks long (spanning the space between squares).
- A wall cannot completely block all possible paths to the opponent’s side of the board.
- Walls can be placed either horizontally or vertically.
- Once placed, walls cannot be moved or removed.

#### **Winning the Game:**
- The first player to move their piece to any square in the opponent's starting row wins the game.

### **Additional Rules:**
- Players can only place a wall if it does not completely block all paths for either player to reach their goal.
- Both players must always have a possible route to reach the other side, though it can be a long and complicated one.

### **Example Scenario:**
- Player 1 starts at position `(5, 1)`, and Player 2 starts at position `(5, 9)`.
- On Player 1's first turn, they can either move their piece to an adjacent square or place a wall.
- If Player 1 moves, Player 2 can respond by either moving their piece or placing a wall to block Player 1's progress.
- The game continues in this manner until one player reaches the other side of the board.

### **Strategy Tips:**
- Use your walls wisely! Placing a wall early can slow down your opponent, but you'll need to keep some walls for later in the game to protect your path.
- Focus on creating a clear path for your piece while simultaneously blocking your opponent's progress.
- Keep in mind that jumping over your opponent's piece can be a great way to advance quickly.

