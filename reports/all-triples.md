# Three-color fixing lands

Generated from [`all-triples.json`](all-triples.json) (`mtg-lands --all-triples --json`), which is the data
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

## Bant (GWU)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Tropical Island | searchable |
| True dual | Tundra | searchable |
| Verge | Floodfarm Verge |  |
| Verge | Hushwood Verge |  |
| True dual | Savannah | searchable |
| Pain | Brushland | pain |
| Verge | Willowrush Verge |  |
| Filter | Mystic Gate | filter |
| Filter | Wooded Bastion | filter |
| Pathway | Barkchannel Pathway // Tidechannel Pathway | MDFC |
| Pathway | Hengegate Pathway // Mistgate Pathway | MDFC |
| Pathway | Branchloft Pathway // Boulderloft Pathway | MDFC |
| - | Nimbus Maze |  |
| Horizon/Canopy | Horizon Canopy |  |
| Pain | Yavimaya Coast | pain |
| Horizon/Canopy | Waterlogged Grove |  |
| Pain | Adarkar Wastes | pain |
| Filter | Flooded Grove | filter |
| Filter | Sungrass Prairie | filter |
| Filter | Skycloud Expanse | filter |
| Filter | Overflowing Basin | filter |
| - | Riftstone Portal |  |
| Depletion | Veldt |  |
| Depletion | Land Cap |  |
| Storage | Saltcrusted Steppe | storage |
| Triland | Treva's Ruins |  |
| Storage | Calciform Pools | storage |
| Locked | Cloudcrest Lake |  |
| Triland | Aysen Abbey |  |
| Locked | Tranquil Garden |  |
| Locked | Thalakos Lowlands |  |
| Locked | Vec Townships |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Breeding Pool | searchable |
| Bond (crowd) | Sea of Clouds |  |
| Shock | Hallowed Fountain | searchable |
| Bond (crowd) | Bountiful Promenade |  |
| Shock | Temple Garden | searchable |
| Bond (crowd) | Rejuvenating Springs |  |
| Slow | Deserted Beach |  |
| Slow | Overgrown Farmland |  |
| Check | Sunpetal Grove |  |
| Slow | Dreamroot Cascade |  |
| Check | Glacial Fortress |  |
| Check | Hinterland Harbor |  |
| Fast | Botanical Sanctum |  |
| Battle/Tango | Prairie Stream | searchable |
| Fast | Razorverge Thicket |  |
| Battle/Tango | Canopy Vista | searchable |
| Fast | Seachrome Coast |  |
| Battle/Tango | Sodden Verdure | searchable |
| Reveal | Fortified Village |  |
| Catch-up | Turbulent Wilderness | searchable |
| Reveal | Port Town |  |
| Reveal | Vineglimmer Snarl |  |
| - | Wanderwine Hub |  |
| - | Abandoned Campground |  |
| - | Fortified Beachhead |  |
| - | Etched Cornfield |  |
| - | Lakeside Shack |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Spara's Headquarters | searchable, cycling |
| Surveil land | Hedge Maze | searchable, surveil |
| Surveil land | Meticulous Archive | searchable, surveil |
| Surveil land | Lush Portico | searchable, surveil |
| Triland | Seaside Citadel |  |
| Bounce/Karoo | Simic Growth Chamber | bounce |
| Scry/Temple | Temple of Enlightenment | scry |
| Snow dual | Rimewood Falls | searchable, snow |
| Bridge | Razortide Bridge |  |
| Scry/Temple | Temple of Plenty | scry |
| Creature land | Restless Anchorage | manland |
| Bounce/Karoo | Azorius Chancery | bounce |
| MDFC spell/land | Strength of the Harvest // Haven of the Harvest | MDFC |
| Bounce/Karoo | Selesnya Sanctuary | bounce |
| Cycling/Bicycle | Scattered Groves | searchable, cycling |
| Scry/Temple | Temple of Mystery | scry |
| Snow dual | Glacial Floodplain | searchable, snow |
| Creature land | Celestial Colonnade | manland |
| Snow dual | Arctic Treeline | searchable, snow |
| Triland | Urban Retreat |  |
| Creature land | Restless Vinestalk | manland |
| Cycling/Bicycle | Irrigated Farmland | searchable, cycling |
| Creature land | Restless Prairie | manland |
| Gain/Refuge | Sejiri Refuge | lifegain |
| Bridge | Tanglepool Bridge |  |
| - | Idyllic Beachfront | searchable |
| - | Tangled Islet | searchable |
| Snow dual | Arctic Flats | snow |
| MDFC spell/land | Balamb Garden, SeeD Academy // Balamb Garden, Airborne | manland, MDFC |
| Bridge | Thornglint Bridge |  |
| Cycling/Bicycle | Rain-Slicked Copse | searchable, cycling |
| Gain/Refuge | Blossoming Sands | lifegain |
| Snow dual | Boreal Shelf | snow |
| - | Radiant Grove | searchable |
| Gain/Refuge | Thornwood Falls | lifegain |
| Gain/Refuge | Graypelt Refuge | lifegain |
| Gain/Refuge | Tranquil Cove | lifegain |
| Creature land | Stirring Wildwood | manland |
| - | Kitchen |  |
| Guildgate | Simic Guildgate |  |
| - | Study |  |
| Guildgate | Selesnya Guildgate |  |
| Guildgate | Azorius Guildgate |  |
| MDFC spell/land | Suppression Ray // Orderly Plaza | MDFC |
| - | Creosote Heath |  |
| - | Guadosalam, Farplane Gateway |  |
| - | Lonely Arroyo |  |
| Campus | Quandrix Campus | scry |
| MDFC spell/land | Drowner of Truth // Drowned Jungle | MDFC |
| - | Conservatory |  |
| Creature land | Lumbering Falls | manland |
| - | Lush Oasis |  |
| - | Sharlayan, Nation of Scholars |  |
| - | Kyoshi Village |  |
| - | Windurst, Federation Center |  |
| - | Botanical Plaza |  |
| - | North Pole Gates |  |
| - | Meditation Pools |  |
| - | Woodland Stream |  |
| - | Meandering River |  |
| - | Skybridge Towers |  |
| Campus | University Campus | surveil |
| - | Elfhame Palace |  |
| - | Tranquil Expanse |  |
| - | Suburban Sanctuary | surveil |
| - | Coastal Tower |  |
| Triland | Irrigation Ditch |  |
| - | Paradox Gardens | surveil |
| Pain | Skyshroud Forest | pain |
| Gain/Refuge | Mutant Town | lifegain |


---

