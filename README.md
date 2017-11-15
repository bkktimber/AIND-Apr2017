# Sudoku Solver

1. Synopsis

### TODO : quick brief for what is Sudoku

Sudoku Solver is the first project in my Artificial Intelligence Nanodegree. The objectives of this project are:
   
   - **Setup and Familiar with Working Environment**
	 This project is run in Python3.6 and uses [Anaconda](https://www.continuum.io/downloads).

   - **Introduction to techniques that are used in building AI agent**
     Sudoku solver uses following techniques:
     	- Contraint Propagation
     	- Depth-First Search

    -**Implement problem solving steps to AI agent**
     There are many technique to solve sudoku problem. Below are techniques used in this solver 

   		- **Elimination**
   	 	  Find any cell in given Sudoku baord that contains a value. Then remove that value from other units in the same row and column. Repeat until no single value unit left in Sudoku baord

	   - **Only Choice**
	   	  Find cells that contain only 1 possible value. Then assign that value to result.

	   - **Naked Twins**
		  Find cells pairs that contain exactly same 2 values. Choose one value from those 2 values then eleminate until there is no other number to eliminate.

With strategies above, this Sudoku Solver is able to solve any sudoku question!

However, I also modified my solver to be able to solve _Diaagonal Sudoku_

### TODO : explain what is Diagonal Sudoku

2. Repo Structure

   - `solution.py`: Sudoku solver that uses strategies describe above.
