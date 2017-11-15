# Sudoku Solver

1. Synopsis

### TODO : quick brief for what is Sudoku

Sudoku Solver is the first project in my Artificial Intelligence Nanodegree. In this project, I implemented Sudoku solver using following strategies:
	
   - **Elimination**
   	 Search for unit with only one value in Sudoku board. Then remove that values from its peers
	 ### TODO : add picture

   - **Only Choice**
	 Search for units only one posiible value, assign that value to the units and then eliminate that value from its peers.
	 ### TODO : add picture

   - **Naked Twins**
	 Search all Sudoku board for units with the smae possible values. Try to solve that board with one of the pairs, if the board is not solved, solve the board with the another value.

With strategies above, this Sudoku Solver is able to solve any sudoku question!

However, I also modified my solver to be able to solve _Diaagonal Sudoku_

### TODO : explain what is Diagonal Sudoku

2. Repo Structure


# Scratchpad below

# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: First, we pick a unit from unitlist as our 1st constraint. Then we looking for any box that contain exactly 2 digits, our 2nd constraint. Looping through each box in 1st constraint and eliminate any digit in our 2nd constraint except the boxes that contain those digits until there is no more to eliminate. Repeat the process.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Adding 2 diagonal units (diag1: (A1,B2,C3,D4,E5,F6,G7,H8,I9), and diag2: (A9,B8,C7,D6,E5,F4,G3,H2,I1)) to unitlist as other constrains of our program. Instead of adjacent peers, our sudoku solver considers those peers and diagonal peers and repeats the steps until board is solve. 

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solution.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Submission
Before submitting your solution to a reviewer, you are required to submit your project to Udacity's Project Assistant, which will provide some initial feedback.  

The setup is simple.  If you have not installed the client tool already, then you may do so with the command `pip install udacity-pa`.  

To submit your code to the project assistant, run `udacity submit` from within the top-level directory of this project.  You will be prompted for a username and password.  If you login using google or facebook, visit [this link](https://project-assistant.udacity.com/auth_tokens/jwt_login for alternate login instructions.

This process will create a zipfile in your top-level directory named sudoku-<id>.zip.  This is the file that you should submit to the Udacity reviews system.