## Esper (WUB)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Underground Sea | searchable |
| Verge | Gloomlake Verge |  |
| True dual | Tundra | searchable |
| True dual | Scrubland | searchable |
| Pain | Underground River | pain |
| Verge | Bleachbone Verge |  |
| Verge | Floodfarm Verge |  |
| Pathway | Brightclimb Pathway // Grimclimb Pathway | MDFC |
| Filter | Sunken Ruins | filter |
| Pathway | Clearwater Pathway // Murkwater Pathway | MDFC |
| Pain | Caves of Koilos | pain |
| Filter | Mystic Gate | filter |
| Pathway | Hengegate Pathway // Mistgate Pathway | MDFC |
| Horizon/Canopy | Silent Clearing |  |
| - | Nimbus Maze |  |
| Tainted | Tainted Isle |  |
| Filter | Fetid Heath | filter |
| Pain | Adarkar Wastes | pain |
| Filter | Darkwater Catacombs | filter |
| Tainted | Tainted Field |  |
| Filter | Desolate Mire | filter |
| - | River of Tears |  |
| Filter | Skycloud Expanse | filter |
| Depletion | River Delta |  |
| Storage | Dreadship Reef | storage |
| Depletion | Land Cap |  |
| Storage | Calciform Pools | storage |
| Locked | Cloudcrest Lake |  |
| Triland | Wizards' School |  |
| Triland | Dromar's Cavern |  |
| Locked | Waterveil Cavern |  |
| Locked | Rootwater Depths |  |
| Locked | Thalakos Lowlands |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Morphic Pool |  |
| Shock | Watery Grave | searchable |
| Bond (crowd) | Sea of Clouds |  |
| Shock | Godless Shrine | searchable |
| Bond (crowd) | Vault of Champions |  |
| Shock | Hallowed Fountain | searchable |
| Slow | Shipwreck Marsh |  |
| Check | Drowned Catacomb |  |
| Slow | Deserted Beach |  |
| Slow | Shattered Sanctum |  |
| Battle/Tango | Sunken Hollow | searchable |
| Check | Glacial Fortress |  |
| Fast | Darkslick Shores |  |
| Reveal | Choked Estuary |  |
| Check | Isolated Chapel |  |
| Fast | Concealed Courtyard |  |
| Battle/Tango | Prairie Stream | searchable |
| Reveal | Shineshadow Snarl |  |
| - | Secluded Glen |  |
| Fast | Seachrome Coast |  |
| Catch-up | Turbulent Moor | searchable |
| Battle/Tango | Eclipsed Steppe | searchable |
| Reveal | Port Town |  |
| - | Wanderwine Hub |  |
| - | Abandoned Campground |  |
| - | Murky Sewer |  |
| - | Fortified Beachhead |  |
| - | Neglected Manor |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Undercity Sewers | searchable, surveil |
| Triland | Raffine's Tower | searchable, cycling |
| Surveil land | Shadowy Backstreet | searchable, surveil |
| Surveil land | Meticulous Archive | searchable, surveil |
| Triland | Arcane Sanctum |  |
| Bounce/Karoo | Dimir Aqueduct | bounce |
| Bridge | Goldmire Bridge |  |
| Bridge | Mistvault Bridge |  |
| MDFC spell/land | Waterlogged Teachings // Inundated Archive | MDFC |
| Creature land | Restless Reef | manland |
| Bounce/Karoo | Orzhov Basilica | bounce |
| Scry/Temple | Temple of Enlightenment | scry |
| Creature land | Restless Anchorage | manland |
| Cycling/Bicycle | Fetid Pools | searchable, cycling |
| Bridge | Razortide Bridge |  |
| Scry/Temple | Temple of Deceit | scry |
| Creature land | Restless Fortress | manland |
| Bounce/Karoo | Azorius Chancery | bounce |
| - | Contaminated Aquifer | searchable |
| Snow dual | Snowfield Sinkhole | searchable, snow |
| Snow dual | Ice Tunnel | searchable, snow |
| MDFC spell/land | Glasswing Grace // Age-Graced Chapel | MDFC |
| Scry/Temple | Temple of Silence | scry |
| Creature land | Celestial Colonnade | manland |
| Snow dual | Glacial Floodplain | searchable, snow |
| Gain/Refuge | Sejiri Refuge | lifegain |
| Cycling/Bicycle | Irrigated Farmland | searchable, cycling |
| Gain/Refuge | Jwar Isle Refuge | lifegain |
| Creature land | Creeping Tar Pit | manland |
| - | Idyllic Beachfront | searchable |
| Creature land | Shambling Vent | manland |
| Snow dual | Boreal Shelf | snow |
| Cycling/Bicycle | Umbral Expanse | searchable, cycling |
| Gain/Refuge | Dismal Backwater | lifegain |
| Snow dual | Frost Marsh | snow |
| Gain/Refuge | Scoured Barrens | lifegain |
| - | Sunlit Marsh | searchable |
| Gain/Refuge | Tranquil Cove | lifegain |
| - | Forlorn Flats |  |
| Guildgate | Orzhov Guildgate |  |
| - | Forsaken Sanctuary |  |
| - | Study |  |
| Guildgate | Azorius Guildgate |  |
| Guildgate | Dimir Guildgate |  |
| - | Soured Springs |  |
| - | Waterfront District |  |
| - | Secret Passage |  |
| - | Ballroom |  |
| MDFC spell/land | Suppression Ray // Orderly Plaza | MDFC |
| - | Submerged Boneyard |  |
| Campus | Silverquill Campus | scry |
| - | Insomnia, Crown City |  |
| - | Lonely Arroyo |  |
| - | Serpent's Pass |  |
| - | Treno, Dark City |  |
| - | Sharlayan, Nation of Scholars |  |
| - | North Pole Gates |  |
| - | Salt Marsh |  |
| - | Sinister Hideout | surveil |
| - | Meandering River |  |
| - | Misty Palms Oasis |  |
| - | Skybridge Towers |  |
| Campus | University Campus | surveil |
| - | Coastal Tower |  |
| Triland | Ancient Spring |  |
| - | Forum of Amity | surveil |
| Pain | Salt Flats | pain |
| Gain/Refuge | Foot Headquarters | lifegain |


---

## Grixis (UBR)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Underground Sea | searchable |
| True dual | Volcanic Island | searchable |
| Verge | Gloomlake Verge |  |
| True dual | Badlands | searchable |
| Verge | Riverpyre Verge |  |
| Verge | Blazemire Verge |  |
| Pain | Underground River | pain |
| Pain | Sulfurous Springs | pain |
| Filter | Sunken Ruins | filter |
| Horizon/Canopy | Fiery Islet |  |
| Filter | Graven Cairns | filter |
| Pathway | Riverglide Pathway // Lavaglide Pathway | MDFC |
| Pathway | Blightstep Pathway // Searstep Pathway | MDFC |
| Pathway | Clearwater Pathway // Murkwater Pathway | MDFC |
| - | Mount Doom |  |
| Tainted | Tainted Isle |  |
| Filter | Cascade Bluffs | filter |
| Tainted | Tainted Peak |  |
| Pain | Shivan Reef | pain |
| Filter | Shadowblood Ridge | filter |
| Filter | Darkwater Catacombs | filter |
| Filter | Ferrous Lake | filter |
| - | River of Tears |  |
| Depletion | River Delta |  |
| Depletion | Lava Tubes |  |
| Storage | Dreadship Reef | storage |
| Triland | Crosis's Catacombs |  |
| Triland | Castle Sengir |  |
| Storage | Molten Slagheap | storage |
| Triland | Crypt of the Eternals | lifegain |
| Locked | Waterveil Cavern |  |
| Locked | Lantern-Lit Graveyard |  |
| Locked | Cinder Marsh |  |
| Locked | Rootwater Depths |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Morphic Pool |  |
| Shock | Steam Vents | searchable |
| Shock | Watery Grave | searchable |
| Bond (crowd) | Luxury Suite |  |
| Bond (crowd) | Training Center |  |
| Shock | Blood Crypt | searchable |
| Slow | Shipwreck Marsh |  |
| Slow | Haunted Ridge |  |
| Check | Drowned Catacomb |  |
| Slow | Stormcarved Coast |  |
| Check | Dragonskull Summit |  |
| Battle/Tango | Sunken Hollow | searchable |
| Fast | Spirebluff Canal |  |
| Fast | Darkslick Shores |  |
| Check | Sulfur Falls |  |
| Fast | Blackcleave Cliffs |  |
| Reveal | Choked Estuary |  |
| Battle/Tango | Smoldering Marsh | searchable |
| Reveal | Foreboding Ruins |  |
| - | Secluded Glen |  |
| Reveal | Frostboil Snarl |  |
| Catch-up | Turbulent Springs | searchable |
| Battle/Tango | Scorched Geyser | searchable |
| - | Auntie's Hovel |  |
| MDFC spell/land | Rush of Inspiration // Crackling Falls | MDFC |
| - | Razortrap Gorge |  |
| - | Murky Sewer |  |
| - | Peculiar Lighthouse |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Undercity Sewers | searchable, surveil |
| Triland | Xander's Lounge | searchable, cycling |
| Surveil land | Thundering Falls | searchable, surveil |
| Surveil land | Raucous Theater | searchable, surveil |
| Bounce/Karoo | Dimir Aqueduct | bounce |
| Bounce/Karoo | Izzet Boilerworks | bounce |
| Triland | Crumbling Necropolis |  |
| Bridge | Drossforge Bridge |  |
| Bridge | Mistvault Bridge |  |
| Bounce/Karoo | Rakdos Carnarium | bounce |
| MDFC spell/land | Waterlogged Teachings // Inundated Archive | MDFC |
| Creature land | Restless Reef | manland |
| Cycling/Bicycle | Fetid Pools | searchable, cycling |
| Bridge | Silverbluff Bridge |  |
| Scry/Temple | Temple of Malice | scry |
| Scry/Temple | Temple of Deceit | scry |
| Snow dual | Volatile Fjord | searchable, snow |
| - | Jagged Barrens |  |
| - | Contaminated Aquifer | searchable |
| Snow dual | Ice Tunnel | searchable, snow |
| Triland | Oscorp Industries |  |
| Creature land | Restless Vents | manland |
| Gain/Refuge | Akoum Refuge | lifegain |
| Cycling/Bicycle | Canyon Slough | searchable, cycling |
| - | Geothermal Bog | searchable |
| Scry/Temple | Temple of Epiphany | scry |
| Gain/Refuge | Jwar Isle Refuge | lifegain |
| Creature land | Creeping Tar Pit | manland |
| Gain/Refuge | Bloodfell Caves | lifegain |
| Gain/Refuge | Dismal Backwater | lifegain |
| Snow dual | Frost Marsh | snow |
| - | Molten Tributary | searchable |
| Creature land | Lavaclaw Reaches | manland |
| Snow dual | Sulfurous Mire | searchable, snow |
| Gain/Refuge | Swiftwater Cliffs | lifegain |
| - | Eroded Canyon |  |
| Cycling/Bicycle | Coastal Peak | searchable, cycling |
| Guildgate | Izzet Guildgate |  |
| Snow dual | Tresserhorn Sinks | snow |
| Guildgate | Dimir Guildgate |  |
| - | Waterfront District |  |
| - | Secret Passage |  |
| - | Library |  |
| Guildgate | Rakdos Guildgate |  |
| - | Soured Springs |  |
| - | Vector, Imperial Capital |  |
| - | Submerged Boneyard |  |
| Creature land | Restless Spire | manland, scry |
| Campus | Prismari Campus | scry |
| Creature land | Wandering Fumarole | manland |
| - | Boiling Rock Prison |  |
| - | Baron, Airship Kingdom |  |
| - | Billiard Room |  |
| - | Treno, Dark City |  |
| - | Urborg Volcano |  |
| - | Serpent's Pass |  |
| - | Cinder Barrens |  |
| - | Airship Engine Room |  |
| - | Ominous Asylum | surveil |
| - | Highland Lake |  |
| Triland | Sulfur Vent |  |
| - | Salt Marsh |  |
| - | Tramway Station |  |
| - | Sinister Hideout | surveil |
| - | Spectacle Summit | surveil |
| Gain/Refuge | TCRI Building | lifegain |
| Pain | Caldera Lake | pain |


