# AI Chess Game - README

## Overview
This project is a **Python-based chess game** featuring a graphical user interface and an AI opponent built with **Pygame**. Players control the white pieces, while the AI, set to **hard difficulty** by default, controls the black pieces. The AI uses a depth-based minimax algorithm with alpha-beta pruning achieving an estimated elo range of 500-600. Essential chess rules are implemented, including automatic promotion to a queen and castling.

## Features
1. **Graphical Interface:**  
   - Developed using Pygame, providing interactive piece movement.  
   - Highlights checks and displays endgame messages for checkmate, stalemate, or draw.

2. **AI Opponent:**  
   - Operates on a depth-based strategy using:  
     - **Piece-square tables** for positional advantages.  
     - **Transposition tables** for optimized evaluations.  
     - **Minimax algorithm** with alpha-beta pruning to identify the best moves.  
   - Operates at a depth of 4 moves, with an estimated Elo rating of **500–600**.  

3. **Chess Mechanics:**  
   - Implements **kingside castling** and **auto-promotion** to a queen.  
   - Detects **check**, **checkmate**, and **stalemates**.  

## Project Structure
- **`ai.py`**: Implements the AI, including move evaluation using piece-square tables, transposition tables, and minimax.  
- **`board.py`**: Manages the chessboard, including move validation, piece placement, and captures.  
- **`game.py`**: Coordinates game logic, player interactions, and visual updates.  
- **`main.py`**: Initializes and launches the game, creating the game window and running the game loop.  
- **`pieces.py`**: Defines chess pieces (Pawn, Rook, Knight, Bishop, Queen, King) and their movement rules.  

## Getting Started
### Prerequisites
- **Python 3.x**  
- **Pygame library**: Install using `pip install pygame`

### Cloning the Repository
To set up the project locally, use the following commands:
```bash
git clone https://github.com/jeyoo2005/ai_chess_engine
cd chess-engine
python main.py
