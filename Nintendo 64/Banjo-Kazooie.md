# Banjo-Kazooie

[My save file archive](https://github.com/kism/Retro-Game-Save-Documentation/tree/master/Nintendo%2064/Working/Banjo-Kazooie)

[Hex Workshop Bookmarks](https://github.com/kism/Retro-Game-Save-Documentation/tree/master/Nintendo%2064/Hex%20Workshop%20Bookmarks)

### Save layout

| Thing                    | Range     | Length |
|--------------------------|-----------|--------|
| Metadata ?               | 000 - 007 | 8      |
| Save 3                   | 008 - 077 | 70     |
| ???                      | 078 - 07F | 8      |
| Save 2                   | 080 - 0EF | 70     |
| Copy of 'Metadata ?'     | 0F0 - 0F7 | 8      |
| Copy of last loaded save | 0F7 - 167 | 70     |
| ???                      | 168 - 16F | 8      |
| Save 1                   | 170 - 1DF | 70     |
| Stop N Swap?             | 1E0 - 1FF | 20     |

### Quirks

Save validation happens at game select screen, the only save that can be validated is the one that was last loaded, the game compares the save with a copy at 0F7 - 167. 1F8 - 167 doesnt get cleared if data is invalid and will only be overridden on the next save.

The last file loaded is located at 001 as an unsigned integer

The stop n swap? area is the only area validated on boot.

### Offset dump

So far all offsets are for in game save file 3 (subtract 8 for it to be reletive to the start of the save (I'll fix this later))

**Spendable Items**

| Event            | Offest |
|------------------|--------|
| Mumbo Tokens     | 065    |
| Eggs             | 066    |
| Red Feathers     | 067    |
| Gold Feathers    | 068    |
| Jiggys           | 069    |

**Totals (UI_16 Counts in seconds)**

| Event               | Offest    |
|---------------------|-----------|
| SM Time             | 0E3 - 0E4 |
| GL Time             | 034 - 035 |
| MM Time             | 02A - 02B |
| TTT Time            | 02C - 02D |
| CC Time             | 02E - 02F |
| BGS Time            | 030 - 031 |
| FP Time             | 032 - 033 |
| GV Time             | 036 - 037 |
| MMM Time            | 03C - 03D |
| RBB Time            | 03A - 03B |
| CCW Time            | 03E - 03F |

**Moves**

| Move        | Offset | Bit       |
|-------------|--------|-----------|
| Talon Trot  | 06B    | Bit 0 = 1 |
| Beak Buster | 06D    | Bit 2 = 1 |

**Mumbos Mountian Collectables**

| Thing            | Offset | Changes / Data Type |
|------------------|--------|---------------------|
| MM Notes         | 022    | UI_8                |
| MM Stonehenge MT | 040    | Bit 4 = 1           |