---

## Jund (BRG)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Badlands | searchable |
| Verge | Blazemire Verge |  |
| True dual | Bayou | searchable |
| True dual | Taiga | searchable |
| Verge | Wastewood Verge |  |
| Pain | Sulfurous Springs | pain |
| Filter | Graven Cairns | filter |
| - | Mount Doom |  |
| Pain | Llanowar Wastes | pain |
| Pathway | Blightstep Pathway // Searstep Pathway | MDFC |
| Verge | Thornspire Verge |  |
| Pathway | Darkbore Pathway // Slitherbore Pathway | MDFC |
| Filter | Fire-Lit Thicket | filter |
| Pathway | Cragcrown Pathway // Timbercrown Pathway | MDFC |
| Pain | Karplusan Forest | pain |
| Horizon/Canopy | Nurturing Peatland |  |
| Filter | Twilight Mire | filter |
| Tainted | Tainted Peak |  |
| Filter | Shadowblood Ridge | filter |
| Reverse-pain | Grove of the Burnwillows |  |
| Tainted | Tainted Wood |  |
| Filter | Viridescent Bog | filter |
| Filter | Mossfire Valley | filter |
| Depletion | Lava Tubes |  |
| Depletion | Timberline Ridge |  |
| Triland | Darigaaz's Caldera |  |
| Storage | Molten Slagheap | storage |
| Locked | Pinecrest Ridge |  |
| Locked | Lantern-Lit Graveyard |  |
| Triland | Koskun Keep |  |
| Storage | Fungal Reaches | storage |
| Locked | Cinder Marsh |  |
| Locked | Mogg Hollows |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Luxury Suite |  |
| Shock | Blood Crypt | searchable |
| Shock | Overgrown Tomb | searchable |
| Shock | Stomping Ground | searchable |
| Slow | Haunted Ridge |  |
| Bond (crowd) | Undergrowth Stadium |  |
| Bond (crowd) | Spire Garden |  |
| Slow | Rockfall Vale |  |
| Check | Dragonskull Summit |  |
| Slow | Deathcap Glade |  |
| Check | Woodland Cemetery |  |
| Battle/Tango | Cinder Glade | searchable |
| Check | Rootbound Crag |  |
| Fast | Blackcleave Cliffs |  |
| Battle/Tango | Smoldering Marsh | searchable |
| Fast | Blooming Marsh |  |
| Battle/Tango | Vernal Fen | searchable |
| Reveal | Necroblossom Snarl |  |
| Reveal | Foreboding Ruins |  |
| - | Gilt-Leaf Palace |  |
| Fast | Copperline Gorge |  |
| Reveal | Game Trail |  |
| Catch-up | Turbulent Fen | searchable |
| - | Auntie's Hovel |  |
| - | Razortrap Gorge |  |
| - | Strangled Cemetery |  |
| - | Bleeding Woods |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Surveil land | Underground Mortuary | searchable, surveil |
| Triland | Ziatora's Proving Ground | searchable, cycling |
| Surveil land | Raucous Theater | searchable, surveil |
| Surveil land | Commercial District | searchable, surveil |
| MDFC spell/land | Revitalizing Repast // Old-Growth Grove | MDFC |
| Bounce/Karoo | Golgari Rot Farm | bounce |
| Bridge | Drossforge Bridge |  |
| Bounce/Karoo | Rakdos Carnarium | bounce |
| Creature land | Restless Cottage | manland |
| Triland | Savage Lands |  |
| MDFC spell/land | Stump Stomp // Burnwillow Clearing | MDFC |
| Bounce/Karoo | Gruul Turf | bounce |
| Snow dual | Woodland Chasm | searchable, snow |
| Scry/Temple | Temple of Malice | scry |
| Scry/Temple | Temple of Abandon | scry |
| Snow dual | Highland Forest | searchable, snow |
| - | Jagged Barrens |  |
| - | Haunted Mire | searchable |
| Creature land | Restless Ridgeline | manland |
| Cycling/Bicycle | Sheltered Thicket | searchable, cycling |
| Scry/Temple | Temple of Malady | scry |
| Creature land | Restless Vents | manland |
| Bridge | Darkmoss Bridge |  |
| Cycling/Bicycle | Festering Thicket | searchable, cycling |
| Creature land | Hissing Quagmire | manland |
| Gain/Refuge | Akoum Refuge | lifegain |
| - | Wooded Ridgeline | searchable |
| - | Geothermal Bog | searchable |
| Cycling/Bicycle | Canyon Slough | searchable, cycling |
| Bridge | Slagwoods Bridge |  |
| Gain/Refuge | Bloodfell Caves | lifegain |
| Gain/Refuge | Jungle Hollow | lifegain |
| Snow dual | Sulfurous Mire | searchable, snow |
| Creature land | Lavaclaw Reaches | manland |
| Gain/Refuge | Rugged Highlands | lifegain |
| - | Festering Gulch |  |
| Snow dual | Tresserhorn Sinks | snow |
| - | Bristling Backwoods |  |
| Campus | Witherbloom Campus | scry |
| Guildgate | Gruul Guildgate |  |
| Guildgate | Golgari Guildgate |  |
| Creature land | Raging Ravine | manland |
| - | Vector, Imperial Capital |  |
| Guildgate | Rakdos Guildgate |  |
| Gain/Refuge | Kazandu Refuge | lifegain |
| - | Dining Room |  |
| - | Gongaga, Reactor Town |  |
| - | Boiling Rock Prison |  |
| Snow dual | Highland Weald | snow |
| - | Billiard Room |  |
| - | Urborg Volcano |  |
| - | Foul Orchard |  |
| - | Timber Gorge |  |
| - | Gohn, Town of Ruin |  |
| - | Omashu City |  |
| - | Cinder Barrens |  |
| Triland | Geothermal Crevice |  |
| - | Ominous Asylum | surveil |
| - | Foggy Bottom Swamp |  |
| - | Lounge |  |
| - | Titan's Grave | surveil |
| - | Tramway Station |  |
| - | Racers' Ring |  |
| - | Savage Mansion | surveil |
| - | Shivan Oasis |  |
| Gain/Refuge | Illegitimate Business | lifegain |
| Pain | Pine Barrens | pain |


---

