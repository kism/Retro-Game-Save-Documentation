#Super Mario 64

Save type: eeprom 512 bytes

The end of a section in the save area is marked by 0x44 0x41 0x00 0xXX, 0xXX being the 8 bit checksum, each save takes up two sections which contain (hopefully) the same data.

| Thing          | Range     | Checksum location |
|----------------|-----------|-------------------|
| Save 1 Copy 1  | 000 - 035 | 037               |
| Save 1 Copy 2  | 038 - 06D | 06F               |
| Save 2 Copy 1  | 070 - 0A5 | 0A7               |
| Save 2 Copy 2  | 0A8 - 0DD | 0DF               |
| Save 3 Copy 1  | 0E0 - 115 | 117               |
| Save 3 Copy 2  | 118 - 14D | 14F               |
| Save 4 Copy 1  | 150 - 185 | 187               |
| Save 4 Copy 2  | 188 - 1BD | 1BF               |
| Options Copy 1 | 1C0 - 1DB | 1DF               |
| Options Copy 2 | 1E0 - 1FB | 1FF               |