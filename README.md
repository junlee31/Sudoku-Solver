# Sudoku-Solver

For this project, I have used Python to create a Sudoku Solver. In order to create an efficient solver, I decided to utlizie a backtracking algorithm to find the possible solutions. By using a backtracking algo, it goes through each empty box and figures out a solution. If the solution ends up being wrong, it backtracks to the last empty box and solves it again. 

How it works:

I created 4 functions:

   1. print_board:
            - In this function it prints out the sudoku board that you wish to solve.
    
   2. find_empty:
            - In this function, we want to locate the empty spaces in order to begin the solver. 
   
   3. check:
            - In this function, we check to see if the solutions the algorithm has found are valid or not. 
    
   4. solve:
            - Lastly, we take the functions above and create a solve function which solves your board. 


Example #1:
Board Without Answers: (0 represents empty spaces)

7 8 0 |4 0 0 |1 2 0

6 0 0 |0 7 5 |0 0 9

0 0 0 |6 0 1 |0 7 8
- - - - - - - - - - 
0 0 7 |0 4 0 |2 6 0

0 0 1 |0 5 0 |9 3 0

9 0 4 |0 6 0 |0 0 5
- - - - - - - - - - 
0 7 0 |3 0 0 |0 1 2

1 2 0 |0 0 7 |4 0 0

0 4 9 |2 0 6 |0 0 7

Board With Correct Answers:

7 8 5 |4 3 9 |1 2 6

6 1 2 |8 7 5 |3 4 9

4 9 3 |6 2 1 |5 7 8
- - - - - - - - - - 
8 5 7 |9 4 3 |2 6 1

2 6 1 |7 5 8 |9 3 4

9 3 4 |1 6 2 |7 8 5
- - - - - - - - - - 
5 7 8 |3 9 4 |6 1 2

1 2 6 |5 8 7 |4 9 3

3 4 9 |2 1 6 |8 5 7
