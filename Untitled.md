| Operation Name | addresing mode allowed in source operand | addresing mode allowed in destination operand |
| -------------- | ---------------------------------------- | --------------------------------------------- |
| mov            | 0, 1, 2, 3                               | 1, 2, 3                                       |
| cmp            | 0, 1, 2, 3                               | 0, 1, 2, 3                                    |
| add            | 0, 1, 2, 3                               | 1, 2, 3                                       |
| sub            | 0, 1, 2, 3                               | 1, 2, 3                                       |
| not            | No source operand                        | 1, 2, 3                                       |
| clr            | No source operand                        | 1, 2, 3                                       |
| lea            | 1, 2                                     | 1, 2, 3                                       |
| inc            | No source operand                        | 1, 2, 3                                       |
| dec            | No source operand                        | 1, 2, 3                                       |
| jmp            | No source operand                        | 1, 3                                          |
| bne            | No source operand                        | 1, 3                                          |
| red            | No source operand                        | 1, 2, 3                                       |
| prn            | No source operand                        | 0, 1, 2, 3                                    |
| jsr            | No source operand                        | 1, 3                                          |
| rts            | No source operand                        | No destination operand                        |
| hlt            | No source operand                        | No destination operand                        |