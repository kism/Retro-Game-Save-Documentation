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

Unconfirmed 8 bit checksum(?), two per savegame, indicated by 0x44 0x41 0x00 0xXX, 0xXX being the 8 bit checksum.

Save 1: 000 - 06F, Checksums: 034 - 037, 06C - 06F

Save 2: 070 - 0DF, Checksums: 074 - 037, 7EC - 7EF 

Save 3: 0E0 - 14F, Checksums: 114 - 117, 14C - 14F

Save 4: 150 - 1BF, Checksums: 184 - 187, 1BC - 1BF

Options: 1C0 - 1FF

### eeprom 16kbit
Big Endian

16kbit / 2048 bytes

### SRAM
256kbit / 32768 bytes

### FlashRAM

### Controller Pack
