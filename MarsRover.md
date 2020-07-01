## Mars Rover

A squad of robotic rovers are to be landed by NASA on a plateau on Mars.

This plateau, which is curiously rectangular, must be navigated by the rovers so that their onboard cameras
can get a complete view of the surrounding terrain to send back to Earth.

Your task is to develop an API that moves the rovers around on the plateau.

In this API, the plateau is represented as a 10x10 grid, and a rover has state consisting of two parts:

- Its position on the grid (represented by an X,Y coordinate pair)
- The compass direction it's facing (represented by a letter, one of `N`, `S`, `E`, `W`)

### Input

The input to the program is a string of one-character move commands:

- `L` and `R` rotate the direction the rover is facing
- `M` moves the rover one grid square forward in the direction it is currently facing

If a rover reaches the end of the plateau, it wraps around the end of the grid.

### Output

The program's output is the final position of the rover after all the move commands have been executed. The position is
represented as a coordinate pair and a direction, joined by colons to form a string. For example: a rover whose 
position is `2:3:W` is at square (2,3), facing west.


### Rules
- The rover start from 0,0, in North direction.
- The rover receives a char array of commands e.g. `RMMLM` and returns the finishing point after the moves e.g. `2:1:N`
- The rover wraps around if it reaches the end of the grid.

### Examples
- given a grid, input `MMRMMLM` gives output `2:3:N`
- given a grid, input `MMMMMMMMMM` gives output `0:0:N` (due to wrap-around)
