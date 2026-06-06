# Two-color fixing lands

Generated from [`all-pairs.json`](all-pairs.json) (`mtg-lands --all-pairs --json`), which is the data
source of record. Each identity is split into three tables by how the land
enters play - read straight from the oracle text:

- **Enters untapped** - always untapped (true duals, painlands, filters, verges,
  horizon lands, Tainted, storage/depletion/locked lands).
- **Conditional** - untapped only if a condition is met, else tapped (shock,
  check, fast, slow, battle, bond, reveal, catch-up).
- **Enters tapped** - always tapped (Temples, surveil lands, bounce, gain,
  cycling, snow, creature lands, Campus, Bridge, Guildgate, plain taplands).

Columns: **Cycle** (the recognized land cycle, or `-` if it is a one-off / not a
named cycle), **Card**, and **Tags** (orthogonal properties):
`searchable` = has basic land types (fetchable), `filter`, `pain`,
`lifegain`, `manland`, `MDFC`, `cycling`, `snow`, `scry`, `surveil`, `bounce`,
`storage`. Rows are ordered by a popularity+price score, best first.

The ~135 **any-color** lands (City of Brass, Command Tower, Cavern of Souls, ...)
tap for any color and recur in every identity, so they are listed once at the
[end](#any-color-generic-fixing) rather than under each guild.


---

## Azorius (WU)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Tundra | searchable |
| Verge | Floodfarm Verge |  |
| Filter | Mystic Gate | filter |
| Pathway | Hengegate Pathway // Mistgate Pathway | MDFC |
| - | Nimbus Maze |  |
| Pain | Adarkar Wastes | pain |
| Filter | Skycloud Expanse | filter |
| Depletion | Land Cap |  |
| Storage | Calciform Pools | storage |
| Locked | Cloudcrest Lake |  |
| Locked | Thalakos Lowlands |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Sea of Clouds |  |
| Shock | Hallowed Fountain | searchable |
| Slow | Deserted Beach |  |
| Check | Glacial Fortress |  |
| Battle/Tango | Prairie Stream | searchable |
| Fast | Seachrome Coast |  |
| Reveal | Port Town |  |
| - | Wanderwine Hub |  |
| - | Abandoned Campground |  |
| - | Fortified Beachhead |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Meticulous Archive | searchable, surveil |
| Scry/Temple | Temple of Enlightenment | scry |
| Bridge | Razortide Bridge |  |
| Creature land | Restless Anchorage | manland |
| Bounce/Karoo | Azorius Chancery | bounce |
| Snow dual | Glacial Floodplain | searchable, snow |
| Creature land | Celestial Colonnade | manland |
| Gain/Refuge | Sejiri Refuge | lifegain |
| Cycling/Bicycle | Irrigated Farmland | searchable, cycling |
| - | Idyllic Beachfront | searchable |
| Gain/Refuge | Tranquil Cove | lifegain |
| Snow dual | Boreal Shelf | snow |
| Guildgate | Azorius Guildgate |  |
| - | Study |  |
| MDFC spell/land | Suppression Ray // Orderly Plaza | MDFC |
| - | Lonely Arroyo |  |
| - | Sharlayan, Nation of Scholars |  |
| - | North Pole Gates |  |
| - | Meandering River |  |
| - | Skybridge Towers |  |
| Campus | University Campus | surveil |
| - | Coastal Tower |  |


---

## Dimir (UB)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Underground Sea | searchable |
| Verge | Gloomlake Verge |  |
| Filter | Sunken Ruins | filter |
| Pain | Underground River | pain |
| Pathway | Clearwater Pathway // Murkwater Pathway | MDFC |
| Tainted | Tainted Isle |  |
| Filter | Darkwater Catacombs | filter |
| - | River of Tears |  |
| Depletion | River Delta |  |
| Storage | Dreadship Reef | storage |
| Locked | Waterveil Cavern |  |
| Locked | Rootwater Depths |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Morphic Pool |  |
| Shock | Watery Grave | searchable |
| Slow | Shipwreck Marsh |  |
| Check | Drowned Catacomb |  |
| Battle/Tango | Sunken Hollow | searchable |
| Fast | Darkslick Shores |  |
| Reveal | Choked Estuary |  |
| - | Secluded Glen |  |
| - | Murky Sewer |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Undercity Sewers | searchable, surveil |
| Bounce/Karoo | Dimir Aqueduct | bounce |
| Bridge | Mistvault Bridge |  |
| MDFC spell/land | Waterlogged Teachings // Inundated Archive | MDFC |
| Creature land | Restless Reef | manland |
| Cycling/Bicycle | Fetid Pools | searchable, cycling |
| - | Contaminated Aquifer | searchable |
| Scry/Temple | Temple of Deceit | scry |
| Snow dual | Ice Tunnel | searchable, snow |
| Creature land | Creeping Tar Pit | manland |
| Gain/Refuge | Jwar Isle Refuge | lifegain |
| Gain/Refuge | Dismal Backwater | lifegain |
| Snow dual | Frost Marsh | snow |
| Guildgate | Dimir Guildgate |  |
| - | Waterfront District |  |
| - | Secret Passage |  |
| - | Soured Springs |  |
| - | Submerged Boneyard |  |
| - | Treno, Dark City |  |
| - | Serpent's Pass |  |
| - | Salt Marsh |  |
| - | Sinister Hideout | surveil |


---

## Rakdos (BR)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Badlands | searchable |
| Verge | Blazemire Verge |  |
| Pain | Sulfurous Springs | pain |
| Pathway | Blightstep Pathway // Searstep Pathway | MDFC |
| Filter | Graven Cairns | filter |
| - | Mount Doom |  |
| Tainted | Tainted Peak |  |
| Filter | Shadowblood Ridge | filter |
| Depletion | Lava Tubes |  |
| Storage | Molten Slagheap | storage |
| Locked | Lantern-Lit Graveyard |  |
| Locked | Cinder Marsh |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Luxury Suite |  |
| Shock | Blood Crypt | searchable |
| Slow | Haunted Ridge |  |
| Check | Dragonskull Summit |  |
| Fast | Blackcleave Cliffs |  |
| Battle/Tango | Smoldering Marsh | searchable |
| Reveal | Foreboding Ruins |  |
| - | Auntie's Hovel |  |
| - | Razortrap Gorge |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Raucous Theater | searchable, surveil |
| Bridge | Drossforge Bridge |  |
| Bounce/Karoo | Rakdos Carnarium | bounce |
| Scry/Temple | Temple of Malice | scry |
| - | Jagged Barrens |  |
| Creature land | Restless Vents | manland |
| - | Geothermal Bog | searchable |
| Gain/Refuge | Akoum Refuge | lifegain |
| Cycling/Bicycle | Canyon Slough | searchable, cycling |
| Gain/Refuge | Bloodfell Caves | lifegain |
| Snow dual | Sulfurous Mire | searchable, snow |
| Creature land | Lavaclaw Reaches | manland |
| Guildgate | Rakdos Guildgate |  |
| Snow dual | Tresserhorn Sinks | snow |
| - | Vector, Imperial Capital |  |
| - | Boiling Rock Prison |  |
| - | Urborg Volcano |  |
| - | Billiard Room |  |
| - | Cinder Barrens |  |
| - | Ominous Asylum | surveil |
| - | Tramway Station |  |


---

## Gruul (RG)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Taiga | searchable |
| Verge | Thornspire Verge |  |
| Filter | Fire-Lit Thicket | filter |
| Pathway | Cragcrown Pathway // Timbercrown Pathway | MDFC |
| Pain | Karplusan Forest | pain |
| Reverse-pain | Grove of the Burnwillows |  |
| Filter | Mossfire Valley | filter |
| Depletion | Timberline Ridge |  |
| Locked | Pinecrest Ridge |  |
| Storage | Fungal Reaches | storage |
| Locked | Mogg Hollows |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Stomping Ground | searchable |
| Bond (crowd) | Spire Garden |  |
| Slow | Rockfall Vale |  |
| Battle/Tango | Cinder Glade | searchable |
| Check | Rootbound Crag |  |
| Fast | Copperline Gorge |  |
| Reveal | Game Trail |  |
| - | Bleeding Woods |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Commercial District | searchable, surveil |
| MDFC spell/land | Stump Stomp // Burnwillow Clearing | MDFC |
| Bounce/Karoo | Gruul Turf | bounce |
| Scry/Temple | Temple of Abandon | scry |
| Snow dual | Highland Forest | searchable, snow |
| Cycling/Bicycle | Sheltered Thicket | searchable, cycling |
| Creature land | Restless Ridgeline | manland |
| - | Wooded Ridgeline | searchable |
| Bridge | Slagwoods Bridge |  |
| Gain/Refuge | Rugged Highlands | lifegain |
| - | Bristling Backwoods |  |
| Guildgate | Gruul Guildgate |  |
| Creature land | Raging Ravine | manland |
| Gain/Refuge | Kazandu Refuge | lifegain |
| - | Gongaga, Reactor Town |  |
| - | Dining Room |  |
| Snow dual | Highland Weald | snow |
| - | Timber Gorge |  |
| - | Omashu City |  |
| - | Racers' Ring |  |
| - | Savage Mansion | surveil |
| - | Shivan Oasis |  |


---

## Selesnya (GW)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Savannah | searchable |
| Verge | Hushwood Verge |  |
| Pain | Brushland | pain |
| Filter | Wooded Bastion | filter |
| Pathway | Branchloft Pathway // Boulderloft Pathway | MDFC |
| Horizon/Canopy | Horizon Canopy |  |
| Filter | Sungrass Prairie | filter |
| - | Riftstone Portal |  |
| Depletion | Veldt |  |
| Storage | Saltcrusted Steppe | storage |
| Locked | Tranquil Garden |  |
| Locked | Vec Townships |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Bountiful Promenade |  |
| Shock | Temple Garden | searchable |
| Slow | Overgrown Farmland |  |
| Check | Sunpetal Grove |  |
| Fast | Razorverge Thicket |  |
| Battle/Tango | Canopy Vista | searchable |
| Reveal | Fortified Village |  |
| - | Etched Cornfield |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Lush Portico | searchable, surveil |
| Scry/Temple | Temple of Plenty | scry |
| MDFC spell/land | Strength of the Harvest // Haven of the Harvest | MDFC |
| Bounce/Karoo | Selesnya Sanctuary | bounce |
| Cycling/Bicycle | Scattered Groves | searchable, cycling |
| Snow dual | Arctic Treeline | searchable, snow |
| Creature land | Restless Prairie | manland |
| - | Radiant Grove | searchable |
| Gain/Refuge | Blossoming Sands | lifegain |
| Bridge | Thornglint Bridge |  |
| Snow dual | Arctic Flats | snow |
| Gain/Refuge | Graypelt Refuge | lifegain |
| Creature land | Stirring Wildwood | manland |
| Guildgate | Selesnya Guildgate |  |
| - | Creosote Heath |  |
| - | Conservatory |  |
| - | Windurst, Federation Center |  |
| - | Kyoshi Village |  |
| - | Botanical Plaza |  |
| - | Tranquil Expanse |  |
| - | Elfhame Palace |  |
| - | Suburban Sanctuary | surveil |


---

## Orzhov (WB)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Scrubland | searchable |
| Verge | Bleachbone Verge |  |
| Pathway | Brightclimb Pathway // Grimclimb Pathway | MDFC |
| Horizon/Canopy | Silent Clearing |  |
| Pain | Caves of Koilos | pain |
| Filter | Fetid Heath | filter |
| Tainted | Tainted Field |  |
| Filter | Desolate Mire | filter |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Vault of Champions |  |
| Shock | Godless Shrine | searchable |
| Slow | Shattered Sanctum |  |
| Fast | Concealed Courtyard |  |
| Check | Isolated Chapel |  |
| Reveal | Shineshadow Snarl |  |
| Catch-up | Turbulent Moor | searchable |
| Battle/Tango | Eclipsed Steppe | searchable |
| - | Neglected Manor |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Shadowy Backstreet | searchable, surveil |
| Bridge | Goldmire Bridge |  |
| Bounce/Karoo | Orzhov Basilica | bounce |
| Creature land | Restless Fortress | manland |
| MDFC spell/land | Glasswing Grace // Age-Graced Chapel | MDFC |
| Snow dual | Snowfield Sinkhole | searchable, snow |
| Scry/Temple | Temple of Silence | scry |
| Creature land | Shambling Vent | manland |
| Gain/Refuge | Scoured Barrens | lifegain |
| - | Sunlit Marsh | searchable |
| Cycling/Bicycle | Umbral Expanse | searchable, cycling |
| Guildgate | Orzhov Guildgate |  |
| - | Forlorn Flats |  |
| - | Forsaken Sanctuary |  |
| - | Ballroom |  |
| Campus | Silverquill Campus | scry |
| - | Insomnia, Crown City |  |
| - | Misty Palms Oasis |  |
| - | Forum of Amity | surveil |
| Gain/Refuge | Foot Headquarters | lifegain |
| Pain | Salt Flats | pain |


---

## Izzet (UR)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Volcanic Island | searchable |
| Verge | Riverpyre Verge |  |
| Horizon/Canopy | Fiery Islet |  |
| Pathway | Riverglide Pathway // Lavaglide Pathway | MDFC |
| Filter | Cascade Bluffs | filter |
| Pain | Shivan Reef | pain |
| Filter | Ferrous Lake | filter |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Steam Vents | searchable |
| Bond (crowd) | Training Center |  |
| Slow | Stormcarved Coast |  |
| Fast | Spirebluff Canal |  |
| Check | Sulfur Falls |  |
| Reveal | Frostboil Snarl |  |
| Catch-up | Turbulent Springs | searchable |
| Battle/Tango | Scorched Geyser | searchable |
| MDFC spell/land | Rush of Inspiration // Crackling Falls | MDFC |
| - | Peculiar Lighthouse |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Thundering Falls | searchable, surveil |
| Bounce/Karoo | Izzet Boilerworks | bounce |
| Bridge | Silverbluff Bridge |  |
| Snow dual | Volatile Fjord | searchable, snow |
| Scry/Temple | Temple of Epiphany | scry |
| - | Molten Tributary | searchable |
| Gain/Refuge | Swiftwater Cliffs | lifegain |
| - | Eroded Canyon |  |
| Guildgate | Izzet Guildgate |  |
| Cycling/Bicycle | Coastal Peak | searchable, cycling |
| - | Library |  |
| Creature land | Restless Spire | manland, scry |
| Campus | Prismari Campus | scry |
| Creature land | Wandering Fumarole | manland |
| - | Baron, Airship Kingdom |  |
| - | Airship Engine Room |  |
| - | Highland Lake |  |
| - | Spectacle Summit | surveil |
| Gain/Refuge | TCRI Building | lifegain |
| Pain | Caldera Lake | pain |


---

## Golgari (BG)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Bayou | searchable |
| Verge | Wastewood Verge |  |
| Pathway | Darkbore Pathway // Slitherbore Pathway | MDFC |
| Horizon/Canopy | Nurturing Peatland |  |
| Pain | Llanowar Wastes | pain |
| Filter | Twilight Mire | filter |
| Filter | Viridescent Bog | filter |
| Tainted | Tainted Wood |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Overgrown Tomb | searchable |
| Bond (crowd) | Undergrowth Stadium |  |
| Slow | Deathcap Glade |  |
| Check | Woodland Cemetery |  |
| Fast | Blooming Marsh |  |
| Battle/Tango | Vernal Fen | searchable |
| Reveal | Necroblossom Snarl |  |
| - | Gilt-Leaf Palace |  |
| Catch-up | Turbulent Fen | searchable |
| - | Strangled Cemetery |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Underground Mortuary | searchable, surveil |
| MDFC spell/land | Revitalizing Repast // Old-Growth Grove | MDFC |
| Bounce/Karoo | Golgari Rot Farm | bounce |
| Creature land | Restless Cottage | manland |
| Snow dual | Woodland Chasm | searchable, snow |
| - | Haunted Mire | searchable |
| Scry/Temple | Temple of Malady | scry |
| Cycling/Bicycle | Festering Thicket | searchable, cycling |
| Bridge | Darkmoss Bridge |  |
| Creature land | Hissing Quagmire | manland |
| Gain/Refuge | Jungle Hollow | lifegain |
| Guildgate | Golgari Guildgate |  |
| - | Festering Gulch |  |
| Campus | Witherbloom Campus | scry |
| - | Foul Orchard |  |
| - | Gohn, Town of Ruin |  |
| - | Foggy Bottom Swamp |  |
| - | Lounge |  |
| - | Titan's Grave | surveil |
| Gain/Refuge | Illegitimate Business | lifegain |
| Pain | Pine Barrens | pain |


---

## Boros (RW)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Plateau | searchable |
| Verge | Sunbillow Verge |  |
| Pathway | Needleverge Pathway // Pillarverge Pathway | MDFC |
| Horizon/Canopy | Sunbaked Canyon |  |
| Filter | Sunscorched Divide | filter |
| Filter | Rugged Prairie | filter |
| Pain | Battlefield Forge | pain |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Sacred Foundry | searchable |
| Bond (crowd) | Spectator Seating |  |
| Slow | Sundown Pass |  |
| Fast | Inspiring Vantage |  |
| Battle/Tango | Radiant Summit | searchable |
| Check | Clifftop Retreat |  |
| Reveal | Furycalm Snarl |  |
| Catch-up | Turbulent Steppe | searchable |
| - | Ancient Amphitheater |  |
| - | Raucous Carnival |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Elegant Parlor | searchable, surveil |
| MDFC spell/land | Legion Leadership // Legion Stronghold | MDFC |
| Bridge | Rustvale Bridge |  |
| Creature land | Restless Bivouac | manland |
| Scry/Temple | Temple of Triumph | scry |
| - | Sacred Peaks | searchable |
| Bounce/Karoo | Boros Garrison | bounce |
| - | Abraded Bluffs |  |
| Snow dual | Alpine Meadow | searchable, snow |
| Cycling/Bicycle | Glittering Massif | searchable, cycling |
| Gain/Refuge | Wind-Scarred Crag | lifegain |
| Guildgate | Boros Guildgate |  |
| Creature land | Needle Spires | manland |
| Campus | Lorehold Campus | scry |
| - | Rabanastre, Royal City |  |
| - | Sun-Blessed Peak |  |
| - | Hall |  |
| - | Stone Quarry |  |
| - | Fields of Strife | surveil |
| Gain/Refuge | Dimension X | lifegain |
| Pain | Scabland | pain |


---

## Simic (GU)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Tropical Island | searchable |
| Verge | Willowrush Verge |  |
| Pathway | Barkchannel Pathway // Tidechannel Pathway | MDFC |
| Horizon/Canopy | Waterlogged Grove |  |
| Pain | Yavimaya Coast | pain |
| Filter | Flooded Grove | filter |
| Filter | Overflowing Basin | filter |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Breeding Pool | searchable |
| Bond (crowd) | Rejuvenating Springs |  |
| Slow | Dreamroot Cascade |  |
| Fast | Botanical Sanctum |  |
| Check | Hinterland Harbor |  |
| Battle/Tango | Sodden Verdure | searchable |
| Reveal | Vineglimmer Snarl |  |
| Catch-up | Turbulent Wilderness | searchable |
| - | Lakeside Shack |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Hedge Maze | searchable, surveil |
| Bounce/Karoo | Simic Growth Chamber | bounce |
| Snow dual | Rimewood Falls | searchable, snow |
| Scry/Temple | Temple of Mystery | scry |
| Creature land | Restless Vinestalk | manland |
| - | Tangled Islet | searchable |
| Bridge | Tanglepool Bridge |  |
| Gain/Refuge | Thornwood Falls | lifegain |
| Cycling/Bicycle | Rain-Slicked Copse | searchable, cycling |
| MDFC spell/land | Balamb Garden, SeeD Academy // Balamb Garden, Airborne | manland, MDFC |
| Guildgate | Simic Guildgate |  |
| - | Kitchen |  |
| - | Guadosalam, Farplane Gateway |  |
| Campus | Quandrix Campus | scry |
| MDFC spell/land | Drowner of Truth // Drowned Jungle | MDFC |
| Creature land | Lumbering Falls | manland |
| - | Lush Oasis |  |
| - | Woodland Stream |  |
| - | Meditation Pools |  |
| - | Paradox Gardens | surveil |
| Gain/Refuge | Mutant Town | lifegain |
| Pain | Skyshroud Forest | pain |


---

## Any-color (generic fixing)

Tap for any color; run in any identity. 150 cards.

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| - | Cavern of Souls |  |
| - | Nykthos, Shrine to Nyx |  |
| - | Gemstone Caverns |  |
| - | Mana Confluence |  |
| - | City of Brass | pain |
| - | Three Tree City |  |
| - | Reflecting Pool |  |
| - | Talon Gates of Madara |  |
| - | Plaza of Heroes |  |
| - | Forbidden Orchard |  |
| MDFC spell/land | Primal Amulet // Primal Wellspring | MDFC |
| Horizon/Canopy | Horizon of Progress |  |
| - | Lazotep Quarry |  |
| - | Tarnished Citadel |  |
| MDFC spell/land | Dowsing Dagger // Lost Vale | MDFC |
| MDFC spell/land | Matzalantli, the Great Door // The Core | MDFC |
| - | Planar Nexus |  |
| - | Cascading Cataracts |  |
| - | Secluded Courtyard |  |
| - | Command Tower |  |
| - | Baldur's Gate |  |
| - | Maelstrom of the Spirit Dragon |  |
| - | Abstergo Entertainment |  |
| - | Unclaimed Territory |  |
| MDFC spell/land | Storm the Vault // Vault of Catlacan | MDFC |
| - | Gond Gate |  |
| - | Sliver Hive |  |
| - | Exotic Orchard |  |
| MDFC spell/land | Journey to Eternity // Atzal, Cave of Eternity | MDFC |
| - | Gemstone Mine |  |
| - | Abundant Countryside |  |
| - | The Mycosynth Gardens |  |
| - | Opal Palace |  |
| - | Haven of the Spirit Dragon |  |
| - | Lotus Vale |  |
| - | Mirrex |  |
| - | Glimmervoid |  |
| - | Great Hall of the Citadel |  |
| - | Spire of Industry |  |
| MDFC spell/land | Treasure Map // Treasure Cove | MDFC, scry |
| - | Survivors' Encampment |  |
| - | Heap Gate |  |
| Storage | Crucible of the Spirit Dragon | storage |
| - | Ancient Ziggurat |  |
| MDFC spell/land | Hadana's Climb // Winged Temple of Orazca | MDFC |
| Creature land | Mech Hangar | manland |
| - | Jasmine Dragon Tea Shop |  |
| - | The Grey Havens | scry |
| - | Conduit Pylons | surveil |
| - | Meteor Crater |  |
| - | Pillar of the Paruns |  |
| - | Undiscovered Paradise |  |
| Bridge | Tendo Ice Bridge |  |
| Horizon/Canopy | Voldaren Estate |  |
| MDFC spell/land | Golden Guardian // Gold-Forge Garrison | MDFC |
| MDFC spell/land | Azor's Gateway // Sanctum of the Sun | MDFC |
| - | Eclipsed Realms |  |
| Locked | Forsaken City |  |
| Scry/Temple | Crystal Grotto | scry |
| - | Aether Hub |  |
| - | Plaza of Harmony |  |
| - | Hall of Tagsin |  |
| - | Hidden Grotto | surveil |
| - | Ally Encampment |  |
| - | Thran Quarry |  |
| - | The Seedcore |  |
| - | Holdout Settlement |  |
| - | Daily Bugle Building |  |
| Scry/Temple | Rumble Arena | scry |
| - | Springjack Pasture |  |
| - | Gallifrey Council Chamber | surveil |
| Creature land | Great Hall of the Biblioplex | manland |
| - | Turtle Lair |  |
| MDFC spell/land | Profane Procession // Tomb of the Dusk Rose | MDFC |
| - | Capital City | cycling |
| - | Archaeological Dig |  |
| - | Brotherhood Headquarters |  |
| - | White Lotus Hideout |  |
| - | Hall of Oracles |  |
| - | Study Hall | scry |
| MDFC spell/land | Path of Mettle // Metzali, Tower of Triumph | MDFC |
| - | Captivating Cave |  |
| - | Guildmages' Forum |  |
| - | Interplanar Beacon | lifegain |
| - | Paliano, the High City |  |
| - | Rhystic Cave |  |
| - | Henge of Ramos |  |
| - | Corrupted Crossroads |  |
| - | Painted Bluffs |  |
| - | Cave of Temptation |  |
| - | Branch of Vitu-Ghazi |  |
| - | Bucolic Ranch |  |
| - | Mirrodin's Core |  |
| - | Unknown Shores |  |
| - | Shimmering Grotto |  |
| - | Rainbow Vale |  |
| - | Throne of Makindi |  |
| - | Forgotten Monument |  |
| - | School of the Unseen |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| - | Starting Town |  |
| Scry/Temple | Temple of the Dragon Queen |  |
| Bridge | Command Bridge |  |
| Guildgate | Gateway Plaza |  |
| - | Transguild Promenade |  |
| - | Primal Beyond |  |
| - | Rupture Spire |  |
| - | Public Thoroughfare |  |
| - | Archway Commons |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| - | Lotus Field |  |
| - | Valgavoth's Lair |  |
| - | Path of Ancestry | scry |
| - | Sea Gate |  |
| Creature land | Cactus Preserve | manland |
| - | Manor Gate |  |
| - | Power Depot |  |
| - | Citadel Gate |  |
| - | Hidden Hideout |  |
| - | Black Dragon Gate |  |
| - | Thriving Isle |  |
| - | Cliffgate |  |
| - | Scene of the Crime |  |
| - | Vivid Grove |  |
| - | Thriving Moor |  |
| - | Vivid Meadow |  |
| - | Sunken Citadel |  |
| MDFC spell/land | Bloodsoaked Insight // Sanguine Morass | MDFC |
| - | Thriving Heath |  |
| - | Vivid Creek |  |
| - | Pit of Offerings |  |
| - | Vivid Crag |  |
| Pain | Grand Coliseum | pain |
| - | Vivid Marsh |  |
| - | Thriving Bluff |  |
| - | Tarnation Vista |  |
| - | Thriving Grove |  |
| - | Big Apple, 3 a.m. |  |
| - | Mirage Mesa |  |
| - | Crossroads Village |  |
| - | Uncharted Haven |  |
| Snow dual | Shimmerdrift Vale | snow |
| - | Edgewall Inn |  |
| - | Crumbling Vestige |  |
| - | Night Market | cycling |
| - | Abandoned Outpost |  |
| - | Seafloor Debris |  |
| - | Cryptic Spires |  |
| - | Timberland Ruins |  |
| - | Base Camp |  |
| - | Ravaged Highlands |  |
| - | Bog Wreckage |  |
