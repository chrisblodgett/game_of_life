# Game of Life - self-replicating systems with cellular automation

## This is a zero player game created by John Horton Conway way back in 1970, where evolution is determined by some initial conditions after which you get to observe how the game evolves.

The game world is an infinite grid (in theory) of square 'cells' each of which could be in two possible states either alive or dead (or if you wish populated and unpopulated).

Every cell interacts with its eights neighbors (horizontally, vertically, and diagonally).

There are only 4 rules that govern this interaction and whether a cell emerges from the interaction alive or dead-

Any live cell with fewer than two live neighbors dies, as if by underpopulation.
Any live cell with two or three live neighbors lives on to the next generation.
Any live cell with more than three live neighbors dies, as if by overpopulation.
Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.
All other cells (which ones do these pertain to by the way) keep their current life status unchanged.

The initial pattern (conditions) of the world grid constitutes the seed of the system, the first generation is created by applying the above rules simultaneously to every cell in this seed. Live, dead, births and deaths occur simultaneously - this happens during the discrete moement called a tick (you'll see what this means in the code and my way of handling it). Afterwhich, the rules continue to be applied repeatedly to create further generations.

Before looking at my implementation below, I encourage you to try to code this on your own from the rules only which is the route I went, throughout the process you'll learn so much and it really is alot of fun. Originally, amazingly, different tile patterns and how they evolve were discovered without computers by using blackboards and graph paper by hand.

It goes without saying that in my code the world is not infiinite - I've made it so my boundary cells (outside_boundary) can either be all dead or all alive (I defaulted to all alive but feel free to change it).

When I first learned about this automation I was fasicnated and amazed at how such an interesting and dyamic system could be created from random intial conditions four simple rules applied repeatedly. I love the simplicity and beauty of this automation, I hope you will too. Let's get to it-