## Naya (RGW)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Taiga | searchable |
| True dual | Plateau | searchable |
| Verge | Sunbillow Verge |  |
| Verge | Hushwood Verge |  |
| True dual | Savannah | searchable |
| Pain | Brushland | pain |
| Verge | Thornspire Verge |  |
| Pathway | Needleverge Pathway // Pillarverge Pathway | MDFC |
| Filter | Fire-Lit Thicket | filter |
| Filter | Wooded Bastion | filter |
| Pathway | Cragcrown Pathway // Timbercrown Pathway | MDFC |
| Pathway | Branchloft Pathway // Boulderloft Pathway | MDFC |
| Pain | Karplusan Forest | pain |
| Horizon/Canopy | Sunbaked Canyon |  |
| Horizon/Canopy | Horizon Canopy |  |
| Reverse-pain | Grove of the Burnwillows |  |
| Filter | Rugged Prairie | filter |
| Filter | Sunscorched Divide | filter |
| Pain | Battlefield Forge | pain |
| Filter | Sungrass Prairie | filter |
| Filter | Mossfire Valley | filter |
| - | Riftstone Portal |  |
| Depletion | Veldt |  |
| Depletion | Timberline Ridge |  |
| Triland | Rith's Grove |  |
| Storage | Saltcrusted Steppe | storage |
| Triland | An-Havva Township |  |
| Locked | Pinecrest Ridge |  |
| Locked | Tranquil Garden |  |
| Storage | Fungal Reaches | storage |
| Locked | Mogg Hollows |  |
| Locked | Vec Townships |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Sacred Foundry | searchable |
| Bond (crowd) | Spectator Seating |  |
| Shock | Stomping Ground | searchable |
| Bond (crowd) | Bountiful Promenade |  |
| Shock | Temple Garden | searchable |
| Bond (crowd) | Spire Garden |  |
| Slow | Rockfall Vale |  |
| Slow | Overgrown Farmland |  |
| Slow | Sundown Pass |  |
| Check | Sunpetal Grove |  |
| Battle/Tango | Cinder Glade | searchable |
| Check | Rootbound Crag |  |
| Check | Clifftop Retreat |  |
| Fast | Inspiring Vantage |  |
| Battle/Tango | Radiant Summit | searchable |
| Fast | Razorverge Thicket |  |
| Battle/Tango | Canopy Vista | searchable |
| Fast | Copperline Gorge |  |
| Reveal | Game Trail |  |
| Reveal | Fortified Village |  |
| Reveal | Furycalm Snarl |  |
| Catch-up | Turbulent Steppe | searchable |
| - | Ancient Amphitheater |  |
| - | Raucous Carnival |  |
| - | Bleeding Woods |  |
| - | Etched Cornfield |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Jetmir's Garden | searchable, cycling |
| Surveil land | Elegant Parlor | searchable, surveil |
| Surveil land | Commercial District | searchable, surveil |
| Surveil land | Lush Portico | searchable, surveil |
| Triland | Jungle Shrine |  |
| MDFC spell/land | Legion Leadership // Legion Stronghold | MDFC |
| MDFC spell/land | Stump Stomp // Burnwillow Clearing | MDFC |
| Bounce/Karoo | Gruul Turf | bounce |
| Scry/Temple | Temple of Plenty | scry |
| MDFC spell/land | Strength of the Harvest // Haven of the Harvest | MDFC |
| Snow dual | Highland Forest | searchable, snow |
| Bounce/Karoo | Selesnya Sanctuary | bounce |
| Bridge | Rustvale Bridge |  |
| Scry/Temple | Temple of Abandon | scry |
| Cycling/Bicycle | Scattered Groves | searchable, cycling |
| Creature land | Restless Bivouac | manland |
| Cycling/Bicycle | Sheltered Thicket | searchable, cycling |
| Creature land | Restless Ridgeline | manland |
| Snow dual | Arctic Treeline | searchable, snow |
| Scry/Temple | Temple of Triumph | scry |
| - | Wooded Ridgeline | searchable |
| Creature land | Restless Prairie | manland |
| Bridge | Slagwoods Bridge |  |
| - | Sacred Peaks | searchable |
| Bounce/Karoo | Boros Garrison | bounce |
| - | Abraded Bluffs |  |
| Snow dual | Alpine Meadow | searchable, snow |
| Cycling/Bicycle | Glittering Massif | searchable, cycling |
| Snow dual | Arctic Flats | snow |
| Gain/Refuge | Blossoming Sands | lifegain |
| Bridge | Thornglint Bridge |  |
| - | Radiant Grove | searchable |
| Gain/Refuge | Wind-Scarred Crag | lifegain |
| Gain/Refuge | Rugged Highlands | lifegain |
| Creature land | Stirring Wildwood | manland |
| Gain/Refuge | Graypelt Refuge | lifegain |
| Creature land | Needle Spires | manland |
| - | Bristling Backwoods |  |
| - | Creosote Heath |  |
| Creature land | Raging Ravine | manland |
| Guildgate | Selesnya Guildgate |  |
| Guildgate | Gruul Guildgate |  |
| Guildgate | Boros Guildgate |  |
| Campus | Lorehold Campus | scry |
| - | Conservatory |  |
| Gain/Refuge | Kazandu Refuge | lifegain |
| - | Dining Room |  |
| - | Gongaga, Reactor Town |  |
| Snow dual | Highland Weald | snow |
| - | Botanical Plaza |  |
| - | Kyoshi Village |  |
| - | Sun-Blessed Peak |  |
| - | Hall |  |
| - | Windurst, Federation Center |  |
| - | Timber Gorge |  |
| - | Rabanastre, Royal City |  |
| - | Omashu City |  |
| - | Stone Quarry |  |
| - | Fields of Strife | surveil |
| - | Elfhame Palace |  |
| - | Racers' Ring |  |
| - | Tranquil Expanse |  |
| - | Suburban Sanctuary | surveil |
| - | Savage Mansion | surveil |
| - | Shivan Oasis |  |
| Triland | Tinder Farm |  |
| Pain | Scabland | pain |
| Gain/Refuge | Dimension X | lifegain |


---

