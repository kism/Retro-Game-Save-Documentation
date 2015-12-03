#Super Mario 64

Save type: eeprom 512 bytes

The end of a section in the save area is marked by 0x44 0x41 0x00 0xXX, 0xXX being the 8 bit checksum, each save takes up two sections which contain (hopefully) the same data.

| Thing          | Save Data Range | Checksum Range | End of Segment Indicator | Checksum location |
|----------------|-----------------|----------------|--------------------------|-------------------|
| Save 1 Copy 1  | 000 - 033       | 000 - 035      | 034 - 037                | 037               |
| Save 1 Copy 2  | 038 - 06B       | 038 - 06D      | 06C - 06F                | 06F               |
| Save 2 Copy 1  | 070 - 0A3       | 070 - 0A5      | 0A4 - 0A7                | 0A7               |
| Save 2 Copy 2  | 0A8 - 0DB       | 0A8 - 0DD      | 0DC - 0DF                | 0DF               |
| Save 3 Copy 1  | 0E0 - 113       | 0E0 - 115      | 114 - 117                | 117               |
| Save 3 Copy 2  | 118 - 14B       | 118 - 14D      | 14C - 14F                | 14F               |
| Save 4 Copy 1  | 150 - 183       | 150 - 185      | 184 - 187                | 187               |
| Save 4 Copy 2  | 188 - 1BB       | 188 - 1BD      | 1BC - 1BF                | 1BF               |
| Options Copy 1 | 1C0 - 1DB       | 1C0 - 1DD      | 1DC - 1DF                | 1DF               |
| Options Copy 2 | 1E0 - 1FB       | 1E0 - 1FD      | 1FC - 1FF                | 1FF               |
