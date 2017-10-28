# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Suduko can have identical twins, triplets, quads etc. <Br />
   1.Finding all instances of naked twins from rows, colums and 3x# square units  <Br />
   2.Eliminating the naked twins as possibilities for their peers

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: There are two diagonal arrays
[A1, B2, C3, D4, E5, F6, G7, H8, I9]  and [A9, B8, C7, D6, E5, F4, G3, H2, I1]
so these are added to the unitlist and passing to the same proceoss of eliminate and naked twins 
recursively until the suduko is solved. 


#   Solved Sudoko
2 6 7 |9 4 5 |3 8 1<br />
8 5 3 |7 1 6 |2 4 9<br />
4 9 1 |8 2 3 |5 7 6<br />
------+------+------<br />
5 7 6 |4 3 8 |1 9 2 <br />
3 8 4 |1 9 2 |6 5 7 <br />
1 2 9 |6 5 7 |4 3 8 <br />
------+------+------<br />
6 4 2 |3 7 9 |8 1 5 <br />
9 3 5 |2 8 1 |7 6 4 <br />
7 1 8 |5 6 4 |9 2 3<br />

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solution.py` - Fill in the required functions in this file to complete the project.
* `test_solution.py` - You can test your solution by running `python -m unittest`.
* `PySudoku.py` - This is code for visualizing your solution.
* `visualize.py` - This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the `assign_value` function provided in solution.py

### Submission
Before submitting your solution to a reviewer, you are required to submit your project to Udacity's Project Assistant, which will provide some initial feedback.  

The setup is simple.  If you have not installed the client tool already, then you may do so with the command `pip install udacity-pa`.  

To submit your code to the project assistant, run `udacity submit` from within the top-level directory of this project.  You will be prompted for a username and password.  If you login using google or facebook, visit [this link](https://project-assistant.udacity.com/auth_tokens/jwt_login) for alternate login instructions.

This process will create a zipfile in your top-level directory named sudoku-<id>.zip.  This is the file that you should submit to the Udacity reviews system.

