What it does: 
Given any valid Rubik's Cube scramble, the solving algorithm will find a solution,
Uses Rubik's Cube Notation (eg. R U R' U') to communicate move sequence of solution.

How it works:
Cross — BFS with number of correctly placed edge pieces as the search heuristic
F2L — Dynamic BFS that prunes the search as pairs form, restarting after each pair is slotted to prevent exponential state space explosion
OLL / PLL — Hardcoded 2-look OLL and PLL pattern matching; BFS over the last layer is unnecessary given the finite algorithm set

Why it's hard:
The Rubik's cube has 43 quintillion possible states. I avoid an exhaustive search of these states by using effective heuristics,
and CFOP decomposition of the solving process.


Features
Interactive 2D visualizer
Can input 
Step-by-step CFOP solution breakdown

How to run:
open html file in a browser, open inspect element console before using 
