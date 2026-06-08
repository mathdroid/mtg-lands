# Two-color fixing lands, by guild

Generated from the data in [`all-pairs.json`](all-pairs.json) (`mtg-lands --all-pairs --json`). For each guild, every Commander-legal land whose color identity fits the pair and that taps for both colors.

Lands are grouped by **how they enter the battlefield** - there are no quality tiers. Three tables per guild:

- **Enters untapped** - never enters tapped (true duals, pain, filter, verge, ...).
- **Conditional** - enters tapped unless a condition is met (shock, check, fast, slow, battle, bond, reveal, catch-up).
- **Enters tapped** - always tapped (temples, surveil lands, gates, trilands, ...).

Columns: **Cycle** (the named land cycle, or `-` if it matches none), **Card**, **Tags**, **EDHREC** rank, **Price** (USD; `RL` = Reserved List, no current nonfoil price). Within each table cards are ordered by a popularity+price score.

**Tags** are cross-cutting attributes: `searchable` (has basic land types, so a fetchland can find it), `filter`, `pain`, `snow`, `manland`, `cycling`, `mdfc`, `lifegain`, `any-color`.

Each guild also matches ~132 **any-color** rainbow lands (City of Brass, Command Tower, Reflecting Pool, ...). They recur in every identity, so they are listed once at the end rather than per guild.

---

## Azorius (WU)

### Enters untapped (11)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Tundra | searchable | 368 | RL |
| Verge | Floodfarm Verge | - | 713 | $8.31 |
| Filter | Mystic Gate | filter | 897 | $4.09 |
| Pathway (MDFC) | Hengegate Pathway // Mistgate Pathway | mdfc | 1151 | $5.36 |
| - | Nimbus Maze | - | 1850 | $6.85 |
| Pain | Adarkar Wastes | pain | 159 | $0.34 |
| Filter | Skycloud Expanse | filter | 349 | $0.23 |
| Depletion | Land Cap | - | 27684 | $1.01 |
| Storage | Calciform Pools | - | 11254 | $0.30 |
| Locked | Cloudcrest Lake | - | 22428 | $0.32 |
| Locked | Thalakos Lowlands | - | 24553 | RL |

### Conditional (enters tapped unless a condition is met) (10)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Bond (crowd) | Sea of Clouds | - | 166 | $17.83 |
| Shock | Hallowed Fountain | searchable | 65 | $8.77 |
| Slow | Deserted Beach | - | 277 | $5.43 |
| Check | Glacial Fortress | - | 99 | $0.38 |
| Battle/Tango | Prairie Stream | searchable | 105 | $0.30 |
| Fast | Seachrome Coast | - | 1212 | $0.36 |
| Reveal | Port Town | - | 345 | $0.23 |
| - | Wanderwine Hub | - | 13985 | $1.76 |
| - | Abandoned Campground | - | 9299 | $0.27 |
| - | Fortified Beachhead | - | 12169 | $0.24 |

### Enters tapped (22)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Meticulous Archive | searchable | 704 | $11.53 |
| Scry/Temple | Temple of Enlightenment | - | 302 | $0.29 |
| Creature land | Restless Anchorage | manland | 3800 | $1.18 |
| Bridge (artifact) | Razortide Bridge | - | 1034 | $0.32 |
| Bounce/Karoo | Azorius Chancery | - | 437 | $0.27 |
| Snow dual | Glacial Floodplain | searchable, snow | 3843 | $0.40 |
| Cycling/Bicycle | Irrigated Farmland | searchable, cycling | 805 | $0.25 |
| Creature land | Celestial Colonnade | manland | 5506 | $0.58 |
| Gain/Refuge | Sejiri Refuge | lifegain | 4736 | $0.37 |
| - | Idyllic Beachfront | searchable | 2253 | $0.24 |
| Gain/Refuge | Tranquil Cove | lifegain | 1075 | $0.13 |
| Snow dual | Boreal Shelf | snow | 11611 | $0.94 |
| Guildgate | Azorius Guildgate | - | 1994 | $0.14 |
| - | Study | - | 13190 | $0.41 |
| MDFC spell/land | Suppression Ray // Orderly Plaza | mdfc | 7159 | $0.29 |
| - | Lonely Arroyo | - | 6451 | $0.27 |
| - | Sharlayan, Nation of Scholars | - | 5355 | $0.17 |
| - | North Pole Gates | - | 8532 | $0.22 |
| - | Meandering River | - | 7441 | $0.13 |
| - | Skybridge Towers | - | 7561 | $0.13 |
| - | Coastal Tower | - | 12058 | RL |
| Campus | University Campus | - | 10436 | $0.14 |

---

## Dimir (UB)

### Enters untapped (12)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Underground Sea | searchable | 299 | RL |
| Verge | Gloomlake Verge | - | 633 | $11.00 |
| Pain | Underground River | pain | 152 | $1.49 |
| Filter | Sunken Ruins | filter | 1047 | $9.12 |
| Pathway (MDFC) | Clearwater Pathway // Murkwater Pathway | mdfc | 752 | $4.30 |
| Tainted | Tainted Isle | - | 497 | $0.81 |
| Filter | Darkwater Catacombs | filter | 313 | $0.34 |
| - | River of Tears | - | 2561 | $0.31 |
| Depletion | River Delta | - | 26522 | $1.00 |
| Storage | Dreadship Reef | - | 9504 | $0.36 |
| Locked | Waterveil Cavern | - | 22982 | $0.21 |
| Locked | Rootwater Depths | - | 23391 | RL |

