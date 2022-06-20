# conway_ttl
Conway's Game of Life cell logic in three TTL logic ICs.

![conway_ttl_](https://raw.githubusercontent.com/pzagrebin/conway_ttl/main/conway_ttl.png)

Two 283 adders produce sum of alive neighbor cells from seven cells,
then multiplexer choose the next state taking into account the last neighbor cell:

last cell is dead: 0,1,4,5,6,7 -> dead; 2 -> previous state; 3 -> alive

last cell is alive: 0,3,4,5,6,7 -> dead; 1 -> previous state; 2 -> alive

74250 output is inverted, so part of second adder is used to invert in back to positive.

[.dig](https://github.com/pzagrebin/conway_ttl/blob/main/conway_ttl.dig) file for [Digital](https://github.com/hneemann/Digital) simulator is included.
