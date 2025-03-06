# Tower of Hanoi - Interactive Puzzle Game

## Overview

This project implements the classic **Tower of Hanoi** puzzle game using **JavaScript** and **SVG** (Scalable Vector Graphics). It includes an interactive interface with visual representations of disks and pegs, along with step-by-step controls, animations, and an optimized solution using dynamic programming.

### Key Features
- **Interactive User Interface**: Play the Tower of Hanoi game with a graphical SVG-based interface.
- **Step-by-Step Mode**: Allows users to control the game flow step-by-step.
- **Dynamic Programming**: Optimized solution using dynamic programming for minimal moves.
- **Disk Movement Animations**: Smooth animations for moving disks between pegs.
- **Abort/Resume**: Allows pausing, resuming, and aborting animations at any time.

## Technologies Used

- **JavaScript (ES6+)**: For game logic, animations, and handling user interactions.
- **SVG (Scalable Vector Graphics)**: For rendering the game's visual elements (disks, pegs, and base).
- **HTML5**: For structuring the game UI and appending the SVG elements.
- **CSS**: For basic styling, like rounding corners and adding drop shadows.
- **Async/Await**: For handling asynchronous disk movements and animations.
- **AbortController**: To abort ongoing animations and allow user control over the game's flow.
- **Dynamic Programming**: To calculate the optimal sequence of moves efficiently.

## How It Works

### 1. **Game Setup**
   - The game is initialized with a configurable number of pegs and disks.
   - Each disk is visually represented by a rectangle, and pegs are placed vertically.
   - The base of the puzzle is rendered at the bottom.

### 2. **Game Logic**
   - The goal is to move all the disks from the first peg to the last peg, following the rules:
     - Only one disk can be moved at a time.
     - A larger disk cannot be placed on top of a smaller disk.
   - The solution is calculated using dynamic programming to minimize the number of moves.

### 3. **Disk Movement**
   - Each disk's movement is animated with SVG's `<animateMotion>` tag.
   - The disk moves smoothly along a path calculated based on the starting and target peg positions.

### 4. **Step-by-Step Mode**
   - In step mode, users can manually progress the game one move at a time, providing more control over the puzzle-solving process.
   - Users can pause, resume, or abort the game at any time.

## Installation

To use this project, you need a web environment. Follow these steps to get started:

### 1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/tower-of-hanoi.git