### Conditional (enters tapped unless a condition is met) (9)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Bond (crowd) | Morphic Pool | - | 139 | $31.32 |
| Shock | Watery Grave | searchable | 52 | $11.11 |
| Slow | Shipwreck Marsh | - | 231 | $7.43 |
| Check | Drowned Catacomb | - | 111 | $3.43 |
| Fast | Darkslick Shores | - | 1367 | $2.10 |
| Reveal | Choked Estuary | - | 289 | $0.38 |
| Battle/Tango | Sunken Hollow | searchable | 86 | $0.32 |
| - | Secluded Glen | - | 4911 | $3.67 |
| - | Murky Sewer | - | 8704 | $0.19 |

### Enters tapped (22)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Undercity Sewers | searchable | 433 | $17.74 |
| Bounce/Karoo | Dimir Aqueduct | - | 340 | $0.37 |
| Bridge (artifact) | Mistvault Bridge | - | 1741 | $0.63 |
| MDFC spell/land | Waterlogged Teachings // Inundated Archive | mdfc | 1379 | $0.42 |
| Creature land | Restless Reef | manland | 3723 | $2.68 |
| Cycling/Bicycle | Fetid Pools | searchable, cycling | 862 | $0.32 |
| Scry/Temple | Temple of Deceit | - | 333 | $0.25 |
| - | Contaminated Aquifer | searchable | 2125 | $0.33 |
| Snow dual | Ice Tunnel | searchable, snow | 3980 | $0.46 |
| Creature land | Creeping Tar Pit | manland | 2852 | $0.32 |
| Gain/Refuge | Jwar Isle Refuge | lifegain | 4336 | $0.36 |
| Gain/Refuge | Dismal Backwater | lifegain | 956 | $0.18 |
| Snow dual | Frost Marsh | snow | 11612 | $0.78 |
| Guildgate | Dimir Guildgate | - | 1707 | $0.11 |
| - | Soured Springs | - | 5387 | $0.29 |
| - | Waterfront District | - | 6581 | $0.30 |
| - | Secret Passage | - | 14335 | $0.40 |
| - | Submerged Boneyard | - | 4934 | $0.23 |
| - | Treno, Dark City | - | 4908 | $0.20 |
| - | Serpent's Pass | - | 9614 | $0.26 |
| - | Salt Marsh | - | 11197 | $0.25 |
| - | Sinister Hideout | - | 8391 | $0.15 |

---

## Rakdos (BR)

### Enters untapped (12)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Badlands | searchable | 387 | RL |
| Verge | Blazemire Verge | - | 565 | $8.79 |
| Pain | Sulfurous Springs | pain | 158 | $1.02 |
| Pathway (MDFC) | Blightstep Pathway // Searstep Pathway | mdfc | 813 | $5.29 |
| Filter | Graven Cairns | filter | 583 | $3.50 |
| - | Mount Doom | - | 1198 | $7.86 |
| Filter | Shadowblood Ridge | filter | 423 | $0.68 |
| Tainted | Tainted Peak | - | 500 | $0.48 |
| Depletion | Lava Tubes | - | 27435 | $1.01 |
| Storage | Molten Slagheap | - | 8275 | $0.12 |
| Locked | Lantern-Lit Graveyard | - | 22278 | $0.20 |
| Locked | Cinder Marsh | - | 23086 | RL |

### Conditional (enters tapped unless a condition is met) (9)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Bond (crowd) | Luxury Suite | - | 163 | $28.64 |
| Shock | Blood Crypt | searchable | 69 | $10.28 |
| Slow | Haunted Ridge | - | 275 | $8.05 |
| Check | Dragonskull Summit | - | 87 | $0.48 |
| Fast | Blackcleave Cliffs | - | 1067 | $1.58 |
| Battle/Tango | Smoldering Marsh | searchable | 95 | $0.36 |
| Reveal | Foreboding Ruins | - | 326 | $0.32 |
| - | Auntie's Hovel | - | 11043 | $7.47 |
| - | Razortrap Gorge | - | 8122 | $0.27 |

### Enters tapped (21)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Raucous Theater | searchable | 562 | $11.29 |
| Bridge (artifact) | Drossforge Bridge | - | 2168 | $1.17 |
| Bounce/Karoo | Rakdos Carnarium | - | 476 | $0.34 |
| Scry/Temple | Temple of Malice | - | 416 | $0.26 |
| - | Jagged Barrens | - | 3392 | $0.42 |
| Cycling/Bicycle | Canyon Slough | searchable, cycling | 703 | $0.25 |
| - | Geothermal Bog | searchable | 2271 | $0.29 |
| Creature land | Restless Vents | manland | 4767 | $0.41 |
| Gain/Refuge | Akoum Refuge | lifegain | 3595 | $0.36 |
| Gain/Refuge | Bloodfell Caves | lifegain | 893 | $0.19 |
| Snow dual | Sulfurous Mire | searchable, snow | 5363 | $0.33 |
| Creature land | Lavaclaw Reaches | manland | 7449 | $0.37 |
| Guildgate | Rakdos Guildgate | - | 1910 | $0.09 |
| Snow dual | Tresserhorn Sinks | snow | 19154 | $0.51 |
| - | Vector, Imperial Capital | - | 5499 | $0.21 |
| - | Billiard Room | - | 13859 | $0.32 |
| - | Cinder Barrens | - | 6082 | $0.21 |
| - | Urborg Volcano | - | 10913 | $0.28 |
| - | Boiling Rock Prison | - | 8359 | $0.25 |
| - | Tramway Station | - | 6896 | $0.13 |
| - | Ominous Asylum | - | 8755 | $0.22 |

