# Active Multiples
This project provides tested plans for a 4HP Eurorack-format synthesizer module, containing two banks of 1 -> 3 active buffers, taking any signal at the input and precisely replicating it on the three outputs.

![Assembled module](/media/1-in-rack)

![Boards](/media/2-boards-front-back.jpg)


## BOM 

Qty | Value            | Device                  | Package             | Parts                                                |
--- | ---------------- | ----------------------- | ------------------- | ---------------------------------------------------- |
8   |                  | Inline mono jack        |                     | A, A1, A2, A3, B, B1, B2, B3                         |
1   |                  | 5x2                     | 2.54mm Pin          | Power                                                |
6   | ~100nF           | Capacitor               | 0603                | DC1 – DC6                                            |
3   | TL072            | Dual op amp             | TSSOP8              |                                                      |


## Notes

1. Solder the power connector before soldering signal jacks. There is very little space between the jacks to reach the top of the board after they are attached.
1. Input A (labeled on PCB) drives output A1, A2, A3; Input B drives output B1, B2, B3. Input A is normalled to Input B; if this behavior isn't desired, cut jumper trace labeled A->B.

