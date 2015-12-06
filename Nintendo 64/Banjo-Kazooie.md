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
| Copy of Metadata ?       | 0F0 - 0F7 | 8      |
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
| Jiggys           | 069    |
| Eggs             | 066    |

**Totals**

| Event               | Offest    | Changes / Data Type |
|---------------------|-----------|---------------------|
| MM Time             | 028 - 02B | Counts in seconds?  |
| GL Time?            | 032 - 035 | Counts in seconds?  |
| Total Game Time     | 074 - 077 | Counts in seconds?  |

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
