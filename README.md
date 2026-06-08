# mtg-lands

Classify the dual / fixing lands for any Magic color identity.

`mtg-lands` is a standalone script that wraps the
[`scry`](https://github.com/mathdroid/scry) CLI. For a color identity it pulls
every Commander-legal land that fits the identity and can make the relevant
colors, then for each land works out three things from color-agnostic
oracle-text patterns: how it enters, its cycle, and its tags.

Full generated reports live in [`reports/`](reports/):
[all pairs](reports/all-pairs.md) and [all triples](reports/all-triples.md).

## Grouping (no tiers)

Lands are grouped by **how they enter the battlefield** - there are no quality
tiers. Three groups:

- **Enters untapped** - never enters tapped (true duals, pain, filter, verge,
  the original/ABUR duals, ...).
- **Conditional** - enters tapped unless a condition is met (shock, check,
  fast, slow, battle/tango, bond, reveal, catch-up).
- **Enters tapped** - always tapped (temples, surveil lands, gates, trilands,
  bounce, gain, cycling, snow, ...).

Each land also carries:

- a **cycle** - a descriptive name (true dual, shock, verge, ...), or `-` when
  it matches no known cycle (catch-all taplands and genuine one-offs).
- **tags** - cross-cutting attributes: `searchable` (has basic land types, so a
  fetchland can find it), `filter`, `pain`, `snow`, `manland`, `cycling`,
  `mdfc`, `lifegain`, `any-color`.

Within each group, cards are ordered by a popularity+price score: the average of
two percentiles across the result set, EDHREC rank (more played = higher) and
USD price (more expensive = higher, with a usd -> usd_foil -> usd_etched
fallback). Reserved List duals often have no nonfoil price; they show `RL` and
the score falls back to popularity rather than treating them as $0.

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

`reports/` holds two kinds of file:

- **Data** (`all-pairs.json`, `all-triples.json`) - the classification straight
  from `mtg-lands --all-pairs --json` / `--all-triples --json`. This is the
  source of truth. Regenerate with the commands above (space batch runs out so
  you do not trip Scryfall's rate limit).
- **Reports** (`all-pairs.md`, `all-triples.md`) - readable markdown that reads
  the JSON as its source. Each guild gets three tables (enters untapped /
  conditional / enters tapped), with columns Cycle, Card, Tags, EDHREC, Price.
  The triples report shows the trilands and true duals that are new at three
  colors and points back to the pair sections for the rest.

The `scry` CLI it wraps backs off and retries on a Scryfall 429 internally, so
the data regeneration is resilient to brief rate limiting.

## Claude Code skill

`skill/SKILL.md` teaches Claude Code when and how to use `mtg-lands`. Install it
by symlinking into your skills directory:

```bash
ln -sfn "$PWD/skill" ~/.claude/skills/mtg-lands
```
