# Banjo-Kazooie

So far all offsets are for in game save file 3

Currently the structure looks very confusing to me

### Offset dump

| Event               | Offest    | Changes / Data Type | Does it stay that way? |
|---------------------|-----------|---------------------|------------------------|
| Chimpy Jiggy        | 002       | Bit 0 =  1          | NOPE                   |
| MM Notes            | 022       | UI_8                | Yes                    |
| MM Time             | 028 - 02B | Counts in seconds?  | Yes                    |
| GL Time?            | 032 - 035 | Counts in seconds?  | Yes                    |
| MM Stonehenge MT    | 040       | Bit 4 = 1           | Yes                    |
| (Spendable MT)      | 065       | UI_8                | Yes                    |
| Eggs                | 66        | UI_8                | Yes                    |
| Spendable Jiggys    | 69        | UI_8                | Yes                    |
| Talon Trot          | 6B        | Bit 0 = 1           | Yes                    |
| Beak Buster         | 6D        | Bit 2 = 1           | Yes                    |
| Total Game Time     | 74 - 77   | Counts in seconds?  | Yes                    |
| MM Stonehenge Jiggy | 0F2       | Bit 2 = 1           | NOPE                   |
| MM Jinjo Jiggy      | 02        | Bit 1 = 1           | Yes?                   |
