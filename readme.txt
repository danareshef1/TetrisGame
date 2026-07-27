Tetris Game – Object-Oriented C++ Project

A console-based Tetris game developed in C++ with a strong focus on object-oriented design, modularity, and polymorphism.

The game supports multiple competition modes, including Human vs. Human, Human vs. Computer, and Computer vs. Computer. Computer-controlled players evaluate possible placements using a heuristic scoring system and can play at three difficulty levels.

Features

Human vs. Human gameplay

Human vs. Computer gameplay

Computer vs. Computer gameplay

Three computer difficulty levels: Best, Good, and Novice

Independent game boards and scoring for both players

Shape movement, rotation, collision detection, and line clearing

Immediate piece drop

Optional colored or monochrome display

Pause and continue functionality

Console-based user interface

Object-Oriented Design

The project uses object-oriented programming principles to separate the game logic into modular components:

Player – an abstract base class that defines the shared player interface

Human – handles keyboard-controlled gameplay

Computer – calculates and executes computer-controlled moves

Board – manages the game board, collisions, occupied cells, and completed lines

Shapes – manages Tetris pieces, movement, rotation, and placement

Point – represents individual coordinates

TetrisGame – controls the game loop and coordinates both players

Menu – manages game modes, instructions, color settings, and game state

The Human and Computer classes inherit from Player and implement its virtual methods, allowing the game to manage both player types through a common interface.

Computer Player

The computer player evaluates possible rotations and board positions before choosing a move.

Its heuristic considers factors such as:

Completed lines

Empty spaces below the piece

Piece height and width

Adjacency to existing blocks

Proximity to board walls

The selected difficulty level affects how often the computer chooses the highest-rated placement.

Controls

Action

Left Player

Right Player

Move left

A

J

Move right

D

L

Rotate clockwise

S

K

Rotate counterclockwise

W

I

Drop piece

X

M

Pause game

Esc

Esc

Lowercase and uppercase controls are supported.

Technologies and Concepts

C++

Object-Oriented Programming

Abstract classes

Inheritance and polymorphism

Virtual functions

Modular class design

Heuristic-based decision making

Console input and rendering

Visual Studio

Project Structure

TetrisGame_Noy_Dana/
├── main.cpp
├── menu.cpp / menu.h
├── tetrisGame.cpp / tetrisGame.h
├── player.cpp / player.h
├── human.cpp / human.h
├── computer.cpp / computer.h
├── board.cpp / board.h
├── shapes.cpp / shapes.h
├── point.cpp / point.h
├── general.cpp / general.h
└── gameDef.h

Running the Project

This project is designed as a Windows console application.

Clone the repository:

git clone https://github.com/danareshef1/TetrisGame.git

Open TetrisGame_Noy_Dana.sln in Visual Studio.

Build the solution.

Run the project from Visual Studio.

Authors

Developed by Dana Reshef and Noy Zion.
