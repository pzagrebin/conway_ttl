# conway_ttl
Conway's Game of Life cell logic in six TTL ICs.

![conway_ttl_](https://user-images.githubusercontent.com/414986/174471073-a86463c9-7177-4a4c-a9c9-7ed7689ff8cd.png)

Five 181 ALUs produce number of alive neighbors, then multiplexer choose the next state:

0,1,4,5,6,7,8 -> dead

2 -> previous state

3 -> alive