---

## Gruul (RG)

### Enters untapped (11)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Taiga | searchable | 440 | RL |
| Verge | Thornspire Verge | - | 806 | $5.05 |
| Filter | Fire-Lit Thicket | filter | 1251 | $7.70 |
| Pathway (MDFC) | Cragcrown Pathway // Timbercrown Pathway | mdfc | 1051 | $3.53 |
| Pain | Karplusan Forest | pain | 220 | $0.39 |
| Reverse-pain | Grove of the Burnwillows | - | 3339 | $7.52 |
| Filter | Mossfire Valley | filter | 522 | $0.32 |
| Depletion | Timberline Ridge | - | 29108 | $0.99 |
| Locked | Pinecrest Ridge | - | 23944 | $0.21 |
| Storage | Fungal Reaches | - | 15038 | $0.13 |
| Locked | Mogg Hollows | - | 24869 | RL |

### Conditional (enters tapped unless a condition is met) (8)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Shock | Stomping Ground | searchable | 68 | $7.58 |
| Bond (crowd) | Spire Garden | - | 187 | $5.00 |
| Slow | Rockfall Vale | - | 216 | $2.10 |
| Battle/Tango | Cinder Glade | searchable | 85 | $0.35 |
| Check | Rootbound Crag | - | 129 | $0.33 |
| Fast | Copperline Gorge | - | 1463 | $0.47 |
| Reveal | Game Trail | - | 367 | $0.30 |
| - | Bleeding Woods | - | 9477 | $0.22 |

### Enters tapped (22)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Commercial District | searchable | 644 | $8.29 |
| MDFC spell/land | Stump Stomp // Burnwillow Clearing | mdfc | 1250 | $0.39 |
| Bounce/Karoo | Gruul Turf | - | 413 | $0.31 |
| Snow dual | Highland Forest | searchable, snow | 3139 | $0.46 |
| Scry/Temple | Temple of Abandon | - | 484 | $0.26 |
| Cycling/Bicycle | Sheltered Thicket | searchable, cycling | 627 | $0.25 |
| Creature land | Restless Ridgeline | manland | 4328 | $0.46 |
| - | Wooded Ridgeline | searchable | 1724 | $0.25 |
| Bridge (artifact) | Slagwoods Bridge | - | 3206 | $0.32 |
| - | Bristling Backwoods | - | 3281 | $0.28 |
| Gain/Refuge | Rugged Highlands | lifegain | 1353 | $0.17 |
| Creature land | Raging Ravine | manland | 2653 | $0.22 |
| Guildgate | Gruul Guildgate | - | 2028 | $0.14 |
| Gain/Refuge | Kazandu Refuge | lifegain | 5735 | $0.26 |
| - | Gongaga, Reactor Town | - | 5963 | $0.26 |
| - | Dining Room | - | 15033 | $0.34 |
| - | Omashu City | - | 7704 | $0.25 |
| Snow dual | Highland Weald | snow | 16392 | $0.32 |
| - | Timber Gorge | - | 8573 | $0.25 |
| - | Racers' Ring | - | 7689 | $0.13 |
| - | Savage Mansion | - | 10435 | $0.13 |
| - | Shivan Oasis | - | 13040 | $0.15 |

---

## Selesnya (GW)

### Enters untapped (12)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Savannah | searchable | 472 | RL |
| Verge | Hushwood Verge | - | 757 | $7.57 |
| Pain | Brushland | pain | 240 | $1.50 |
| Filter | Wooded Bastion | filter | 2018 | $16.30 |
| Pathway (MDFC) | Branchloft Pathway // Boulderloft Pathway | mdfc | 1132 | $3.52 |
| Horizon/Canopy | Horizon Canopy | - | 1664 | $4.33 |
| Filter | Sungrass Prairie | filter | 439 | $0.23 |
| - | Riftstone Portal | - | 10930 | $2.68 |
| Depletion | Veldt | - | 28576 | $1.20 |
| Storage | Saltcrusted Steppe | - | 12107 | $0.34 |
| Locked | Tranquil Garden | - | 22998 | $0.20 |
| Locked | Vec Townships | - | 25119 | RL |

### Conditional (enters tapped unless a condition is met) (8)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Bond (crowd) | Bountiful Promenade | - | 213 | $17.89 |
| Shock | Temple Garden | searchable | 82 | $8.08 |
| Slow | Overgrown Farmland | - | 290 | $2.61 |
| Check | Sunpetal Grove | - | 136 | $0.55 |
| Fast | Razorverge Thicket | - | 1477 | $0.62 |
| Battle/Tango | Canopy Vista | searchable | 103 | $0.25 |
| Reveal | Fortified Village | - | 342 | $0.26 |
| - | Etched Cornfield | - | 10622 | $0.16 |