## Abzan (WBG)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Scrubland | searchable |
| True dual | Bayou | searchable |
| Verge | Bleachbone Verge |  |
| True dual | Savannah | searchable |
| Verge | Wastewood Verge |  |
| Verge | Hushwood Verge |  |
| Pain | Brushland | pain |
| Pathway | Brightclimb Pathway // Grimclimb Pathway | MDFC |
| Pain | Llanowar Wastes | pain |
| Pathway | Darkbore Pathway // Slitherbore Pathway | MDFC |
| Pain | Caves of Koilos | pain |
| Filter | Wooded Bastion | filter |
| Horizon/Canopy | Nurturing Peatland |  |
| Horizon/Canopy | Silent Clearing |  |
| Pathway | Branchloft Pathway // Boulderloft Pathway | MDFC |
| Horizon/Canopy | Horizon Canopy |  |
| Filter | Twilight Mire | filter |
| Filter | Fetid Heath | filter |
| Tainted | Tainted Field |  |
| Filter | Viridescent Bog | filter |
| Tainted | Tainted Wood |  |
| Filter | Sungrass Prairie | filter |
| Filter | Desolate Mire | filter |
| - | Riftstone Portal |  |
| Depletion | Veldt |  |
| Storage | Saltcrusted Steppe | storage |
| Locked | Tranquil Garden |  |
| Locked | Vec Townships |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Bond (crowd) | Vault of Champions |  |
| Shock | Godless Shrine | searchable |
| Shock | Overgrown Tomb | searchable |
| Bond (crowd) | Bountiful Promenade |  |
| Shock | Temple Garden | searchable |
| Bond (crowd) | Undergrowth Stadium |  |
| Slow | Overgrown Farmland |  |
| Slow | Shattered Sanctum |  |
| Check | Sunpetal Grove |  |
| Slow | Deathcap Glade |  |
| Check | Woodland Cemetery |  |
| Check | Isolated Chapel |  |
| Fast | Blooming Marsh |  |
| Fast | Concealed Courtyard |  |
| Battle/Tango | Vernal Fen | searchable |
| Reveal | Necroblossom Snarl |  |
| Fast | Razorverge Thicket |  |
| Battle/Tango | Canopy Vista | searchable |
| - | Gilt-Leaf Palace |  |
| Reveal | Shineshadow Snarl |  |
| Catch-up | Turbulent Fen | searchable |
| Reveal | Fortified Village |  |
| Triland | Murmuring Bosk | searchable, pain |
| Catch-up | Turbulent Moor | searchable |
| Battle/Tango | Eclipsed Steppe | searchable |
| - | Strangled Cemetery |  |
| - | Neglected Manor |  |
| - | Etched Cornfield |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Indatha Triome | searchable, cycling |
| Surveil land | Underground Mortuary | searchable, surveil |
| Surveil land | Shadowy Backstreet | searchable, surveil |
| Surveil land | Lush Portico | searchable, surveil |
| MDFC spell/land | Revitalizing Repast // Old-Growth Grove | MDFC |
| Bridge | Goldmire Bridge |  |
| Bounce/Karoo | Golgari Rot Farm | bounce |
| Creature land | Restless Cottage | manland |
| Bounce/Karoo | Orzhov Basilica | bounce |
| Scry/Temple | Temple of Plenty | scry |
| Triland | Sandsteppe Citadel |  |
| Snow dual | Woodland Chasm | searchable, snow |
| MDFC spell/land | Strength of the Harvest // Haven of the Harvest | MDFC |
| Bounce/Karoo | Selesnya Sanctuary | bounce |
| Creature land | Restless Fortress | manland |
| Scry/Temple | Temple of Silence | scry |
| Cycling/Bicycle | Scattered Groves | searchable, cycling |
| - | Haunted Mire | searchable |
| MDFC spell/land | Glasswing Grace // Age-Graced Chapel | MDFC |
| Snow dual | Snowfield Sinkhole | searchable, snow |
| Scry/Temple | Temple of Malady | scry |
| Snow dual | Arctic Treeline | searchable, snow |
| Bridge | Darkmoss Bridge |  |
| Cycling/Bicycle | Festering Thicket | searchable, cycling |
| Creature land | Hissing Quagmire | manland |
| Creature land | Restless Prairie | manland |
| Creature land | Shambling Vent | manland |
| Snow dual | Arctic Flats | snow |
| Gain/Refuge | Blossoming Sands | lifegain |
| Gain/Refuge | Jungle Hollow | lifegain |
| - | Radiant Grove | searchable |
| Gain/Refuge | Scoured Barrens | lifegain |
| Cycling/Bicycle | Umbral Expanse | searchable, cycling |
| - | Sunlit Marsh | searchable |
| Bridge | Thornglint Bridge |  |
| Gain/Refuge | Graypelt Refuge | lifegain |
| - | Festering Gulch |  |
| Creature land | Stirring Wildwood | manland |
| Guildgate | Golgari Guildgate |  |
| Guildgate | Orzhov Guildgate |  |
| Guildgate | Selesnya Guildgate |  |
| - | Creosote Heath |  |
| - | Forsaken Sanctuary |  |
| - | Forlorn Flats |  |
| Campus | Witherbloom Campus | scry |
| - | Ballroom |  |
| Campus | Silverquill Campus | scry |
| - | Conservatory |  |
| - | Insomnia, Crown City |  |
| - | Foul Orchard |  |
| - | Windurst, Federation Center |  |
| - | Kyoshi Village |  |
| - | Botanical Plaza |  |
| - | Gohn, Town of Ruin |  |
| - | Foggy Bottom Swamp |  |
| - | Titan's Grave | surveil |
| - | Lounge |  |
| - | Misty Palms Oasis |  |
| - | Tranquil Expanse |  |
| - | Elfhame Palace |  |
| - | Suburban Sanctuary | surveil |
| - | Forum of Amity | surveil |
| Gain/Refuge | Illegitimate Business | lifegain |
| Gain/Refuge | Foot Headquarters | lifegain |
| Pain | Salt Flats | pain |
| Pain | Pine Barrens | pain |


---

## Jeskai (URW)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Volcanic Island | searchable |
| Verge | Riverpyre Verge |  |
| True dual | Tundra | searchable |
| Verge | Floodfarm Verge |  |
| True dual | Plateau | searchable |
| Verge | Sunbillow Verge |  |
| Horizon/Canopy | Fiery Islet |  |
| Pathway | Riverglide Pathway // Lavaglide Pathway | MDFC |
| Pathway | Needleverge Pathway // Pillarverge Pathway | MDFC |
| Filter | Mystic Gate | filter |
| Pathway | Hengegate Pathway // Mistgate Pathway | MDFC |
| - | Nimbus Maze |  |
| Horizon/Canopy | Sunbaked Canyon |  |
| Pain | Shivan Reef | pain |
| Filter | Cascade Bluffs | filter |
| Pain | Adarkar Wastes | pain |
| Filter | Ferrous Lake | filter |
| Filter | Rugged Prairie | filter |
| Filter | Sunscorched Divide | filter |
| Pain | Battlefield Forge | pain |
| Filter | Skycloud Expanse | filter |
| Depletion | Land Cap |  |
| Storage | Calciform Pools | storage |
| Locked | Cloudcrest Lake |  |
| Locked | Thalakos Lowlands |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Steam Vents | searchable |
| Shock | Sacred Foundry | searchable |
| Bond (crowd) | Sea of Clouds |  |
| Bond (crowd) | Training Center |  |
| Bond (crowd) | Spectator Seating |  |
| Shock | Hallowed Fountain | searchable |
| Slow | Deserted Beach |  |
| Slow | Stormcarved Coast |  |
| Slow | Sundown Pass |  |
| Check | Glacial Fortress |  |
| Fast | Spirebluff Canal |  |
| Check | Sulfur Falls |  |
| Check | Clifftop Retreat |  |
| Fast | Inspiring Vantage |  |
| Battle/Tango | Prairie Stream | searchable |
| Battle/Tango | Radiant Summit | searchable |
| Fast | Seachrome Coast |  |
| Reveal | Furycalm Snarl |  |
| Reveal | Frostboil Snarl |  |
| Catch-up | Turbulent Springs | searchable |
| Reveal | Port Town |  |
| Catch-up | Turbulent Steppe | searchable |
| Battle/Tango | Scorched Geyser | searchable |
| - | Wanderwine Hub |  |
| MDFC spell/land | Rush of Inspiration // Crackling Falls | MDFC |
| - | Ancient Amphitheater |  |
| - | Abandoned Campground |  |
| - | Raucous Carnival |  |
| - | Fortified Beachhead |  |
| - | Peculiar Lighthouse |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Raugrin Triome | searchable, cycling |
| Surveil land | Thundering Falls | searchable, surveil |
| Surveil land | Meticulous Archive | searchable, surveil |
| Surveil land | Elegant Parlor | searchable, surveil |
| Bounce/Karoo | Izzet Boilerworks | bounce |
| MDFC spell/land | Legion Leadership // Legion Stronghold | MDFC |
| Scry/Temple | Temple of Enlightenment | scry |
| Bridge | Razortide Bridge |  |
| Creature land | Restless Anchorage | manland |
| Bounce/Karoo | Azorius Chancery | bounce |
| Bridge | Silverbluff Bridge |  |
| Bridge | Rustvale Bridge |  |
| Snow dual | Volatile Fjord | searchable, snow |
| Creature land | Restless Bivouac | manland |
| Snow dual | Glacial Floodplain | searchable, snow |
| Scry/Temple | Temple of Triumph | scry |
| Triland | Mystic Monastery |  |
| Creature land | Celestial Colonnade | manland |
| Cycling/Bicycle | Irrigated Farmland | searchable, cycling |
| Gain/Refuge | Sejiri Refuge | lifegain |
| Snow dual | Alpine Meadow | searchable, snow |
| Bounce/Karoo | Boros Garrison | bounce |
| - | Sacred Peaks | searchable |
| - | Abraded Bluffs |  |
| Scry/Temple | Temple of Epiphany | scry |
| - | Idyllic Beachfront | searchable |
| Cycling/Bicycle | Glittering Massif | searchable, cycling |
| Gain/Refuge | Wind-Scarred Crag | lifegain |
| Snow dual | Boreal Shelf | snow |
| - | Eroded Canyon |  |
| - | Molten Tributary | searchable |
| Cycling/Bicycle | Coastal Peak | searchable, cycling |
| Gain/Refuge | Swiftwater Cliffs | lifegain |
| Gain/Refuge | Tranquil Cove | lifegain |
| Creature land | Needle Spires | manland |
| - | Study |  |
| Guildgate | Izzet Guildgate |  |
| Guildgate | Azorius Guildgate |  |
| MDFC spell/land | Suppression Ray // Orderly Plaza | MDFC |
| - | Library |  |
| Guildgate | Boros Guildgate |  |
| Campus | Lorehold Campus | scry |
| - | Lonely Arroyo |  |
| Creature land | Restless Spire | manland, scry |
| Creature land | Wandering Fumarole | manland |
| Campus | Prismari Campus | scry |
| - | Baron, Airship Kingdom |  |
| - | Sharlayan, Nation of Scholars |  |
| - | Sun-Blessed Peak |  |
| - | Rabanastre, Royal City |  |
| - | Hall |  |
| - | Airship Engine Room |  |
| - | North Pole Gates |  |
| - | Highland Lake |  |
| - | Stone Quarry |  |
| - | Meandering River |  |
| - | Skybridge Towers |  |
| - | Fields of Strife | surveil |
| Campus | University Campus | surveil |
| - | Spectacle Summit | surveil |
| - | Coastal Tower |  |
| Gain/Refuge | TCRI Building | lifegain |
| Gain/Refuge | Dimension X | lifegain |
| Pain | Caldera Lake | pain |
| Pain | Scabland | pain |


