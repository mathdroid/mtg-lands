---
name: mtg-lands
description: List and classify the dual / fixing lands available to a Magic color identity, using the `mtg-lands` CLI. Use when the user asks what lands to run in a color pair or commander identity, wants the fixing lands for a guild / shard / wedge (e.g. "Gruul lands", "what duals are in Jund", "rg fixing"), or wants lands grouped by how they enter (untapped / tapped) or by cycle (shock, fastland, fetchable dual, ...).
---

# mtg-lands

`mtg-lands` is a CLI at `~/.local/bin/mtg-lands` (or `~/bin/mtg-lands`) that
wraps [`scry`](../scry) to list every Commander-legal fixing land for a color
identity and classify each one.

## Usage

```bash
mtg-lands rg               # one pair: letters or guild name (rg / gruul)
mtg-lands bant             # one triple: letters or shard/wedge (gwu / bant)
mtg-lands --all-pairs      # all 10 guilds
mtg-lands --all-triples    # all 10 shards/wedges
mtg-lands rg --generic     # also expand the any-color (rainbow) lands
mtg-lands rg --json        # machine-readable: entry, cycle, tags, score, edhrec, price
```

It needs the `scry` binary on PATH (or `SCRY_BIN` set).

## What it reports

Each identity is split into three tables by how the land enters play, read from
the oracle text:

- **Enters untapped** - true duals, pain, filter, verge, horizon, Tainted, ...
- **Conditional** - untapped only if a condition is met (shock, check, fast,
  slow, battle, bond, reveal, catch-up).
- **Enters tapped** - temples, surveil lands, bounce, gain, cycling, snow,
  creature lands, Campus, Bridge, Guildgate, plain taplands.

Each land also has a **cycle** (the named cycle, or `-` for a one-off) and
**tags**: `searchable` (has basic land types, so a fetchland can find it),
`filter`, `pain`, `lifegain`, `manland`, `MDFC`, `cycling`, `snow`, `scry`,
`surveil`, `bounce`, `storage`. Rows are ordered by a popularity+price score.

Any-color (rainbow) lands tap for any color and recur in every identity, so they
are listed once at the end (or expand with `--generic`).

## Tips

- For deck-building "what are my best lands in <colors>", run `mtg-lands <colors>`
  and read the untapped/conditional tables first.
- Use `--json` when you need to filter or sort programmatically (e.g. only
  `searchable` lands, or only those under a price).
- A triple is the union of its three pairs plus the trilands.
