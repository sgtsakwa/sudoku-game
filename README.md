# Sudoku Game

An interactive Sudoku application built in Python using Kivy.  
This project combines gameplay features with algorithmic solving and puzzle generation, with backtracking used as the core solving method.

## Project Overview

This application was developed to demonstrate both the user experience of playing Sudoku and the underlying logic used to solve and generate puzzles. The project includes multiple difficulty levels, interactive controls, and a graphical user interface designed for accessible gameplay.

## Features

- Multiple difficulty levels: Easy, Medium, Hard, and Extreme
- Sudoku puzzle generation
- Backtracking-based Sudoku solver
- Interactive graphical user interface built with Kivy
- Hint system
- Notes mode
- Undo and erase functions
- Pause and resume functionality
- Score tracking
- Timer
- Mistake counter and game-over condition

## Technologies Used

- Python **[version 3.14.3]**
- Kivy **[version 3.11.9]**
- Visual Studio Code for development and testing

## How the Project Works

The game first generates a complete valid Sudoku solution using recursive backtracking.  
A playable puzzle is then created by removing values according to the selected difficulty level.

The solver works by:
1. Finding an empty cell
2. Testing candidate values
3. Checking whether each value is valid according to Sudoku rules
4. Moving forward recursively if the value is valid
5. Backtracking if a dead end is reached

## Difficulty Levels

Difficulty is controlled by the number of clues left in the puzzle.

- **Easy**: more starting clues
- **Medium**: moderate number of clues
- **Hard**: fewer starting clues
- **Extreme**: minimal clues, more challenging generation and solving

Harder puzzles require fewer pre-filled values, which increases the logical effort needed to solve them.

## Repository Structure

```text
main.py
icons/
README.md