---

## Sultai (BGU)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Underground Sea | searchable |
| True dual | Tropical Island | searchable |
| Verge | Gloomlake Verge |  |
| True dual | Bayou | searchable |
| Pain | Underground River | pain |
| Verge | Wastewood Verge |  |
| Filter | Sunken Ruins | filter |
| Pathway | Clearwater Pathway // Murkwater Pathway | MDFC |
| Verge | Willowrush Verge |  |
| Pain | Llanowar Wastes | pain |
| Pathway | Darkbore Pathway // Slitherbore Pathway | MDFC |
| Pathway | Barkchannel Pathway // Tidechannel Pathway | MDFC |
| Horizon/Canopy | Nurturing Peatland |  |
| Tainted | Tainted Isle |  |
| Pain | Yavimaya Coast | pain |
| Horizon/Canopy | Waterlogged Grove |  |
| Filter | Twilight Mire | filter |
| Filter | Flooded Grove | filter |
| Filter | Darkwater Catacombs | filter |
| Filter | Viridescent Bog | filter |
| Tainted | Tainted Wood |  |
| - | River of Tears |  |
| Filter | Overflowing Basin | filter |
| Depletion | River Delta |  |
| Storage | Dreadship Reef | storage |
| Locked | Waterveil Cavern |  |
| Locked | Rootwater Depths |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Breeding Pool | searchable |
| Bond (crowd) | Morphic Pool |  |
| Shock | Watery Grave | searchable |
| Shock | Overgrown Tomb | searchable |
| Bond (crowd) | Rejuvenating Springs |  |
| Slow | Shipwreck Marsh |  |
| Check | Drowned Catacomb |  |
| Bond (crowd) | Undergrowth Stadium |  |
| Slow | Dreamroot Cascade |  |
| Slow | Deathcap Glade |  |
| Battle/Tango | Sunken Hollow | searchable |
| Check | Woodland Cemetery |  |
| Fast | Darkslick Shores |  |
| Reveal | Choked Estuary |  |
| Fast | Blooming Marsh |  |
| Check | Hinterland Harbor |  |
| Fast | Botanical Sanctum |  |
| Battle/Tango | Vernal Fen | searchable |
| Reveal | Necroblossom Snarl |  |
| - | Gilt-Leaf Palace |  |
| Battle/Tango | Sodden Verdure | searchable |
| - | Secluded Glen |  |
| Catch-up | Turbulent Fen | searchable |
| Catch-up | Turbulent Wilderness | searchable |
| Reveal | Vineglimmer Snarl |  |
| - | Strangled Cemetery |  |
| - | Murky Sewer |  |
| - | Lakeside Shack |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Zagoth Triome | searchable, cycling |
| Surveil land | Undercity Sewers | searchable, surveil |
| Surveil land | Underground Mortuary | searchable, surveil |
| Surveil land | Hedge Maze | searchable, surveil |
| MDFC spell/land | Revitalizing Repast // Old-Growth Grove | MDFC |
| Bounce/Karoo | Dimir Aqueduct | bounce |
| Bounce/Karoo | Golgari Rot Farm | bounce |
| Bridge | Mistvault Bridge |  |
| Triland | Opulent Palace |  |
| Creature land | Restless Cottage | manland |
| Bounce/Karoo | Simic Growth Chamber | bounce |
| MDFC spell/land | Waterlogged Teachings // Inundated Archive | MDFC |
| Creature land | Restless Reef | manland |
| Snow dual | Rimewood Falls | searchable, snow |
| Cycling/Bicycle | Fetid Pools | searchable, cycling |
| Snow dual | Woodland Chasm | searchable, snow |
| Scry/Temple | Temple of Deceit | scry |
| Scry/Temple | Temple of Mystery | scry |
| - | Contaminated Aquifer | searchable |
| Snow dual | Ice Tunnel | searchable, snow |
| - | Haunted Mire | searchable |
| Scry/Temple | Temple of Malady | scry |
| Cycling/Bicycle | Festering Thicket | searchable, cycling |
| Bridge | Darkmoss Bridge |  |
| Creature land | Hissing Quagmire | manland |
| Creature land | Restless Vinestalk | manland |
| Gain/Refuge | Jwar Isle Refuge | lifegain |
| Creature land | Creeping Tar Pit | manland |
| - | Tangled Islet | searchable |
| Bridge | Tanglepool Bridge |  |
| Gain/Refuge | Dismal Backwater | lifegain |
| Gain/Refuge | Jungle Hollow | lifegain |
| Gain/Refuge | Thornwood Falls | lifegain |
| Snow dual | Frost Marsh | snow |
| Cycling/Bicycle | Rain-Slicked Copse | searchable, cycling |
| MDFC spell/land | Balamb Garden, SeeD Academy // Balamb Garden, Airborne | manland, MDFC |
| Guildgate | Simic Guildgate |  |
| - | Festering Gulch |  |
| - | Kitchen |  |
| Guildgate | Golgari Guildgate |  |
| Guildgate | Dimir Guildgate |  |
| - | Secret Passage |  |
| - | Waterfront District |  |
| - | Soured Springs |  |
| Campus | Witherbloom Campus | scry |
| - | Guadosalam, Farplane Gateway |  |
| Campus | Quandrix Campus | scry |
| - | Submerged Boneyard |  |
| MDFC spell/land | Drowner of Truth // Drowned Jungle | MDFC |
| Creature land | Lumbering Falls | manland |
| - | Treno, Dark City |  |
| - | Lush Oasis |  |
| - | Serpent's Pass |  |
| - | Foul Orchard |  |
| - | Gohn, Town of Ruin |  |
| - | Meditation Pools |  |
| - | Woodland Stream |  |
| - | Salt Marsh |  |
| - | Lounge |  |
| - | Foggy Bottom Swamp |  |
| - | Sinister Hideout | surveil |
| - | Titan's Grave | surveil |
| - | Paradox Gardens | surveil |
| Gain/Refuge | Illegitimate Business | lifegain |
| Pain | Pine Barrens | pain |
| Gain/Refuge | Mutant Town | lifegain |
| Pain | Skyshroud Forest | pain |


---

