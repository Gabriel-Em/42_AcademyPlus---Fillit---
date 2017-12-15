# 42 Academy+Plus - Fillit
A 42 (school) project that required us to discover and familiarize ourselves with a recurring problematic in programming: searching the optimal solution among a huge set of possibilities, in a respectable timing. In this particular project, we had to find a way to assemble a given Tetriminos set altogether in the smallest possible square.

For more details see 'Fillit - Subject(EN).pdf'

## How to use
Using a terminal from within the Fillit directory:
- run the **Makefile** using the command **make** (this generates the binary as **"fillit"**)
- run the command `./fillit input_file`, where input_file should contain between 1 and 26 tetriminos that must respect the following rules:
	- Precisely 4 lines of 4 characters, each followed by a new line
	- A Tetrimino is a classic piece of Tetris composed of 4 blocks
	- Each character must be either a block character(’#’ ) or an empty character (’.’)
	- Each block of a Tetrimino must touch at least one other block on any of his 4 sides (up, down, left and right)

Examples of valid dscriptions of tetriminos:
```
....   ....   ####   ....   .##.   ....   .#..   ....   ....
..##   ....   ....   ....   ..##   .##.   ###.   ##..   .##.
..#.   ..##   ....   ##..   ....   ##..   ....   #...   ..#.
..#.   ..##   ....   ##..   ....   ....   ....   #...   ..#.
```

- if your input_file doesn't contain valid input, fillit will display "error" and exit, otherwise it will display the smallest possible square to fit all tetriminos, labeled from 'A' to 'Z' in the order they were read from your input_file.

**Example of a valid input file:**

![preview](https://i.imgur.com/Wp0BUHs.png)

**Running fillit on the input file from above:**

![preview](https://i.imgur.com/yqznT0U.png)

# How to test

If you want to test the code, or your own implementation of fillit you can use 
- @jgigault's [42FileChecker](https://github.com/jgigault/42FileChecker)

and follow the instructions on his repository. (*Note: by the time you're reading this there's a good chance there are a lot more fillit testers out there, so look them up yourself as well.*)
