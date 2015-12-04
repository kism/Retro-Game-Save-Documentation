# Banjo-Kazooie

So far all offsets are for in game save file 3

Currently the structure looks very confusing to me

[My save file archive](https://github.com/kism/Retro-Game-Save-Documentation/tree/master/Nintendo%2064/Working/Banjo-Kazooie)

[Hex Workshop Bookmarks](https://github.com/kism/Retro-Game-Save-Documentation/tree/master/Nintendo%2064/Hex%20Workshop%20Bookmarks)

### Save layout

Save 3 - 000 - 077

Save 2 - 078 - 0EF

Save 1 - 168 - 1DF

Stop N Swap? - 1E0 - 1FF

### Quirks

Checksum? validation happens at game select, apparently 1F8 - 167 doesnt get cleared

A weird clone of data appears at 1F0 - 167?

The stop n swap area is the only area validated on boot?

### Offset dump

| Event               | Offest    | Changes / Data Type | Does it stay that way? |
|---------------------|-----------|---------------------|------------------------|
| Chimpy Jiggy        | 002       | Bit 0 =  1          | NOPE                   |
| MM Notes            | 022       | UI_8                | Yes                    |
| MM Time             | 028 - 02B | Counts in seconds?  | Yes                    |
| GL Time?            | 032 - 035 | Counts in seconds?  | Yes                    |
| MM Stonehenge MT    | 040       | Bit 4 = 1           | Yes                    |
| (Spendable MT)      | 065       | UI_8                | Yes                    |
| Eggs                | 066       | UI_8                | Yes                    |
| Spendable Jiggys    | 069       | UI_8                | Yes                    |
| Talon Trot          | 06B       | Bit 0 = 1           | Yes                    |
| Beak Buster         | 06D       | Bit 2 = 1           | Yes                    |
| Total Game Time     | 074 - 077 | Counts in seconds?  | Yes                    |
| MM Stonehenge Jiggy | 0F2       | Bit 2 = 1           | NOPE                   |
| MM Jinjo Jiggy      | 002       | Bit 1 = 1           | Yes?                   |