### Enters tapped (22)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Lush Portico | searchable | 709 | $6.00 |
| Scry/Temple | Temple of Plenty | - | 479 | $0.28 |
| Cycling/Bicycle | Scattered Groves | searchable, cycling | 963 | $0.29 |
| MDFC spell/land | Strength of the Harvest // Haven of the Harvest | mdfc | 1920 | $0.34 |
| Bounce/Karoo | Selesnya Sanctuary | - | 540 | $0.26 |
| Snow dual | Arctic Treeline | searchable, snow | 3605 | $0.37 |
| Creature land | Restless Prairie | manland | 5104 | $0.36 |
| Bridge (artifact) | Thornglint Bridge | - | 4447 | $0.34 |
| - | Radiant Grove | searchable | 1473 | $0.20 |
| Gain/Refuge | Blossoming Sands | lifegain | 1064 | $0.16 |
| Gain/Refuge | Graypelt Refuge | lifegain | 2811 | $0.25 |
| Snow dual | Arctic Flats | snow | 13276 | $1.88 |
| Guildgate | Selesnya Guildgate | - | 1955 | $0.14 |
| Creature land | Stirring Wildwood | manland | 7143 | $0.34 |
| - | Creosote Heath | - | 3664 | $0.23 |
| - | Kyoshi Village | - | 7835 | $0.27 |
| - | Windurst, Federation Center | - | 5600 | $0.20 |
| - | Botanical Plaza | - | 6833 | $0.24 |
| - | Conservatory | - | 14763 | $0.34 |
| - | Tranquil Expanse | - | 7851 | $0.12 |
| - | Elfhame Palace | - | 11187 | $0.19 |
| - | Suburban Sanctuary | - | 10150 | $0.15 |

---

## Orzhov (WB)

### Enters untapped (8)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Scrubland | searchable | 386 | RL |
| Verge | Bleachbone Verge | - | 909 | $11.02 |
| Pathway (MDFC) | Brightclimb Pathway // Grimclimb Pathway | mdfc | 748 | $5.78 |
| Horizon/Canopy | Silent Clearing | - | 1604 | $6.65 |
| Pain | Caves of Koilos | pain | 125 | $0.51 |
| Filter | Fetid Heath | filter | 350 | $0.39 |
| Tainted | Tainted Field | - | 421 | $0.35 |
| Filter | Desolate Mire | filter | 959 | $0.29 |

### Conditional (enters tapped unless a condition is met) (9)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Bond (crowd) | Vault of Champions | - | 169 | $18.12 |
| Shock | Godless Shrine | searchable | 60 | $10.29 |
| Slow | Shattered Sanctum | - | 294 | $1.54 |
| Fast | Concealed Courtyard | - | 1146 | $1.25 |
| Check | Isolated Chapel | - | 93 | $0.33 |
| Reveal | Shineshadow Snarl | - | 420 | $0.31 |
| Catch-up | Turbulent Moor | searchable | 6216 | $5.88 |
| Battle/Tango | Eclipsed Steppe | searchable | 6475 | $2.44 |
| - | Neglected Manor | - | 8190 | $0.15 |

### Enters tapped (21)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Shadowy Backstreet | searchable | 561 | $12.19 |
| Bridge (artifact) | Goldmire Bridge | - | 2097 | $1.57 |
| Bounce/Karoo | Orzhov Basilica | - | 378 | $0.31 |
| Creature land | Restless Fortress | manland, lifegain | 4236 | $0.74 |
| MDFC spell/land | Glasswing Grace // Age-Graced Chapel | mdfc | 2842 | $0.38 |
| Scry/Temple | Temple of Silence | - | 276 | $0.23 |
| Snow dual | Snowfield Sinkhole | searchable, snow | 3740 | $0.40 |
| - | Sunlit Marsh | searchable | 1720 | $0.21 |
| Gain/Refuge | Scoured Barrens | lifegain | 706 | $0.12 |
| Creature land | Shambling Vent | manland | 5485 | $0.35 |
| Cycling/Bicycle | Umbral Expanse | searchable, cycling | 10495 | $0.58 |
| Guildgate | Orzhov Guildgate | - | 1849 | $0.13 |
| - | Forsaken Sanctuary | - | 6150 | $0.30 |
| - | Forlorn Flats | - | 4847 | $0.26 |
| - | Ballroom | - | 12560 | $0.38 |
| Campus | Silverquill Campus | - | 6158 | $0.25 |
| - | Insomnia, Crown City | - | 5608 | $0.22 |
| - | Misty Palms Oasis | - | 10875 | $0.20 |
| - | Forum of Amity | - | 12077 | $0.15 |
| Gain/Refuge | Foot Headquarters | lifegain | 13832 | $0.12 |
| Pain | Salt Flats | pain | 20054 | RL |

---

## Izzet (UR)

### Enters untapped (7)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Volcanic Island | searchable | 346 | RL |
| Verge | Riverpyre Verge | - | 1020 | $24.40 |
| Horizon/Canopy | Fiery Islet | - | 816 | $6.03 |
| Pathway (MDFC) | Riverglide Pathway // Lavaglide Pathway | mdfc | 848 | $5.71 |
| Pain | Shivan Reef | pain | 117 | $0.36 |
| Filter | Cascade Bluffs | filter | 312 | $0.39 |
| Filter | Ferrous Lake | filter | 778 | $0.37 |

