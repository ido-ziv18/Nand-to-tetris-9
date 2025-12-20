# Nonogram Game

A Nonogram (also known as Picross or Griddlers) puzzle game implemented in Jack language for the Nand2Tetris course (Project 9).

## About Nonograms

Nonograms are picture logic puzzles where you fill in cells on a grid to reveal a hidden picture. The numbers on the left and top of the grid indicate how many consecutive filled cells are in each row/column.

## How to Play

### Controls

- **Arrow Keys**: Move the cursor around the grid
- **Space**: Paint/unpaint a cell (toggle between filled and empty)
- **X**: Mark a cell as definitely empty (places an X flag)
- **S**: Skip to the next puzzle
- **ESC**: Quit the game

### Objective

Use the number constraints on the rows and columns to determine which cells should be filled. When all cells match the hidden solution, you win and advance to the next puzzle.

### Tips

- Start with rows/columns that have the largest numbers
- Use X marks to indicate cells you know must be empty
- The constraints show groups of consecutive filled cells (e.g., "2 3" means a group of 2, a gap, then a group of 3)

## Puzzles

The game includes 5 puzzles that cycle:

1. **Heart** - A heart shape
2. **Smiley** - A smiling face
3. **Cat** - A cat silhouette
4. **Spaceship** - A rocket ship
5. **Turtle** - A turtle in the sun

## Project Structure

| File | Description |
|------|-------------|
| `Main.jack` | Entry point, launches the game |
| `NonogramGame.jack` | Main game logic, puzzle definitions, input handling |
| `Board.jack` | Board data structure and constraint generation |
| `GraphicsManager.jack` | All rendering: grid, squares, cursor, constraints, border |
| `TitleScreen.jack` | Title screen with logo, instructions, and key prompt |
| `DigitRenderer.jack` | Pixel-art digit rendering for constraint numbers |
| `Point.jack` | Simple x,y coordinate class |

## Building and Running

This project is designed for the Nand2Tetris software suite:

1. Compile all `.jack` files using the Jack Compiler
2. Load the compiled `.vm` files into the VM Emulator
3. Run the program

## Technical Notes

- Screen resolution: 512x256 pixels (black and white)
- Grid size: 10x10 cells
- Written in Jack, a simple object-oriented language
- No external dependencies beyond the Nand2Tetris OS

## Author

Developed as part of the Nand2Tetris course (Project 9: High-Level Language).

