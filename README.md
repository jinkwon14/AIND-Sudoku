# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Applying the *Naked Twins* method once to the sudoku board eliminate possible occurrences of a pair of values from a remote part of sudoku board. After such values are eliminated, more values in other parts of the board may fall under the conditions of the Naked Twins(or other) method and be further eliminated. This is exactly the application of constraint propagation: enforcing a constraint in one part of the board introduce new constraints in other parts of the board.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Diagonal Sudoku problem introduces an additional constraint to consider. This is beneficial in terms of using constraint propagation for solving sudoku puzzle because now more values fall under the constraints(or conditions to be eliminated) of each elimination method. Therefore more values are eliminated, and in turn, more constraints are introduced in other parts of the board (TODO: graph substantiating this point).

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
