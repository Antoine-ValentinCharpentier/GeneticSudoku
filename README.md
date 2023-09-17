# GeneticSudoku

## Description

This project provides a solution to generate and solve Sudoku grids using genetic algorithms. 

Two distinct phases are implemented:
1. **Generation** of Sudoku grids to be filled
2. **Resolution** of the generated Sudoku grids

## Generation of Sudoku grids to be filled

To generate Sudoku grids for user completion, a genetic algorithm is employed. The genetic algorithm initiates by establishing a population of random Sudoku grids. Subsequently, it assesses the fitness score of each grid by counting the number of misplaced digits both by row and by column.

Grids with a minimal number of misplaced digits are then selected to shape the succeeding generation.

Across successive generations, the population converges towards a well-formed and filled sudoku grid.

Subsequently, we remove some digits, enabling the user to fill them in.

## Resolution of the generated Sudoku grids

Not yet implemented

## Setup the Project

1. Clone the repository:
    ```bash
    git clone git@github.com:Antoine-ValentinCharpentier/GeneticSudoku.git
    cd GeneticSudoku
    ```
2. Initialise the venv:
    ```bash
    python -m venv .venv
    .venv\Scripts\activate OU source .venv/bin/activate
    pip install -r requirements.txt
    ```