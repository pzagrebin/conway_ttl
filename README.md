# conway_ttl
Conway's Game of Life cell logic in six TTL ICs.

Five 181 ALUs produce number of alive neighbors, then multiplexer choose the next state:

0,1,4,5,6,7,8 -> dead

2 -> previous state

3 -> alive
