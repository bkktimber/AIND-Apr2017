# Sudoku Solver

1. Synopsis

## TODO : quick brief for what is Sudoku

Sudoku Solver is the first project in my Artificial Intelligence Nanodegree. In this project, I implemented Sudoku solver using following strategies:
	
   - **Elimination**
   	 Search for unit with only one value in Sudoku board. Then remove that values from its peers
	 ## TODO : add picture

   - **Only Choice**
	 Search for units only one posiible value, assign that value to the units and then eliminate that value from its peers.
	 ## TODO : add picture

   - **Naked Twins**
	 Search all Sudoku board for units with the smae possible values. Try to solve that board with one of the pairs, if the board is not solved, solve the board with the another value.

With strategies above, this Sudoku Solver is able to solve any sudoku question!

However, I also modified my solver to be able to solve _Diaagonal Sudoku_

## TODO : explain what is Diagonal Sudoku

** TODO **

2. Repo Structure