## Mardu (RWB)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Scrubland | searchable |
| True dual | Badlands | searchable |
| Verge | Blazemire Verge |  |
| True dual | Plateau | searchable |
| Verge | Bleachbone Verge |  |
| Pain | Sulfurous Springs | pain |
| Verge | Sunbillow Verge |  |
| Pathway | Brightclimb Pathway // Grimclimb Pathway | MDFC |
| Pathway | Blightstep Pathway // Searstep Pathway | MDFC |
| Filter | Graven Cairns | filter |
| Pathway | Needleverge Pathway // Pillarverge Pathway | MDFC |
| Pain | Caves of Koilos | pain |
| - | Mount Doom |  |
| Horizon/Canopy | Silent Clearing |  |
| Horizon/Canopy | Sunbaked Canyon |  |
| Tainted | Tainted Peak |  |
| Filter | Fetid Heath | filter |
| Filter | Shadowblood Ridge | filter |
| Tainted | Tainted Field |  |
| Filter | Rugged Prairie | filter |
| Filter | Sunscorched Divide | filter |
| Pain | Battlefield Forge | pain |
| Filter | Desolate Mire | filter |
| Depletion | Lava Tubes |  |
| Triland | Tournament Grounds |  |
| Storage | Molten Slagheap | storage |
| Locked | Lantern-Lit Graveyard |  |
| Locked | Cinder Marsh |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Sacred Foundry | searchable |
| Bond (crowd) | Luxury Suite |  |
| Bond (crowd) | Vault of Champions |  |
| Shock | Blood Crypt | searchable |
| Shock | Godless Shrine | searchable |
| Bond (crowd) | Spectator Seating |  |
| Slow | Haunted Ridge |  |
| Slow | Sundown Pass |  |
| Slow | Shattered Sanctum |  |
| Check | Dragonskull Summit |  |
| Fast | Blackcleave Cliffs |  |
| Check | Isolated Chapel |  |
| Battle/Tango | Smoldering Marsh | searchable |
| Fast | Concealed Courtyard |  |
| Fast | Inspiring Vantage |  |
| Check | Clifftop Retreat |  |
| Battle/Tango | Radiant Summit | searchable |
| Reveal | Foreboding Ruins |  |
| Reveal | Shineshadow Snarl |  |
| Catch-up | Turbulent Moor | searchable |
| Reveal | Furycalm Snarl |  |
| Battle/Tango | Eclipsed Steppe | searchable |
| Catch-up | Turbulent Steppe | searchable |
| - | Auntie's Hovel |  |
| - | Ancient Amphitheater |  |
| - | Razortrap Gorge |  |
| - | Raucous Carnival |  |
| - | Neglected Manor |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Savai Triome | searchable, cycling |
| Surveil land | Shadowy Backstreet | searchable, surveil |
| Surveil land | Raucous Theater | searchable, surveil |
| Surveil land | Elegant Parlor | searchable, surveil |
| Triland | Nomad Outpost |  |
| Bridge | Goldmire Bridge |  |
| Bounce/Karoo | Rakdos Carnarium | bounce |
| Bridge | Drossforge Bridge |  |
| MDFC spell/land | Legion Leadership // Legion Stronghold | MDFC |
| Bounce/Karoo | Orzhov Basilica | bounce |
| Scry/Temple | Temple of Malice | scry |
| Creature land | Restless Fortress | manland |
| - | Jagged Barrens |  |
| Creature land | Restless Bivouac | manland |
| Scry/Temple | Temple of Silence | scry |
| Bridge | Rustvale Bridge |  |
| Snow dual | Snowfield Sinkhole | searchable, snow |
| MDFC spell/land | Glasswing Grace // Age-Graced Chapel | MDFC |
| Scry/Temple | Temple of Triumph | scry |
| Creature land | Restless Vents | manland |
| Gain/Refuge | Akoum Refuge | lifegain |
| Cycling/Bicycle | Canyon Slough | searchable, cycling |
| - | Geothermal Bog | searchable |
| Bounce/Karoo | Boros Garrison | bounce |
| - | Sacred Peaks | searchable |
| Snow dual | Alpine Meadow | searchable, snow |
| - | Abraded Bluffs |  |
| Gain/Refuge | Bloodfell Caves | lifegain |
| Creature land | Shambling Vent | manland |
| Cycling/Bicycle | Glittering Massif | searchable, cycling |
| Gain/Refuge | Scoured Barrens | lifegain |
| Cycling/Bicycle | Umbral Expanse | searchable, cycling |
| Gain/Refuge | Wind-Scarred Crag | lifegain |
| Snow dual | Sulfurous Mire | searchable, snow |
| - | Sunlit Marsh | searchable |
| Creature land | Lavaclaw Reaches | manland |
| Creature land | Needle Spires | manland |
| Snow dual | Tresserhorn Sinks | snow |
| - | Forlorn Flats |  |
| - | Forsaken Sanctuary |  |
| Guildgate | Orzhov Guildgate |  |
| - | Ballroom |  |
| Guildgate | Boros Guildgate |  |
| Guildgate | Rakdos Guildgate |  |
| - | Vector, Imperial Capital |  |
| - | Insomnia, Crown City |  |
| Campus | Silverquill Campus | scry |
| Campus | Lorehold Campus | scry |
| - | Billiard Room |  |
| - | Boiling Rock Prison |  |
| - | Urborg Volcano |  |
| - | Rabanastre, Royal City |  |
| - | Sun-Blessed Peak |  |
| - | Cinder Barrens |  |
| - | Hall |  |
| - | Stone Quarry |  |
| - | Ominous Asylum | surveil |
| - | Tramway Station |  |
| - | Misty Palms Oasis |  |
| - | Fields of Strife | surveil |
| - | Forum of Amity | surveil |
| Gain/Refuge | Foot Headquarters | lifegain |
| Gain/Refuge | Dimension X | lifegain |
| Pain | Salt Flats | pain |
| Pain | Scabland | pain |


---

## Temur (GUR)

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| True dual | Volcanic Island | searchable |
| Verge | Riverpyre Verge |  |
| True dual | Tropical Island | searchable |
| True dual | Taiga | searchable |
| Horizon/Canopy | Fiery Islet |  |
| Pathway | Riverglide Pathway // Lavaglide Pathway | MDFC |
| Verge | Thornspire Verge |  |
| Verge | Willowrush Verge |  |
| Filter | Fire-Lit Thicket | filter |
| Pathway | Barkchannel Pathway // Tidechannel Pathway | MDFC |
| Pathway | Cragcrown Pathway // Timbercrown Pathway | MDFC |
| Pain | Karplusan Forest | pain |
| Pain | Yavimaya Coast | pain |
| Pain | Shivan Reef | pain |
| Horizon/Canopy | Waterlogged Grove |  |
| Filter | Cascade Bluffs | filter |
| Filter | Flooded Grove | filter |
| Reverse-pain | Grove of the Burnwillows |  |
| Filter | Ferrous Lake | filter |
| Filter | Mossfire Valley | filter |
| Filter | Overflowing Basin | filter |
| Depletion | Timberline Ridge |  |
| Locked | Pinecrest Ridge |  |
| Storage | Fungal Reaches | storage |
| Locked | Mogg Hollows |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| Shock | Steam Vents | searchable |
| Shock | Breeding Pool | searchable |
| Bond (crowd) | Training Center |  |
| Shock | Stomping Ground | searchable |
| Bond (crowd) | Rejuvenating Springs |  |
| Bond (crowd) | Spire Garden |  |
| Slow | Stormcarved Coast |  |
| Slow | Rockfall Vale |  |
| Slow | Dreamroot Cascade |  |
| Fast | Spirebluff Canal |  |
| Battle/Tango | Cinder Glade | searchable |
| Check | Rootbound Crag |  |
| Check | Sulfur Falls |  |
| Fast | Botanical Sanctum |  |
| Check | Hinterland Harbor |  |
| Fast | Copperline Gorge |  |
| Reveal | Game Trail |  |
| Battle/Tango | Sodden Verdure | searchable |
| Reveal | Frostboil Snarl |  |
| Catch-up | Turbulent Springs | searchable |
| Catch-up | Turbulent Wilderness | searchable |
| Reveal | Vineglimmer Snarl |  |
| Battle/Tango | Scorched Geyser | searchable |
| MDFC spell/land | Rush of Inspiration // Crackling Falls | MDFC |
| - | Bleeding Woods |  |
| - | Peculiar Lighthouse |  |
| - | Lakeside Shack |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| Triland | Ketria Triome | searchable, cycling |
| Surveil land | Hedge Maze | searchable, surveil |
| Surveil land | Thundering Falls | searchable, surveil |
| Surveil land | Commercial District | searchable, surveil |
| Bounce/Karoo | Izzet Boilerworks | bounce |
| Bounce/Karoo | Simic Growth Chamber | bounce |
| MDFC spell/land | Stump Stomp // Burnwillow Clearing | MDFC |
| Snow dual | Rimewood Falls | searchable, snow |
| Triland | Frontier Bivouac |  |
| Bounce/Karoo | Gruul Turf | bounce |
| Bridge | Silverbluff Bridge |  |
| Scry/Temple | Temple of Abandon | scry |
| Snow dual | Highland Forest | searchable, snow |
| Cycling/Bicycle | Sheltered Thicket | searchable, cycling |
| Scry/Temple | Temple of Mystery | scry |
| Snow dual | Volatile Fjord | searchable, snow |
| Creature land | Restless Ridgeline | manland |
| - | Wooded Ridgeline | searchable |
| Bridge | Slagwoods Bridge |  |
| Creature land | Restless Vinestalk | manland |
| Scry/Temple | Temple of Epiphany | scry |
| Bridge | Tanglepool Bridge |  |
| - | Tangled Islet | searchable |
| - | Molten Tributary | searchable |
| - | Eroded Canyon |  |
| Cycling/Bicycle | Rain-Slicked Copse | searchable, cycling |
| Gain/Refuge | Swiftwater Cliffs | lifegain |
| Gain/Refuge | Rugged Highlands | lifegain |
| MDFC spell/land | Balamb Garden, SeeD Academy // Balamb Garden, Airborne | manland, MDFC |
| Gain/Refuge | Thornwood Falls | lifegain |
| Cycling/Bicycle | Coastal Peak | searchable, cycling |
| - | Bristling Backwoods |  |
| - | Kitchen |  |
| Guildgate | Simic Guildgate |  |
| Creature land | Raging Ravine | manland |
| Guildgate | Izzet Guildgate |  |
| - | Library |  |
| Guildgate | Gruul Guildgate |  |
| - | Guadosalam, Farplane Gateway |  |
| Gain/Refuge | Kazandu Refuge | lifegain |
| Campus | Quandrix Campus | scry |
| MDFC spell/land | Drowner of Truth // Drowned Jungle | MDFC |
| Creature land | Wandering Fumarole | manland |
| Campus | Prismari Campus | scry |
| Creature land | Restless Spire | manland, scry |
| - | Dining Room |  |
| - | Gongaga, Reactor Town |  |
| - | Baron, Airship Kingdom |  |
| Creature land | Lumbering Falls | manland |
| Snow dual | Highland Weald | snow |
| - | Lush Oasis |  |
| - | Timber Gorge |  |
| - | Airship Engine Room |  |
| - | Omashu City |  |
| - | Meditation Pools |  |
| - | Highland Lake |  |
| - | Woodland Stream |  |
| - | Spectacle Summit | surveil |
| - | Racers' Ring |  |
| - | Savage Mansion | surveil |
| - | Paradox Gardens | surveil |
| - | Shivan Oasis |  |
| Gain/Refuge | TCRI Building | lifegain |
| Pain | Caldera Lake | pain |
| Gain/Refuge | Mutant Town | lifegain |
| Pain | Skyshroud Forest | pain |


