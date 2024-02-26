# Game of Life - the problem of self-replicating systems with cellular automation
### created by John Horton Conway in 1970

This is a zero player game, where the evolution is determined by some initial conditions and you get to observe how it evolves.
It is 'Turing Complete' it can simulate a universal constructor or any other turing machine
 
The world is an infinite grid of square cells each of which could be in two possible states live or dead (or if you wish populated and unpopulated)
Every cell interacts with its eights neighbors, horizontally, vertically, and diagonally

There are only 4 rules that govern everything-

Any live cell with fewer than two live neighbors dies, as if by underpopulation.
Any live cell with two or three live neighbors lives on to the next generation.
Any live cell with more than three live neighbors dies, as if by overpopulation.
Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

the initial pattern constituters the seed of the system, first generation is created by applying the above rules simultaneously to every cell in the seed, live or dead, births and deaths occur simultaneously, during the discrete moement called a tick. The rules continue to be applied repeatedly to create further generations :) 

Before looking at my implementation below, I encourage you to program your own implementation, throughout the process you'll learn so much.

It goes without saying that my world is not infiinite - I've made it so my boundary cells (outside_boundary variable) can either be all dead or all alive. When I first learned about this automation I was fasicnated and amazed on how such an interesting and dyamic system could be created from just four simple rules. I love the simplicity and beauty, I hope you will too. 