### Conditional (enters tapped unless a condition is met) (9)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Shock | Steam Vents | searchable | 67 | $12.92 |
| Bond (crowd) | Training Center | - | 149 | $16.74 |
| Slow | Stormcarved Coast | - | 202 | $2.02 |
| Fast | Spirebluff Canal | - | 1571 | $6.38 |
| Check | Sulfur Falls | - | 83 | $0.33 |
| Reveal | Frostboil Snarl | - | 344 | $0.28 |
| Catch-up | Turbulent Springs | searchable | 6706 | $5.48 |
| Battle/Tango | Scorched Geyser | searchable | 7130 | $2.73 |
| - | Peculiar Lighthouse | - | 8570 | $0.18 |

### Enters tapped (21)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Thundering Falls | searchable | 625 | $16.24 |
| Bounce/Karoo | Izzet Boilerworks | - | 393 | $0.36 |
| Bridge (artifact) | Silverbluff Bridge | - | 1165 | $0.33 |
| Snow dual | Volatile Fjord | searchable, snow | 4830 | $0.89 |
| Scry/Temple | Temple of Epiphany | - | 270 | $0.18 |
| Gain/Refuge | Swiftwater Cliffs | lifegain | 1006 | $0.16 |
| - | Molten Tributary | searchable | 2491 | $0.23 |
| - | Eroded Canyon | - | 3541 | $0.28 |
| MDFC spell/land | Rush of Inspiration // Crackling Falls | mdfc | 4959 | $0.30 |
| Guildgate | Izzet Guildgate | - | 1673 | $0.13 |
| Cycling/Bicycle | Coastal Peak | searchable, cycling | 11070 | $0.53 |
| - | Library | - | 13311 | $0.39 |
| Campus | Prismari Campus | - | 5636 | $0.23 |
| - | Baron, Airship Kingdom | - | 4863 | $0.22 |
| Creature land | Restless Spire | manland | 4725 | $0.20 |
| Creature land | Wandering Fumarole | manland | 7532 | $0.28 |
| - | Airship Engine Room | - | 7430 | $0.23 |
| - | Highland Lake | - | 6123 | $0.17 |
| - | Spectacle Summit | - | 11952 | $0.17 |
| Gain/Refuge | TCRI Building | lifegain | 16400 | $0.14 |
| Pain | Caldera Lake | pain | 19747 | RL |

---

## Golgari (BG)

### Enters untapped (8)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Bayou | searchable | 430 | RL |
| Verge | Wastewood Verge | - | 1123 | $12.09 |
| Pathway (MDFC) | Darkbore Pathway // Slitherbore Pathway | mdfc | 1113 | $6.50 |
| Horizon/Canopy | Nurturing Peatland | - | 1545 | $7.04 |
| Pain | Llanowar Wastes | pain | 137 | $0.47 |
| Filter | Twilight Mire | filter | 381 | $0.44 |
| Filter | Viridescent Bog | filter | 727 | $0.36 |
| Tainted | Tainted Wood | - | 424 | $0.32 |

### Conditional (enters tapped unless a condition is met) (10)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Shock | Overgrown Tomb | searchable | 70 | $9.94 |
| Bond (crowd) | Undergrowth Stadium | - | 175 | $5.51 |
| Slow | Deathcap Glade | - | 398 | $1.62 |
| Check | Woodland Cemetery | - | 114 | $0.37 |
| Fast | Blooming Marsh | - | 1498 | $1.79 |
| Battle/Tango | Vernal Fen | searchable | 984 | $0.72 |
| Reveal | Necroblossom Snarl | - | 530 | $0.38 |
| - | Gilt-Leaf Palace | - | 5003 | $10.44 |
| Catch-up | Turbulent Fen | searchable | 5985 | $7.54 |
| - | Strangled Cemetery | - | 8565 | $0.24 |

### Enters tapped (21)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Underground Mortuary | searchable | 470 | $16.13 |
| MDFC spell/land | Revitalizing Repast // Old-Growth Grove | mdfc | 737 | $0.98 |
| Bounce/Karoo | Golgari Rot Farm | - | 316 | $0.32 |
| Creature land | Restless Cottage | manland | 3080 | $2.40 |
| Snow dual | Woodland Chasm | searchable, snow | 2858 | $0.60 |
| - | Haunted Mire | searchable | 1207 | $0.31 |
| Scry/Temple | Temple of Malady | - | 343 | $0.24 |
| Cycling/Bicycle | Festering Thicket | searchable, cycling | 2297 | $0.34 |
| Bridge (artifact) | Darkmoss Bridge | - | 2519 | $0.33 |
| Creature land | Hissing Quagmire | manland | 6720 | $0.87 |
| Gain/Refuge | Jungle Hollow | lifegain | 742 | $0.17 |
| Guildgate | Golgari Guildgate | - | 1504 | $0.12 |
| - | Festering Gulch | - | 4892 | $0.29 |
| Campus | Witherbloom Campus | - | 6689 | $0.29 |
| - | Gohn, Town of Ruin | - | 5946 | $0.21 |
| - | Foul Orchard | - | 5065 | $0.18 |
| - | Foggy Bottom Swamp | - | 10076 | $0.21 |
| - | Lounge | - | 16047 | $0.24 |
| - | Titan's Grave | - | 10567 | $0.19 |
| Gain/Refuge | Illegitimate Business | lifegain | 13696 | $0.16 |
| Pain | Pine Barrens | pain | 20742 | RL |

---

## Boros (RW)

