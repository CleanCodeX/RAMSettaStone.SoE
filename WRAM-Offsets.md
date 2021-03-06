﻿# W-RAM Offsets

## W-RAM <-> S-RAM Mappings

(in order of W-RAM offset)

> [Chunk5](Chunks/Chunk05.md): [xA35|2613]  (2 bytes)      => S-RAM: [x8E|142]

> [Chunk6](Chunks/Chunk06.md): [xA3F|2623]  (13 bytes)     => S-RAM: [x90|144]

> [Chunk7](Chunks/Chunk07.md): [xA50|2640]  (4 bytes)      => S-RAM: [x9D|157]

> [Chunk12](Chunks/Chunk12.md): [xA7F|2687]  (2 bytes)     => S-RAM: [xCF|207]

> [Chunk13](Chunks/Chunk13.md): [xA89|2697]  (13 bytes)    => S-RAM: [xD1|209]

> [Chunk14](Chunks/Chunk14.md): [xA9A|2714]  (4 bytes)     => S-RAM: [xDE|222]

> [Chunk16](Chunks/Chunk16.md): [xABA|2746]  (101 bytes)   => S-RAM: [xF0|240]

> [Chunk1](Chunks/Chunk01.md): [x2210|8720]  (72 bytes)    => S-RAM: [x26|038]

> [Chunk18](Chunks/Chunk18.md): [x2258|8792]  (146 bytes)  => S-RAM: [x1F7|503]

> [Chunk19](Chunks/Chunk19.md): [x22FF|8959]  (92 bytes)   => S-RAM: [x289|649]

> [Chunk20](Chunks/Chunk20.md): [x2361|9057]  (44 bytes)   => S-RAM: [x2E5|741]

> [Chunk21](Chunks/Chunk21.md): [x2513|9491]  (32 bytes)   => S-RAM: [x311|785]

> [Chunk17](Chunks/Chunk17.md): [x2F52|12114]  (162 bytes) => S-RAM: [x155|341]

> [Chunk2](Chunks/Chunk02.md): [x4EB3|20147]  (2 bytes)    => S-RAM: [x6E|110]

> [Chunk3](Chunks/Chunk03.md): [x4ECF|20175]  (24 bytes)   => S-RAM: [x70|112]

> [Chunk4](Chunks/Chunk04.md): [x4F23|20259]  (6 bytes)    => S-RAM: [x88|136]

> [Chunk8](Chunks/Chunk08.md): [x4F29|20265]  (14 bytes)   => S-RAM: [xA1|161]

> [Chunk9](Chunks/Chunk09.md): [x4F61|20321]  (2 bytes)    => S-RAM: [xB1|177]

> [Chunk10](Chunks/Chunk10.md): [x4F7D|20349]  (24 bytes)  => S-RAM: [xAF|175]

> [Chunk11](Chunks/Chunk11.md): [x4FD1|20433]  (6 bytes)   => S-RAM: [xC9|201]

> [Chunk15](Chunks/Chunk15.md): [x4FD7|20439]  (14 bytes)  => S-RAM: [xE2|226]

All offsets belong to 7E address space. Meaning offset 0000 is located at $7E:0000

### [Chunk5](Chunks/Chunk05.md) (Boy stats)

WRAM ~	Size ~	Description

> x0A35	(2)		Max HP

### [Chunk6](Chunks/Chunk06.md) (Boy stats)

WRAM ~	Size ~	Description

> x0A3F	(2)		Attack

> x0A41	(2)		Defense

> x0A43	(2)		Magic Def

> x0A45	(2)		Evade %

> x0A47	(2)		Hit %

> x0A49	(3)		Experience 

### [Chunk7](Chunks/Chunk07.md) (Boy stats)

WRAM ~	Size ~	Description

> x0A50	(2)		Level

> x0A52	(2)		Max Chargeup

The values below are curious. As far as I can tell, after saving your game, these values will always be x4F. It seems an oversight of the game programmers, as the game copies these values from $30:4Fxx, which is open bus. The values below will always be x4F in a save file, but it seems the programmers meant to copy the values from 4Fxx.

### [Chunk12](Chunks/Chunk12.md) (Dog stats)

WRAM ~	Size ~	Description

> x0A7F	(2)		Max HP

### [Chunk13](Chunks/Chunk13.md) (Dog stats)

WRAM ~	Size ~	Description

> x0A89	(2)		Attack

> x0A8B	(2)		Defense

> x0A8D	(2)		Magic Def

> x0A8F	(2)		Evade %

> x0A91	(2)		Hit %

> x0A93	(3)		Experience

### [Chunk14](Chunks/Chunk14.md) (Dog stats)

WRAM ~	Size ~	Description

> x0A9A	(2)		Level

> x0A9C	(2)		Max Chargeup

The values below are curious. As far as I can tell, after saving your game, these values will always be x4F. It seems an oversight of the game programmers, as the game copies these values from $30:4Fxx, which is open bus. The values below will always be x4F in a save file, but it seems the programmers meant to copy the values from 4Fxx.

### [Chunk16](Chunks/Chunk16.md) (various things)

WRAM ~	Size ~	Description

> x0ABA	(2)		Current equipped weapon

> x0ABC	(2)		unknown

> x0ABE	(2)		Dog - Pointer to current Collar stats

