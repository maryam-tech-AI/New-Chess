# Chess Game (pychess)

A simple, local chess game built with Python and Pygame. Play against another human locally or play against a basic AI powered by a Minimax search with alpha–beta pruning.

---

## Features
- Two-player local mode (hotseat).
- Play vs AI (Minimax with alpha–beta pruning, depth = 3).
- Full chess rules support (basic moves, castling, en passant, pawn promotion).
- Simple GUI using Pygame and piece artwork.

---

## Demo (screenshots)
Main menu, board, move hints, and game-end screens are included in the `project_images` folder and referenced below:

1. Main screen
![Main screen](https://raw.githubusercontent.com/ahmadrazakhawaja/chess-game-AI-project/master/project_images/Screenshot%202021-03-04%20at%206.16.22%20PM.png)

2. Starting position
![Starting position](https://raw.githubusercontent.com/ahmadrazakhawaja/chess-game-AI-project/master/project_images/Screenshot%202021-03-04%20at%2010.02.30%20PM.png)

3. Move hints (example)
![Move hints](https://raw.githubusercontent.com/ahmadrazakhawaja/chess-game-AI-project/master/project_images/Screenshot%202021-03-04%20at%2010.04.24%20PM.png)

4. Game end
![Game end](https://raw.githubusercontent.com/ahmadrazakhawaja/chess-game-AI-project/master/project_images/Screenshot%202021-03-04%20at%2010.08.36%20PM.png)

---

## Project Structure
- `playchess.py` — application entry point and main Pygame loop.
- `board/` — board representation and helper logic (`chessboard.py`, `move.py`, `tile.py`).
- `pieces/` — piece classes (`pawn.py`, `rook.py`, `knight.py`, `bishop.py`, `queen.py`, `king.py`, `nullpiece.py`, `piece.py`).
- `player/` — AI logic (`AI.py`).
- `chessart/` — piece images used by the GUI.

---

## Installation
1. Clone the repository:

```
git clone https://github.com/ahmadrazakhawaja/chess-game-AI-project.git
cd chess-game-AI-project
```

2. Install dependencies (recommend using a virtual environment):

```
pip install -r requirements.txt
```

If your environment uses `python3` as the interpreter command, replace `python` with `python3` when running the game.

---

## Usage
Run the game from the project root:

```
python playchess.py
```

Controls:
- Use the mouse to select pieces and make moves.
- From the main menu choose `AI` to play vs computer or `2 player` for local multiplayer.

---

## Notes about the AI
- The AI uses a depth-limited Minimax search (depth = 3) with alpha–beta pruning.
- The evaluation function values material and includes simple positional heuristics. It is intentionally lightweight for educational/demo purposes.
- Improvements: deeper search, move ordering, transposition table, and a stronger evaluation function would make the AI significantly stronger.

---

## Contributing
Contributions are welcome. If you want to improve the AI, GUI, or add features, please:

1. Fork the repository.
2. Create a new branch for your feature.
3. Open a pull request with a clear description of changes.

---

## Author
Maryam

---

If you'd like, I can:
- Update the image links to point to a different GitHub repository (for example your `maryam-tech-AI/Chess-Game`).
- Add a `requirements.txt` snippet or a small troubleshooting section.

See the main entry file: [playchess.py](playchess.py#L1).



