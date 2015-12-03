# Grandia II

###Currency 

All values are Little Endian 32 bit Unsigned Integer

| Value         | Range     |
|---------------|-----------|
| Gold          | 2C0 - 2C3 |
| Special Coins | 2C4 - 2C7 |
| Magic Coins   | 2C8 - 2CB |

###Inventory

All values are 8 bit Unsigned Integer

**Consumables**

| Item           | Offset |
|----------------|--------|
| Miracle Elixir | B2D    |
| Hero's Elixir  | B2E    |
| Mystic Potion  | B19    |
| Indigo Potion  | B4B    |
| Golden Potion  | B41    |
| Panacea        | B30    |

**Weapons**

| Item              | Offset |
|-------------------|--------|
| Granasaber        | BE1    |
| Holy Ghost Staff  | BFF    |
| Black Angel Bow   | C1D    |
| Brave Dirk        | C3B    |
| Soul Eater        | C3F    |
| Phoenix Ring      | C59    |
| Leo Rex Battleaxe | C77    |

**Armor**

| Item             | Offset |
|------------------|--------|
| Holy Sword Armor | CA9    |
| Hero's Cuirass   | CBD    |
| Valcyre Dress    | CC7    |
| Priestess Robe   | CD1    |
| Sun Robe         | CDB    |

**Headgear**

| Item              | Offset |
|-------------------|--------|
| God of War Helm   | CEF    |
| Holy Crown        | D03    |
| Illusion Bandanna | D17    |
| Sages Hat         | D2B    |

**Footwear**

| Item           | Offset |
|----------------|--------|
| Lion Boots     | D3F    |
| Glass Slippers | D53    |
| Ogre Shoes     | D5D    |

**Accessories**

| Item            | Offset |
|-----------------|--------|
| Demon Necklace  | D7C    |
| Energy Charm    | D7E    |
| Soul of Asura   | D80    |
| Dragon Scales   | D88    |
| Meteor Earrings | D8C    |
| Jet Black Cape  | D98    |
| King's Pride    | D84    |
| Mana Crystals   | D7B    |
| Angel's Ring    | D82    |
| Mystic Veil     | DAD    |
| Heracles Belt   | DC1    |
| Shoguns Brace   | DC5    |
| Sonic Belt      | DCA    |

**Valuables**

| Item             | Offset |
|------------------|--------|
| Debug HP/MP/SC + | AB5    |
| Debug Stats +    | AB6    |
| Seed of Life     | AF1    |
| Seed of Spells   | AF2    |
| Seed of Moves    | AF3    |
| Seed of Power    | AF4    |
| Seed of Defense  | AF5    |
| Seed of Swift    | AF6    |
| Seed of Running  | AF7    |
| Seed of Magic    | AF8    |
| Seed of Psyche   | AF9    |
| All-Around Seed  | AFA    |
| Omnipotent Seed  | AFB    |
| Lore of Moves    | AFC    |
| Lore of Magic    | AFD    |
| Miracle Scales   | B05    |
| Soul of a Hero   | B06    |
| Astral Miracle   | B07    |
| Ethereal Miracle | B08    |

**Books**

| Item             | Offset |
|------------------|--------|
| Adventure Book   | AE7    |
| Book of Wizards  | AE8    |
| Book of Warriors | AE9    |
| Book of Priests  | AEA    |
| Book of Gales    | AEB    |
| Book of Swords   | AEC    |
| Book of War      | AED    |
| Book of Sages    | AEE    |
| Book of Learning | AEF    |

**Eggs**

| Item        | Offset |
|-------------|--------|
| Holy Egg    | D71    |
| Chaos Egg   | D72    |
| Mist Egg    | D73    |
| Gravity Egg | D74    |
| Soul Egg    | D75    |
| Star Egg    | D76    |
| Tutor Egg   | D77    |
| Change Egg  | D78    |
| Fairy Egg   | D79    |
| Dragon Egg  | D7A    |

###Character Experience

All values are Little Endian 32 bit Unsigned Integer

| Character | Current Exp | Remaining Exp |
|-----------|-------------|---------------|
| Ryudo     | 31C - 31F   | 320 - 323     |
| Elena     | 388 - 38B   | 38C - 38F     |
| Millenia  | 3F4 - 3F7   | 3F8 - 3FB     |
| Roan      | 460 - 463   | 464 - 467     |
| Mareg     | 538 - 53B   | 53C - 53F     |
| Tio       | 3CC - 4CF   | 4D0 - 4D3     |

###Savegame Metadata

| Item            | Range     | Data Type                             |
|-----------------|-----------|---------------------------------------|
| Play Time       | 290 - 293 | Little Endian 32 bit Unsigned Integer |
| Save Point Name | 294 - 2B3 | Array of ASCII                        |
