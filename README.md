# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Applying a *Naked Twins* method once to the sudoku board eliminate possible occurances of a pair of values from a number of boxes on a sudoku board. After such values are eliminated, more values in other parts of the board may be eliminated by the Naked Twins (or other) method. This is exactly the application of constraint propagation: enforcing a constraint in one part of the board introduces new constraints in other parts of the board.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Diagonal sudoku problem introduces an additional constraint to consider. This is beneficial for the constraint propagation in solving sudoku because now more values fall under the constraint(or conditions to be eliminated) of each elimination method, therefore more values are eliminated, and in turn more constrains are introduces in other parts of the board (TODO: graph substantiating this point).

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