### Enters untapped (7)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Plateau | searchable | 456 | RL |
| Verge | Sunbillow Verge | - | 965 | $10.98 |
| Pathway (MDFC) | Needleverge Pathway // Pillarverge Pathway | mdfc | 843 | $5.30 |
| Pain | Battlefield Forge | pain | 123 | $0.60 |
| Horizon/Canopy | Sunbaked Canyon | - | 1475 | $4.25 |
| Filter | Rugged Prairie | filter | 296 | $0.32 |
| Filter | Sunscorched Divide | filter | 857 | $0.32 |

### Conditional (enters tapped unless a condition is met) (10)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Shock | Sacred Foundry | searchable | 78 | $11.04 |
| Bond (crowd) | Spectator Seating | - | 171 | $17.12 |
| Slow | Sundown Pass | - | 291 | $2.20 |
| Fast | Inspiring Vantage | - | 1465 | $1.34 |
| Battle/Tango | Radiant Summit | searchable | 1603 | $0.88 |
| Check | Clifftop Retreat | - | 84 | $0.31 |
| Reveal | Furycalm Snarl | - | 348 | $0.29 |
| Catch-up | Turbulent Steppe | searchable | 7335 | $5.40 |
| - | Ancient Amphitheater | - | 11367 | $0.46 |
| - | Raucous Carnival | - | 8389 | $0.24 |

### Enters tapped (21)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Elegant Parlor | searchable | 777 | $11.21 |
| MDFC spell/land | Legion Leadership // Legion Stronghold | mdfc | 1209 | $0.46 |
| Bridge (artifact) | Rustvale Bridge | - | 1214 | $0.29 |
| Creature land | Restless Bivouac | manland | 4249 | $0.49 |
| Scry/Temple | Temple of Triumph | - | 288 | $0.21 |
| - | Abraded Bluffs | - | 2723 | $0.33 |
| Bounce/Karoo | Boros Garrison | - | 461 | $0.20 |
| Snow dual | Alpine Meadow | searchable, snow | 4112 | $0.36 |
| - | Sacred Peaks | searchable | 1715 | $0.24 |
| Cycling/Bicycle | Glittering Massif | searchable, cycling | 3877 | $0.33 |
| Gain/Refuge | Wind-Scarred Crag | lifegain | 993 | $0.16 |
| Guildgate | Boros Guildgate | - | 1739 | $0.11 |
| Creature land | Needle Spires | manland | 5177 | $0.28 |
| Campus | Lorehold Campus | - | 7381 | $0.27 |
| - | Sun-Blessed Peak | - | 8406 | $0.25 |
| - | Hall | - | 14551 | $0.29 |
| - | Rabanastre, Royal City | - | 5078 | $0.15 |
| - | Stone Quarry | - | 5466 | $0.12 |
| - | Fields of Strife | - | 12968 | $0.22 |
| Gain/Refuge | Dimension X | lifegain | 15238 | $0.16 |
| Pain | Scabland | pain | 21113 | RL |

---

## Simic (GU)

### Enters untapped (7)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| True dual (ABUR) | Tropical Island | searchable | 363 | RL |
| Verge | Willowrush Verge | - | 1184 | $8.85 |
| Pathway (MDFC) | Barkchannel Pathway // Tidechannel Pathway | mdfc | 1074 | $4.39 |
| Horizon/Canopy | Waterlogged Grove | - | 1102 | $1.81 |
| Pain | Yavimaya Coast | pain | 134 | $0.36 |
| Filter | Flooded Grove | filter | 309 | $0.35 |
| Filter | Overflowing Basin | filter | 715 | $0.26 |

### Conditional (enters tapped unless a condition is met) (9)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Shock | Breeding Pool | searchable | 63 | $11.77 |
| Bond (crowd) | Rejuvenating Springs | - | 144 | $8.77 |
| Slow | Dreamroot Cascade | - | 181 | $0.64 |
| Fast | Botanical Sanctum | - | 1661 | $1.41 |
| Check | Hinterland Harbor | - | 100 | $0.34 |
| Battle/Tango | Sodden Verdure | searchable | 2171 | $0.48 |
| Reveal | Vineglimmer Snarl | - | 537 | $0.25 |
| Catch-up | Turbulent Wilderness | searchable | 7116 | $6.06 |
| - | Lakeside Shack | - | 9997 | $0.14 |

### Enters tapped (22)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| Surveil land | Hedge Maze | searchable | 543 | $13.09 |
| Bounce/Karoo | Simic Growth Chamber | - | 281 | $0.32 |
| Snow dual | Rimewood Falls | searchable, snow | 2488 | $0.53 |
| Scry/Temple | Temple of Mystery | - | 300 | $0.25 |
| - | Tangled Islet | searchable | 1281 | $0.24 |
| Bridge (artifact) | Tanglepool Bridge | - | 3128 | $0.30 |
| Creature land | Restless Vinestalk | manland | 5179 | $0.38 |
| Gain/Refuge | Thornwood Falls | lifegain | 1023 | $0.15 |
| MDFC spell/land | Balamb Garden, SeeD Academy // Balamb Garden, Airborne | manland, mdfc | 6726 | $0.37 |
| Guildgate | Simic Guildgate | - | 1414 | $0.12 |
| Cycling/Bicycle | Rain-Slicked Copse | searchable, cycling | 4350 | $0.28 |
| - | Kitchen | - | 12455 | $0.40 |
| MDFC spell/land | Drowner of Truth // Drowned Jungle | mdfc | 5710 | $0.28 |
| Campus | Quandrix Campus | - | 4679 | $0.22 |
| - | Guadosalam, Farplane Gateway | - | 5491 | $0.24 |
| Creature land | Lumbering Falls | manland | 4390 | $0.18 |
| - | Lush Oasis | - | 4446 | $0.15 |
| - | Woodland Stream | - | 5066 | $0.11 |
| - | Meditation Pools | - | 8325 | $0.23 |
| - | Paradox Gardens | - | 12805 | $0.17 |
| Gain/Refuge | Mutant Town | lifegain | 16123 | $0.10 |
| Pain | Skyshroud Forest | pain | 21304 | RL |

