What it does: 
Given any valid Rubik's Cube scramble, the solving algorithm will find a solution,
Uses Rubik's Cube Notation (eg. R U R' U') to communicate move sequence of solution.

How it works:
Cube Solver decomposes the search space into CFOP steps, it uses a BFS to first solve the white cross, (using # of placed pieces as search heuristic)
Then dynamically solves F2L pairs, by searching BFS, pruning as pairs form, and restarting the search after each new pair is slotted (this is necessarty to stop exponential search space explosion)
OLL and PLL (last 2 CFOP steps) are hardcoded (2 look OLL and PLL), BFS'ing for Last Layer algs is unnecessary. 

Why it's hard:
The Rubik's cube has 43 quintillion possible states. I avoid an exhaustive search of these states by using effective heuristics,
and CFOP decomposition of the solving process.


Features
Interactive 2D visualizer
Can input 
Step-by-step CFOP solution breakdown

How to run:
open html file in a browser, open inspect element console before using 
