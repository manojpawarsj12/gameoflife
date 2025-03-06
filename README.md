# Conway's Game of Life

This project is an implementation of Conway's Game of Life using p5.js. Conway's Game of Life is a cellular automaton devised by mathematician John Conway. It is a zero-player game, meaning its evolution is determined by its initial state, requiring no further input. The game consists of a grid of cells that can live, die, or multiply based on a few mathematical rules.

## How It Works

The universe of the Game of Life is an infinite, two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, alive or dead, or populated or unpopulated. Every cell interacts with its eight neighbors, which are the cells that are horizontally, vertically, or diagonally adjacent.

At each step in time, the following transitions occur:
1. Any live cell with fewer than two live neighbors dies, as if by underpopulation.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by overpopulation.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

The initial pattern constitutes the seed of the system. The first generation is created by applying the above rules simultaneously to every cell in the seed; births and deaths occur simultaneously, and the discrete moment at which this happens is called a tick. Each generation is a pure function of the preceding one. The rules continue to be applied repeatedly to create further generations.

## Setup and Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/manojpawarsj12/gameoflife.git
    cd gameoflife
    ```

2. Open `index.html` in your web browser to view the simulation.

## Code Explanation

The main code for the Game of Life is in the `sketch.js` file. Here is a breakdown of the key functions:

- `make2DArray(cols, rows)`: Creates a 2D array with the specified number of columns and rows.
- `setup()`: Initializes the canvas, sets up the grid, and populates it with random alive or dead cells.
- `draw()`: Continuously updates the grid based on the rules of the Game of Life and renders the cells on the canvas.
- `countNeighbors(grid, x, y)`: Counts the number of alive neighbors for a given cell in the grid.

## Usage

Once you open `index.html` in your browser, you will see the simulation start automatically. The grid will update based on the rules of the Game of Life, and you can observe how the cells evolve over time.

## Contributing

Contributions are welcome! If you have any ideas for improvements or bug fixes, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- John Conway, for devising the Game of Life.
- p5.js community, for providing an excellent library for creative coding.

Enjoy playing with the simulation and exploring the fascinating patterns that can emerge from simple rules!
