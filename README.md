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

The end of a section in the save area is marked by 0x44 0x41 0x00 0xXX, 0xXX being the 8 bit checksum, each save takes up two sections.

Save 1: 000 - 06F | Checksum 1: 037, checks 000 - 035 | Checksum 2: 06F, checks 

Save 2: 070 - 0DF | Checksum 1: 037, checks  | Checksum 2: 7EF, checks  

Save 3: 0E0 - 14F | Checksum 1: 117, checks  | Checksum 2: 14F, checks 

Save 4: 150 - 1BF | Checksum 1: 187, checks  | Checksum 2: 1BF, checks 

Options: 1C0 - 1FF

### eeprom 16kbit
Big Endian

16kbit / 2048 bytes

### SRAM
256kbit / 32768 bytes

### FlashRAM

### Controller Pack
