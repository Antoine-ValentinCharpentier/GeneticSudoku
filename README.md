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

## Some generic definitions / Main steps

- **Genetic Algorithm**  
This is an optimization method inspired by the natural selection process in biological evolution. It simulates the process of natural selection, genetic recombination, and mutation. 

- **Individual**  
 A potential solution to the problem at hand. It is characterized by a set of genes. Each genome is characterized by a set of genes that represent something in the individual (to encode an individual's speed, ...).

- **Population**  
Set of individuals. We start by generating an initial population.

- **Fitness Function**  
 A fitness function is defined to evaluate how well each individual in the population performs compared to the optimal solution. It assigns a fitness score to each individual, allowing for an assessment of their ability to solve the given problem.

- **Selection**  
Individuals in the population are selected based on their fitness score. Individuals with higher scores are more likely to be selected.

- **Crossover**  
Selected individuals are crossed to create new individuals (offspring). This simulates the process of genetic recombination, where parental characteristics are mixed to create offspring.

- **Mutation**  
 New individuals may undergo random mutations with a certain probability. Mutations introduce variability into the population by randomly modifying some of their characteristics.

- **New Generation**  
 The new generation of individuals resulting from selection, crossover, and potentially mutation becomes the population for the next generation. This process is repeated over multiple generations.
