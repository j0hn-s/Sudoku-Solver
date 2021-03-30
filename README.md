# Sudoku_Solver
Simple, but well-implemented, backtracking algorithm that solves any sudoku passed through the solver function, using Python (in Notebook format for additional info and tests)

A standard game of sudoku begins with an initial configuration which yields a series of possible and impossible moves, given the rules of the game (for official rules see: https://www.ultraboardgames.com/sudoku/game-rules.php). The provided uses a set of recursively defined functions to solve any inputted sudoku.

Despite being relatively well-implemented, the algorithm does not take full advantage of the constantly increasing heuristic-values that could be used to solve a sudoku throughout any given simulated game and hence performs rather slowly on some  harder sudokus; albeit accurately. Originally the designer of the algorithm aimed to implement an Arc Constraint Algorithm (AC-3), but had trouble implementing a function that created a fully functional instance of the originally-defined constraint satisfaction class.

The designer of the algorithm has consciously settled for a slower but more accurate model, which could have benefitted from a set of additional functions (as included in most AC-3 algorithms or often implemented in well-played human-actor games, such as 'Schneider Notation'), which discover and store illegal- and partially assigned- values as heuristics, to eliminate, propagates and force the yielding of specific values.
