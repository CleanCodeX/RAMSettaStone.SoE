﻿# Secret Of Evermore ~ S-RAM - Map

Size: 8,192 bytes (8 KiB)

* [Offsets overview](SRAM-Offsets.md)
* [Unknowns](SRAM-Unknowns.md)

### Pre-save slot
> byte AudioMode : (0) => mono, (1) => stereo

> byte LastSaveSlotId : (0) => slot 1, (2) => slot 2, (4) => slot 3, (6) => slot 4)

### Save slots 1-4
> [SaveSlot](SaveSlot.md)[]  (817 bytes each)

### Post-save slot
> byte[] Unknown1 (4,922 bytes - probably completely unused space)
