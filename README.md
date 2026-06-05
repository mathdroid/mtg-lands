# mtg-lands

Classify and rank the dual / fixing lands for any Magic color identity.

`mtg-lands` is a standalone script that wraps the
[`scry`](https://github.com/mathdroid/scry) CLI. For a color identity it pulls
every Commander-legal land that fits the identity and can make the relevant
colors, then sorts each land into a known cycle (true dual, shock, fast, check,
pain, filter, verge, ...) using color-agnostic oracle-text patterns, and ranks
them.

Full generated reports live in [`reports/`](reports/):
[all pairs](reports/all-pairs.md) and [all triples](reports/all-triples.md).

## Best fixing per guild

Top of each guild's list: the unconditional true dual (T0), the best-scoring
conditional/untapped land (T1), and the most-played T1.

| Guild | T0 true dual | Best-scoring T1 | Most-played T1 |
|---|---|---|---|
| Azorius WU | Tundra | Sea of Clouds | Hallowed Fountain |
| Dimir UB | Underground Sea | Morphic Pool | Watery Grave |
| Rakdos BR | Badlands | Luxury Suite | Blood Crypt |
| Gruul RG | Taiga | Stomping Ground | Stomping Ground |
| Selesnya GW | Savannah | Bountiful Promenade | Temple Garden |
| Orzhov WB | Scrubland | Vault of Champions | Godless Shrine |
| Izzet UR | Volcanic Island | Steam Vents | Steam Vents |
| Golgari BG | Bayou | Overgrown Tomb | Overgrown Tomb |
| Boros RW | Plateau | Sacred Foundry | Sacred Foundry |
| Simic GU | Tropical Island | Breeding Pool | Breeding Pool |

## Ranking

Lands are ranked **tier first**, then by a popularity+price combo inside each
tier. The tier is the land's fixing quality:

- **T0** True dual - untapped, no drawback, basic land types (e.g. Taiga).
- **T1** Untapped or conditionally untapped (shock, fast, check, pain, filter,
  verge, bond, pathway, slow, battle/tango, horizon, reveal, triland).
- **T2** Enters tapped but with upside (scry/temple, surveil, gain/refuge,
  bounce/karoo, cycling, creature land, snow, storage, tapped utility).
- **T3** Plain tapped or weak (guildgate, depletion, locked, plain taplands).
- **Generic** Taps for any color - recurs in every identity, listed separately.

Tier dominates so an unconditional true dual is always #1, even when Scryfall
has no price for it (Reserved List cards often report a null price; the score
falls back to popularity rather than treating them as $0).

The within-tier score is the average of two percentiles across the result set:
EDHREC rank (more played = higher) and USD price (more expensive = higher, with
a usd -> usd_foil -> usd_etched fallback).

## Usage

```bash
mtg-lands rg               # one pair, by letters or guild name (rg / gruul)
mtg-lands bant             # one triple, by letters or shard/wedge (gwu / bant)
mtg-lands --all-pairs      # all 10 guilds
mtg-lands --all-triples    # all 10 shards/wedges
mtg-lands rg --generic     # also expand every any-color (rainbow) land
mtg-lands rg --json        # machine-readable classification
```

A 3-color identity is computed as the union of its three pairs (the 2-color
duals plus rainbow lands) plus a query at the full triple identity (trilands and
anything else that makes all three colors, whose 3-color identity the pair
queries exclude).

## How cycles are detected

Cycles are color-agnostic structural patterns, so one taxonomy covers all 10
pairs and all 10 triples. Examples:

- Fast land: `enters tapped unless you control two or fewer other lands`
- Check land: `enters tapped unless you control a <basic type>`
- Shock: two basic land types + `pay 2 life`
- Filter: a `{a/b}` hybrid filter ability, or the old `{1},{T}: add {a}{b}`
- True dual: two basic land types and no drawback text at all

Validation: running `--all-pairs` yields exactly 10 true duals, 10 shocks, 10
checks, 10 fasts, 10 pathways, 10 bonds, etc. - one complete cycle per guild.
The only fall-throughs are genuine one-off lands (River of Tears, Mount Doom,
Riftstone Portal) with no cycle.

## Requirements

- The `scry` binary on PATH (or set `SCRY_BIN` to its path).
- Python 3 (standard library only).

The script self-throttles to stay under Scryfall's 10 requests/second limit, so
batch runs (`--all-pairs`, `--all-triples`) are safe.

## Reports

Pre-generated reports for all pairs and triples live in `reports/`
(`all-pairs.md`, `all-triples.md`, `all-pairs.json`). Regenerate them, or the
`all-triples.json` variant, with the commands above. Space batch runs out so you
do not trip Scryfall's rate limit.
