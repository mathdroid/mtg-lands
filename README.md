# mtg-lands

Classify and rank the dual / fixing lands for any Magic color identity.

`mtg-lands` is a standalone script that wraps the
[`scry`](https://github.com/mathdroid/scry) CLI. For a color identity it pulls
every Commander-legal land that fits the identity and can make the relevant
colors, then records each land's entry status (untapped / conditional /
tapped), cycle, and tags. Output is three tables per identity, one per entry
status.

Full reports live in [`reports/`](reports/):
[all pairs](reports/all-pairs.md) and [all triples](reports/all-triples.md).

## Best fixing per guild

The unconditional true dual, the best-scoring conditional land, and the
most-played conditional land per guild.

| Guild | True dual | Best conditional | Most-played conditional |
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

## Model

Each identity-specific land gets three things:

- **Entry status**, read straight from the oracle text:
  - `untapped` - always enters untapped (true duals, painlands, filters, verges,
    horizon lands, Tainted, storage / depletion / locked lands).
  - `conditional` - untapped only if a condition is met, else tapped (shock,
    check, fast, slow, battle, bond, reveal, catch-up).
  - `tapped` - always enters tapped (Temples, surveil lands, bounce, gain,
    cycling, snow, creature lands, Campus, Bridge, Guildgate, plain taplands).
- **Cycle** - the recognized land cycle, or `-` if it is a one-off / not a named
  cycle. Named cycles (Verge, Tainted, Campus, Bridge, Pathway, Guildgate,
  Triome, the Theros Temples) are matched by card name to avoid sweeping in
  look-alikes (Nimbus Maze is not a Verge).
- **Tags** - orthogonal properties: `searchable` (has basic land types, so it is
  fetchable), `filter`, `pain`, `lifegain`, `manland`, `MDFC`, `cycling`,
  `snow`, `scry`, `surveil`, `bounce`, `storage`.

The reports present each identity as three tables (untapped / conditional /
tapped). Rows are ordered by a popularity+price score: the average of two
percentiles across the result set, EDHREC rank (more played = higher) and USD
price (more expensive = higher, with a usd -> usd_foil -> usd_etched fallback;
Reserved List duals with no price fall back to play rate).

Any-color (rainbow) lands tap for any color, recur in every identity, and are
listed once at the end of each report.

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

Named cycles (Verge, Tainted, Campus, Bridge, Pathway, Guildgate, Triome, the
Theros Temples) are matched by card name, which is reliable and avoids
over-matching look-alikes. The rest are color-agnostic structural patterns:

- Fast land: `enters tapped unless you control two or fewer other lands`
- Check land: `enters tapped unless you control a <basic type>`
- Shock: two basic land types + `pay 2 life`
- Filter: a `{a/b}` hybrid filter ability, or the old `{1},{T}: add {a}{b}`
- True dual: two basic land types and no drawback text at all

Validation: running `--all-pairs` yields clean per-guild counts (10 true duals,
10 shocks, 10 checks, 10 fasts, 10 verges, 10 surveil lands, 10 Temples, ...).
The only fall-throughs (cycle `-`) are genuine one-off lands: Nimbus Maze, River
of Tears, Mount Doom, Riftstone Portal.

## Requirements

- The `scry` binary on PATH (or set `SCRY_BIN` to its path).
- Python 3 (standard library only).

The script self-throttles to stay under Scryfall's 10 requests/second limit, so
batch runs (`--all-pairs`, `--all-triples`) are safe.

## Reports

`reports/` holds two kinds of file:

- **Data** (`all-pairs.json`, `all-triples.json`) - the raw classification
  straight from `mtg-lands --all-pairs --json` / `--all-triples --json`. This is
  the source of truth. Regenerate with the commands above (space batch runs out
  so you do not trip Scryfall's rate limit).
- **Reports** (`all-pairs.md`, `all-triples.md`) - markdown built from the JSON:
  per identity, three tables (untapped / conditional / tapped) with Cycle, Card,
  and Tags columns, plus a shared any-color section. Refresh them when the data
  changes.

The `scry` CLI it wraps backs off and retries on a Scryfall 429 internally, so
the data regeneration is resilient to brief rate limiting.
