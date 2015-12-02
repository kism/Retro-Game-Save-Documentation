# Nintendo 64
### eeprom 4kbit
Big Endian

4kbit / 512 bytes

**Mario Party 2**

Gold: 7A-7B

16 bit checksum at 1F8 - 1F9, checks 008 - IEF

**Mario Kart**

Unconfirmed checksum at either 1F6 - 1F7 or 1FE - 1FF, unknown range

**Super Mario 64**

The end of a section in the save area is marked by 0x44 0x41 0x00 0xXX, 0xXX being the 8 bit checksum, each save takes up two sections which contain (hopefully) the same data.

Save 1 Copy 1: 000 - 035 | Checksum at 037

Save 1 Copy 2: 038 - 06D | Checksum at 06F

Save 2 Copy 1: 070 - 0A5 | Checksum at 0A7

Save 2 Copy 2: 0A8 - 0DD | Checksum at 0DF

Save 3 Copy 1: 0E0 - 115 | Checksum at 117

Save 3 Copy 2: 118 - 14D | Checksum at 14F

Save 4 Copy 1: 150 - 185 | Checksum at 187

Save 4 Copy 2: 188 - 1BD | Checksum at 1BF

Options: 1C0 - 1FF

### eeprom 16kbit
Big Endian

16kbit / 2048 bytes

### SRAM
256kbit / 32768 bytes

### FlashRAM

### Controller Pack