---

## Any-color lands (132) - generic across every identity

These tap for any color and appear in every guild's results; they are generic fixing, not guild-specific. Grouped here by enter status.

### Enters untapped (94)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| - | Cavern of Souls | any-color | 112 | $50.57 |
| - | Nykthos, Shrine to Nyx | any-color | 170 | $51.30 |
| - | Gemstone Caverns | any-color | 179 | $52.79 |
| - | Mana Confluence | any-color | 120 | $33.54 |
| - | City of Brass | any-color, pain | 98 | $9.86 |
| - | Three Tree City | any-color | 183 | $23.27 |
| - | Reflecting Pool | any-color | 173 | $16.12 |
| - | Talon Gates of Madara | any-color | 585 | $34.18 |
| - | Plaza of Heroes | any-color | 529 | $9.03 |
| - | Forbidden Orchard | any-color | 689 | $9.13 |
| - | Primal Amulet // Primal Wellspring | any-color, mdfc | 2040 | $15.17 |
| - | Horizon of Progress | any-color | 1458 | $6.69 |
| - | Lazotep Quarry | any-color | 1914 | $7.53 |
| - | Unclaimed Territory | any-color | 243 | $0.65 |
| - | Tarnished Citadel | any-color, pain | 2597 | $18.30 |
| - | Dowsing Dagger // Lost Vale | any-color, mdfc | 2321 | $7.38 |
| - | Matzalantli, the Great Door // The Core | any-color, mdfc | 1716 | $3.03 |
| - | Planar Nexus | any-color | 2589 | $10.30 |
| - | Cascading Cataracts | any-color | 1173 | $1.94 |
| - | Command Tower | any-color | 2 | $0.35 |
| - | Baldur's Gate | any-color | 2396 | $3.82 |
| - | Maelstrom of the Spirit Dragon | any-color | 2222 | $2.71 |
| - | Abstergo Entertainment | any-color | 2094 | $2.22 |
| - | The Mycosynth Gardens | any-color | 875 | $0.40 |
| - | Secluded Courtyard | any-color | 223 | $0.35 |
| - | Gond Gate | any-color | 2465 | $1.34 |
| - | Sliver Hive | any-color | 5053 | $12.22 |
| - | Abundant Countryside | any-color | 3830 | $3.68 |
| - | Exotic Orchard | any-color | 9 | $0.28 |
| - | Gemstone Mine | any-color | 3341 | $2.56 |
| - | Haven of the Spirit Dragon | any-color | 1138 | $0.37 |
| - | Opal Palace | any-color | 634 | $0.33 |
| - | Lotus Vale | any-color | 6915 | $40.49 |
| - | Mirrex | any-color | 2696 | $0.91 |
| - | Glimmervoid | any-color | 4683 | $4.33 |
| - | Treasure Map // Treasure Cove | any-color, mdfc | 2897 | $0.52 |
| - | Spire of Industry | any-color | 392 | $0.28 |
| - | Great Hall of the Citadel | any-color | 1818 | $0.34 |
| - | Survivors' Encampment | any-color | 2568 | $0.37 |
| - | Crucible of the Spirit Dragon | any-color | 3893 | $0.53 |
| - | Mech Hangar | any-color, manland | 3264 | $0.40 |
| - | Heap Gate | any-color | 2955 | $0.38 |
| - | Jasmine Dragon Tea Shop | any-color | 4864 | $0.77 |
| - | Meteor Crater | any-color | 7496 | $3.49 |
| - | Conduit Pylons | any-color | 1961 | $0.29 |
| - | Eclipsed Realms | any-color | 4044 | $0.40 |
| - | Pillar of the Paruns | any-color | 6325 | $1.28 |
| - | Undiscovered Paradise | any-color | 16588 | $37.61 |
| - | Ancient Ziggurat | any-color | 2726 | $0.34 |
| - | Tendo Ice Bridge | any-color | 7085 | $1.76 |
| - | The Grey Havens | any-color | 1529 | $0.26 |
| - | Golden Guardian // Gold-Forge Garrison | any-color, mdfc | 7326 | $1.48 |
| - | Voldaren Estate | any-color | 2390 | $0.28 |
| - | Azor's Gateway // Sanctum of the Sun | any-color, mdfc | 8414 | $2.09 |
| - | Crystal Grotto | any-color | 2590 | $0.29 |
| - | Forsaken City | any-color | 22216 | $10.31 |
| - | Aether Hub | any-color | 3216 | $0.30 |
| - | Hidden Grotto | any-color | 2318 | $0.26 |
| - | Rumble Arena | any-color | 3668 | $0.30 |
| - | Hall of Tagsin | any-color | 6079 | $0.39 |
| - | Ally Encampment | any-color | 7822 | $0.70 |
| - | Plaza of Harmony | any-color | 7291 | $0.51 |
| - | Thran Quarry | any-color | 14168 | $4.73 |
| - | Holdout Settlement | any-color | 2991 | $0.28 |
| - | The Seedcore | any-color | 5650 | $0.35 |
| - | Springjack Pasture | any-color | 11880 | $0.86 |
| - | Gallifrey Council Chamber | any-color | 5472 | $0.29 |
| - | Hall of Oracles | any-color | 5916 | $0.29 |
| - | Daily Bugle Building | any-color | 4010 | $0.25 |
| - | Great Hall of the Biblioplex | any-color, manland | 12475 | $0.48 |
| - | Captivating Cave | any-color | 5864 | $0.27 |
| - | White Lotus Hideout | any-color | 5973 | $0.27 |
| - | Capital City | any-color, cycling | 4087 | $0.24 |
| - | Guildmages' Forum | any-color | 9255 | $0.34 |
| - | Archaeological Dig | any-color | 17328 | $0.40 |
| - | Brotherhood Headquarters | any-color | 4907 | $0.24 |
| - | Study Hall | any-color | 4327 | $0.22 |
| - | Turtle Lair | any-color | 6925 | $0.26 |
| - | Interplanar Beacon | any-color, lifegain | 4320 | $0.19 |
| - | Paliano, the High City | any-color | 24296 | $0.36 |
| - | Rhystic Cave | any-color | 19710 | $0.34 |
| - | Henge of Ramos | any-color | 26266 | $0.35 |
| - | Corrupted Crossroads | any-color | 5369 | $0.12 |
| - | Painted Bluffs | any-color | 6691 | $0.18 |
| - | Cave of Temptation | any-color | 9068 | $0.24 |
| - | Branch of Vitu-Ghazi | any-color | 7251 | $0.18 |
| - | Bucolic Ranch | any-color | 13737 | $0.25 |
| - | Mirrodin's Core | any-color | 10916 | $0.22 |
| - | Unknown Shores | any-color | 7534 | $0.08 |
| - | Shimmering Grotto | any-color | 11429 | $0.19 |
| - | Rainbow Vale | any-color | 13132 | RL |
| - | Throne of Makindi | any-color | 18091 | $0.19 |
| - | Forgotten Monument | any-color | 13355 | $0.16 |
| - | School of the Unseen | any-color | 26542 | $0.22 |

