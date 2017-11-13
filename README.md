# Sudoku Solver

1. Synopsis

Sudoku Solver is the first project in my Artificial Intelligence Nanodegree. In this project, I implemented Sudoku solver using following strategies:
	
	- **Elimination**
	  Search for unit with only one value in Sudoku board. Then remove that values from its peers
	  ## TODO : add picture

	- **Only Choice**
	  Search for units only one posiible value, assign that value to the units and then eliminate that value from its peers.
	  ## TODO : add picture

	- **Naked Twins**
	  Search all Sudoku board for units with the smae possible values. Try to solve that board with one of the pairs, if the board is not solved, solve the board with the another value.


For this project, you will implement some extensions to the Sudoku algorithm developed in the lectures. The first extension will be an implementation of the naked twins technique. The second will be a modification of the algorithm to solve a diagonal sudoku.

** TODO **

2. Repo Structure