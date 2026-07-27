<div align="center">

# Tetris Game

### A console-based Tetris game built with C++ and object-oriented design

![C++](https://img.shields.io/badge/Language-C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![OOP](https://img.shields.io/badge/Design-Object--Oriented-informational)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)

</div>

## About the Project

A two-player Tetris game developed in C++ as an object-oriented programming project.

The game supports human and computer-controlled players, several game modes, independent boards, scoring, piece rotation, collision detection, and line clearing.

## Game Modes

- Human vs. Human
- Human vs. Computer
- Computer vs. Computer

The computer player is available in three difficulty levels: **Best**, **Good**, and **Novice**.

## Key Features

- Two independent game boards
- Keyboard-controlled and computer-controlled players
- Shape movement, rotation, and immediate drop
- Collision detection and completed-line removal
- Score tracking
- Pause and resume functionality
- Colored or monochrome display
- Heuristic-based computer decisions

## Object-Oriented Design

| Component | Responsibility |
|---|---|
| `Player` | Abstract base class shared by all player types |
| `Human` | Handles keyboard-controlled gameplay |
| `Computer` | Evaluates placements and performs automated moves |
| `Board` | Manages the board, collisions, and completed lines |
| `Shapes` | Handles Tetris pieces, movement, and rotation |
| `TetrisGame` | Controls the main game loop |
| `Menu` | Manages game modes and settings |

The `Human` and `Computer` classes inherit from `Player` and implement its virtual methods, demonstrating **abstraction, inheritance, and polymorphism**.

## Computer Player

The computer player evaluates possible rotations and positions before selecting a move.

Its decision-making considers:

- Completed lines
- Empty spaces below the piece
- Adjacency to existing blocks
- Piece dimensions
- Distance from the board walls

## Controls

| Action | Left Player | Right Player |
|---|---:|---:|
| Move left | `A` | `J` |
| Move right | `D` | `L` |
| Rotate clockwise | `S` | `K` |
| Rotate counterclockwise | `W` | `I` |
| Drop piece | `X` | `M` |
| Pause | `Esc` | `Esc` |

## Running the Project

1. Clone the repository:

```bash
git clone https://github.com/danareshef1/TetrisGame.git
```

2. Open the solution file in **Visual Studio**.
3. Build and run the project.

## Technologies

`C++` · `OOP` · `Abstract Classes` · `Inheritance` · `Polymorphism` · `Virtual Functions` · `Visual Studio`

## Authors

Developed by **Dana Reshef** and **Noy Zion**.