### Conditional (enters tapped unless a condition is met) (3)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| - | Starting Town | any-color | 894 | $10.86 |
| - | Temple of the Dragon Queen | any-color | 2490 | $0.29 |
| - | Primal Beyond | any-color | 6578 | $0.22 |

### Enters tapped (35)
| Cycle | Card | Tags | EDHREC | Price |
|---|---|---|---|---|
| - | Lotus Field | any-color | 926 | $2.87 |
| - | Path of Ancestry | any-color | 14 | $0.36 |
| - | Valgavoth's Lair | any-color | 1700 | $0.95 |
| - | Sea Gate | any-color | 2373 | $1.60 |
| - | Cactus Preserve | any-color, manland | 3597 | $5.24 |
| - | Power Depot | any-color | 2000 | $0.42 |
| - | Citadel Gate | any-color | 2830 | $1.38 |
| - | Hidden Hideout | any-color | 5051 | $3.19 |
| - | Thriving Isle | any-color | 1028 | $0.31 |
| - | Scene of the Crime | any-color | 2582 | $0.32 |
| - | Vivid Meadow | any-color | 5729 | $0.40 |
| - | Sunken Citadel | any-color | 6029 | $0.49 |
| - | Vivid Creek | any-color | 4301 | $0.35 |
| - | Thriving Heath | any-color | 1080 | $0.23 |
| - | Pit of Offerings | any-color | 3347 | $0.32 |
| - | Tarnation Vista | any-color | 8737 | $0.64 |
| - | Grand Coliseum | any-color, pain | 4760 | $0.29 |
| - | Big Apple, 3 a.m. | any-color | 8709 | $0.39 |
| - | Mirage Mesa | any-color | 3909 | $0.25 |
| - | Transguild Promenade | any-color | 7911 | $0.35 |
| - | Command Bridge | any-color | 3934 | $0.25 |
| - | Gateway Plaza | any-color | 2504 | $0.16 |
| - | Crossroads Village | any-color | 3233 | $0.21 |
| - | Uncharted Haven | any-color | 2729 | $0.14 |
| - | Shimmerdrift Vale | any-color, snow | 6828 | $0.24 |
| - | Edgewall Inn | any-color | 9262 | $0.25 |
| - | Rupture Spire | any-color | 5968 | $0.14 |
| - | Crumbling Vestige | any-color | 8720 | $0.23 |
| - | Public Thoroughfare | any-color | 8558 | $0.20 |
| - | Night Market | any-color, cycling | 6913 | $0.09 |
| - | Abandoned Outpost | any-color | 21778 | $0.25 |
| - | Cryptic Spires | any-color | 10353 | $0.17 |
| - | Seafloor Debris | any-color | 23461 | $0.24 |
| - | Archway Commons | any-color | 9026 | $0.12 |
| - | Base Camp | any-color | 10991 | $0.10 |