> x0AC0	(2)		Boy - Pointer to current Armor stats

> x0AC2	(2)		Boy - Pointer to current Helmet stats

> x0AC4	(2)		Boy - Pointer to current Armband stats

> x0AC6	(3)		Money - Talons

> x0AC9	(3)		Money - Jewels

> x0ACC	(3)		Money - Gold Coins

> x0ACF	(3)		Money - Credits

> x0AD2-0B1E	x4D	Most are listed in Secret_of_Evermore:RAM_map

### [Chunk1](Chunks/Chunk01.md) (Character names)

WRAM ~	Size ~	Description

> x2210	(36)	Boy name (zero padded, must end with byte x00)

> x2234	(36)	Dog name (zero padded, must end with byte x00)

### [Chunk18](Chunks/Chunk18.md) (unknowns)

WRAM ~		Size ~	Description

> x2258-22E9	(146)	unknown

### [Chunk19](Chunks/Chunk19.md) (Alchemy ingredients and Inventory)

WRAM ~		Size ~	Description

> x22FF-235A	(92)	Most are listed in Secret_of_Evermore:RAM_map

### [20](Chunks/Chunk20.md) (unknowns)

WRAM ~		Size ~	Description

> x2361-238C	(44)	unknown

### [Chunk21](Chunks/Chunk21.md) (Trade good amounts)

WRAM ~		Size ~	Description

> x2513-2532	(32) 	Most are listed in Secret_of_Evermore:RAM_map

### [Chunk17](Chunks/Chunk17.md) (Alchemy levels and unknowns)

WRAM ~		Size ~	Description

> x2F52		(70)	Alchemy spell levels (low part)

> x2F98		(70)	Alchemy spell levels (high part)

> x2FDE-2FF3	(22)	unknown

### [Chunk2](Chunks/Chunk02.md) (Boy stats)

WRAM ~	Size ~	Description

> x4EB3	(2)		Current HP

### [Chunk3](Chunks/Chunk03.md) (Boy stats)

WRAM ~	Size ~	Description

> x4ECF	(2)		Status 1 - Status ID

> x4ED1	(2)		Status 1 - Main Timer

> x4ED3	(2)		Status 1 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

> x4ED5	(2)		Status 2 - Status ID

> x4ED7	(2)		Status 2 - Main Timer

> x4ED9	(2)		Status 2 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

> x4EDB	(2)		Status 3 - Status ID

> x4EDD	(2)		Status 3 - Main Timer

> x4EDF	(2)		Status 3 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

> x4EE1	(2)		Status 4 - Status ID

> x4EE3	(2)		Status 4 - Main Timer

> x4EE5	(2)		Status 4 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

### [Chunk4](Chunks/Chunk04.md) (unknowns)

WRAM ~	Size ~	Description

> x4F23	(2)		unknown

> x4F25	(2)		unknown

> x4F27	(2)		unknown

### [Chunk8](Chunks/Chunk08.md) (Boy stats)

WRAM	Size	Open bus	Description

> x4F29	(2)		$30:4F29	Overall boost to Attack statistic

> x4F2B	(2)		$30:4F2B	Overall boost to Defense statistic

> x4F2D	(2)		$30:4F2D	Overall boost to Evade % statistic

> x4F2F	(2)		$30:4F2F	Overall boost to Hit % statistic

> x4F31	(2)		$30:4F31	Overall boost to Magic Defense statistic

> x4F33	(2)		$30:?		Last damage taken.

> x4F35	(2)		$30:4F35	Regenerate (Horace) or Pixie Dust protection in effect

### [Chunk9](Chunks/Chunk09.md) (Dog stats)

WRAM ~	Size ~	Description

> x4F61	(2)		Current HP

### [Chunk10](Chunks/Chunk10.md) (Dog stats)

WRAM ~	Size ~	Description

> x4F7D	(2)		Status 1 - Status ID

> x4F7F	(2)		Status 1 - Main Timer

> x4F81	(2)		Status 1 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

> x4F83	(2)		Status 2 - Status ID

> x4F85	(2)		Status 2 - Main Timer

> x4F87	(2)		Status 2 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

> x4F89	(2)		Status 3 - Status ID

> x4F8B	(2)		Status 3 - Main Timer

> x4F8D	(2)		Status 3 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

> x4F8F	(2)		Status 4 - Status ID

> x4F91	(2)		Status 4 - Main Timer

> x4F93	(2)		Status 4 - Boost provided to statistic(s), OR Time since/until last/next damage/healing interval

### [Chunk11](Chunks/Chunk11.md) (unknowns)

WRAM ~	Size ~	Description

> x4FD1	(2)		unknown

> x4FD3	(2)		unknown

> x4FD5	(2)		unknown

### [Chunk15](Chunks/Chunk15.md) (Boy stats)

WRAM ~	Size ~	Description

> x4FD7	(2)		Overall boost to Attack statistic

> x4FD9	(2)		Overall boost to Defense statistic

> x4FDB	(2)		Overall boost to Evade % statistic

> x4FDD	(2)		Overall boost to Hit % statistic

> x4FDF	(2)		Overall boost to Magic Defense statistic

> x4FE1	(2)		Last damage taken.

> x4FE3	(2)		Regenerate (Horace) or Pixie Dust protection in effect