---

## Any-color (generic fixing)

Tap for any color; run in any identity. 150 cards.

### Enters untapped

| Cycle | Card | Tags |
|---|---|---|
| - | Cavern of Souls |  |
| - | Mana Confluence |  |
| - | Nykthos, Shrine to Nyx |  |
| - | Gemstone Caverns |  |
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
| - | Secluded Courtyard |  |
| - | Cascading Cataracts |  |
| - | Planar Nexus |  |
| - | Command Tower |  |
| MDFC spell/land | Dowsing Dagger // Lost Vale | MDFC |
| MDFC spell/land | Matzalantli, the Great Door // The Core | MDFC |
| - | Unclaimed Territory |  |
| - | Baldur's Gate |  |
| - | Abstergo Entertainment |  |
| - | Maelstrom of the Spirit Dragon |  |
| - | Exotic Orchard |  |
| MDFC spell/land | Storm the Vault // Vault of Catlacan | MDFC |
| - | Sliver Hive |  |
| - | Gond Gate |  |
| - | Abundant Countryside |  |
| - | Gemstone Mine |  |
| MDFC spell/land | Journey to Eternity // Atzal, Cave of Eternity | MDFC |
| - | The Mycosynth Gardens |  |
| - | Lotus Vale |  |
| - | Opal Palace |  |
| - | Haven of the Spirit Dragon |  |
| - | Glimmervoid |  |
| - | Mirrex |  |
| - | Spire of Industry |  |
| - | Great Hall of the Citadel |  |
| MDFC spell/land | Treasure Map // Treasure Cove | MDFC, scry |
| MDFC spell/land | Hadana's Climb // Winged Temple of Orazca | MDFC |
| Storage | Crucible of the Spirit Dragon | storage |
| - | Survivors' Encampment |  |
| - | Heap Gate |  |
| - | Ancient Ziggurat |  |
| Creature land | Mech Hangar | manland |
| - | Jasmine Dragon Tea Shop |  |
| - | Meteor Crater |  |
| - | The Grey Havens | scry |
| - | Undiscovered Paradise |  |
| - | Pillar of the Paruns |  |
| - | Conduit Pylons | surveil |
| Bridge | Tendo Ice Bridge |  |
| MDFC spell/land | Azor's Gateway // Sanctum of the Sun | MDFC |
| MDFC spell/land | Golden Guardian // Gold-Forge Garrison | MDFC |
| Horizon/Canopy | Voldaren Estate |  |
| Locked | Forsaken City |  |
| - | Eclipsed Realms |  |
| - | Ally Encampment |  |
| - | Thran Quarry |  |
| Scry/Temple | Crystal Grotto | scry |
| - | Aether Hub |  |
| - | Plaza of Harmony |  |
| - | Hall of Tagsin |  |
| - | The Seedcore |  |
| - | Hidden Grotto | surveil |
| - | Holdout Settlement |  |
| - | Springjack Pasture |  |
| - | Daily Bugle Building |  |
| Scry/Temple | Rumble Arena | scry |
| - | Gallifrey Council Chamber | surveil |
| Creature land | Great Hall of the Biblioplex | manland |
| - | Capital City | cycling |
| MDFC spell/land | Profane Procession // Tomb of the Dusk Rose | MDFC |
| - | Turtle Lair |  |
| MDFC spell/land | Path of Mettle // Metzali, Tower of Triumph | MDFC |
| - | Archaeological Dig |  |
| - | Brotherhood Headquarters |  |
| - | White Lotus Hideout |  |
| - | Hall of Oracles |  |
| - | Study Hall | scry |
| - | Guildmages' Forum |  |
| - | Captivating Cave |  |
| - | Paliano, the High City |  |
| - | Interplanar Beacon | lifegain |
| - | Rhystic Cave |  |
| - | Henge of Ramos |  |
| - | Cave of Temptation |  |
| - | Painted Bluffs |  |
| - | Corrupted Crossroads |  |
| - | Bucolic Ranch |  |
| - | Branch of Vitu-Ghazi |  |
| - | Mirrodin's Core |  |
| - | Shimmering Grotto |  |
| - | Unknown Shores |  |
| - | Rainbow Vale |  |
| - | Throne of Makindi |  |
| - | School of the Unseen |  |
| - | Forgotten Monument |  |

### Conditional (untapped only if a condition is met)

| Cycle | Card | Tags |
|---|---|---|
| - | Starting Town |  |
| Scry/Temple | Temple of the Dragon Queen |  |
| Bridge | Command Bridge |  |
| - | Transguild Promenade |  |
| Guildgate | Gateway Plaza |  |
| - | Primal Beyond |  |
| - | Public Thoroughfare |  |
| - | Rupture Spire |  |
| - | Archway Commons |  |

### Enters tapped

| Cycle | Card | Tags |
|---|---|---|
| - | Lotus Field |  |
| - | Path of Ancestry | scry |
| - | Valgavoth's Lair |  |
| Creature land | Cactus Preserve | manland |
| - | Sea Gate |  |
| - | Citadel Gate |  |
| - | Power Depot |  |
| - | Manor Gate |  |
| - | Hidden Hideout |  |
| - | Black Dragon Gate |  |
| - | Thriving Isle |  |
| - | Cliffgate |  |
| - | Vivid Grove |  |
| - | Scene of the Crime |  |
| - | Thriving Moor |  |
| - | Vivid Creek |  |
| - | Sunken Citadel |  |
| MDFC spell/land | Bloodsoaked Insight // Sanguine Morass | MDFC |
| - | Vivid Meadow |  |
| - | Vivid Marsh |  |
| - | Pit of Offerings |  |
| - | Thriving Heath |  |
| - | Vivid Crag |  |
| Pain | Grand Coliseum | pain |
| - | Tarnation Vista |  |
| - | Thriving Bluff |  |
| - | Big Apple, 3 a.m. |  |
| - | Thriving Grove |  |
| - | Mirage Mesa |  |
| - | Crossroads Village |  |
| - | Uncharted Haven |  |
| - | Edgewall Inn |  |
| Snow dual | Shimmerdrift Vale | snow |
| - | Crumbling Vestige |  |
| - | Abandoned Outpost |  |
| - | Night Market | cycling |
| - | Seafloor Debris |  |
| - | Cryptic Spires |  |
| - | Timberland Ruins |  |
| - | Base Camp |  |
| - | Ravaged Highlands |  |
| - | Bog Wreckage |  |
