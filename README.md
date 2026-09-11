# Delightful's Game Research Starter Pack — data

A directory of the press, institutions, datasets, media, people and communities behind the video games industry across **ten markets**, plus the trends, platforms and genres that frame them.

**914 sources. 10 markets. 37 trends. 35 platforms. 30 genres.** Every source was opened and read before its description was written.

The site is at **https://games.thisisdelightful.com** — this repository is the data behind it, in the same files the site offers for download.

Directory last compiled 11 September 2026.

## Licence

**Creative Commons Attribution 4.0 International** — [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

Use it, change it, publish from it, including commercially. Crediting the source is the one condition.

The licence covers the data in these files. It does not cover the material the rows point at: the reporting, artwork, figures and writing behind every link belong to whoever published them.

### Citing it

> Delightful's Game Research Starter Pack, CC BY 4.0. https://games.thisisdelightful.com

## What is and is not checked

Read this before building on the data. It is the same warning the site leads with.

- **Every source was opened and read** before its description was written.
- **What a source claims is not checked.** A number reached through this data carries the authority of the outlet that published it and no more.
- **Nothing here is scored or ranked.** Row order is not a judgement.
- **Market-size figures are NOT comparable across markets.** Ten markets publish on ten different bases, in different years, against different definitions of a player. Putting them in one chart produces a chart that means nothing.
- **The industry has no shared genre taxonomy.** Two datasets that appear to describe the same thing often do not. The genres here are the labels platforms use, not a scheme imposed over them.

## The files

CSV is UTF-8, RFC 4180, one row per thing. A cell holding several plain tokens joins them with `; `. Where a row carries a list of other things, that list is its own file. **An empty cell means the field was not collected for that kind of row, not that the answer is nothing.**

There is no ID column. Rows are identified by name, and row order is export order, which is not a ranking of anything by anyone.

| File | Rows | What it is |
|---|---|---|
| [`data/sources.csv`](data/sources.csv) | 914 | Every source in the directory: outlet, institution, dataset, podcast, book, person or community, with what it lets you find out, who owns it, what it costs, which markets it covers and what to watch for. |
| [`data/sources.json`](data/sources.json) | 914 | The same rows, as JSON. |
| [`data/markets.json`](data/markets.json) | 10 | Per-market claims and population figures, nested. Every claim carries the source and link it came from; every population figure carries the definition saying who was counted. |
| [`data/trends.csv`](data/trends.csv) | 37 | The trends currently moving the industry, with stage, category and the markets each lands in. |
| [`data/trend-reading.csv`](data/trend-reading.csv) | 110 | The further reading attached to each trend. One row per link. |
| [`data/trends.json`](data/trends.json) | 37 | Trends with their reading attached. |
| [`data/platforms.csv`](data/platforms.csv) | 35 | Storefronts, consoles, livestreaming and UGC platforms, with who owns each. |
| [`data/genres.csv`](data/genres.csv) | 30 | Genre definitions, local-language terms and subgenres. |
| [`data/example-games.csv`](data/example-games.csv) | 90 | The games named as examples of each genre. |
| [`data/landscape.json`](data/landscape.json) | — | Platforms and genres with their example games. |
| [`data/searching-tips.csv`](data/searching-tips.csv) | 39 | Search techniques, each with a query you can paste and the markets it applies to. |
| [`data/searching-tips.json`](data/searching-tips.json) | 39 | The same rows, as JSON. |
| [`data/vocabulary.csv`](data/vocabulary.csv) | 211 | Every value each filter can take, and how many rows carry it. **Read this before building on the data** — it is the coverage record, and it says where the directory is thin. |
| [`data/vocab.json`](data/vocab.json) | — | The same counts, nested by facet. |
| [`games-research-starter-pack.xlsx`](games-research-starter-pack.xlsx) | — | Every table as one workbook, a sheet each, filters already on. |

## Markets covered

Canada · China · France · Germany · Italy · Japan · South Korea · MENA · United Kingdom · United States

Brazil and India are next. Nine further markets — Australia, Spain, Mexico, Netherlands, Poland, Turkey, Taiwan and others — have source rows but no full profile yet; `vocabulary.csv` gives the counts.

## Using it with a language model

The files are small enough to hand to a model directly, and `sources.csv` is the one to start with. Two things worth putting in the prompt:

- **Ask it to quote rows rather than summarise them.** A model handed 914 rows in a chat window starts summarising, and summarising is where invented rows come from.
- **Tell it not to compare market-size figures.** See the warning above; it is the mistake this data makes easiest.

The site's [data and download page](https://games.thisisdelightful.com/doc/data-and-download) carries a field-by-field dictionary and several ready-made prompts.

## How it was made

[Method](https://games.thisisdelightful.com/doc/method) — who it is for, where it came from, how it was assembled, what was checked and what was not, including the two problems found in the underlying data.

## Corrections

Corrections are wanted, including ones arguing that a source does not belong here or that an outlet, person or community is missing. **games@thisisdelightful.com** — say which row and what is wrong with it. Corrections are made in the workbook and published on the next pass rather than patched in place, so these files and the site change together.

---

*This README is generated by `scripts/build-mirror.mjs` in the site repository. Every count in it is read from the export manifest rather than typed, so it describes the files it ships beside.*
