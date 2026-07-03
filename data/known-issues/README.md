# Known-Issues Database

**English** | [日本語](./README.ja.md)

A community-contributed collection of **model-specific known issues** — the "everyone in the owners' club knows this" knowledge that makes the skills dramatically more useful for a specific vehicle.

Each entry is one Markdown file describing one issue on one platform (model/generation/engine). Entries are designed to be pasted into an AI session alongside a skill, or read directly by a buyer or owner.

## How to use these entries

1. Find entries matching your vehicle (file names are `<make>-<platform-or-model>-<issue>.md`).
2. Paste the relevant entries into your AI conversation along with your question — e.g., combine with the [Used Car Inspector](../../skills/used-car-inspector/) before a viewing.
3. Treat entries as **leads to verify**, not verdicts: production changes and regional differences mean your exact vehicle may differ.

## Contributing an entry

Copy [`TEMPLATE.md`](./TEMPLATE.md), fill in every section, and open a PR. Requirements:

- **One issue per file.** Split multi-issue write-ups.
- **Scope precisely.** Years, engine codes, and markets. "BMW timing chains" is too broad; "N20 engines built before ~2015" is right.
- **Describe symptoms observably.** What an owner can hear, see, or measure — not just the failed part.
- **Be honest about frequency.** "Known failure point" and "every single one fails" are different claims; do not exaggerate.
- **State the fix and realistic cost range**, marking the currency and region your estimate comes from.
- **Note your sources** in general terms (owner communities, TSB numbers, personal shop experience). No copyrighted text dumps.
- Entries about **defeating emissions or safety systems are not accepted** (see [CONTRIBUTING.md](../../CONTRIBUTING.md)).

Japanese-language entries are welcome — use [`TEMPLATE.ja.md`](./TEMPLATE.ja.md) and a `.ja.md` suffix. Entries for Japan-market vehicles (kei cars, JDM-only models) are especially valuable.

## Current entries

| Entry | Vehicle scope | Severity | 日本語 |
|---|---|---|---|
| [bmw-n20-timing-chain.md](./bmw-n20-timing-chain.md) | BMW N20/N26 2.0T (2011–2015-ish production) | Critical | [あり](./bmw-n20-timing-chain.ja.md) |
| [toyota-2az-fe-oil-consumption.md](./toyota-2az-fe-oil-consumption.md) | Toyota 2AZ-FE 2.4L (~2006–2011) | Major | [あり](./toyota-2az-fe-oil-consumption.ja.md) |
| [subaru-ej25-head-gasket.md](./subaru-ej25-head-gasket.md) | Subaru SOHC EJ25 (~1999–2011) | Major | [あり](./subaru-ej25-head-gasket.ja.md) |
| [honda-idcd-dct-judder.md](./honda-idcd-dct-judder.md) | Honda i-DCD hybrids (2013–2015 focus) | Major | [あり](./honda-idcd-dct-judder.ja.md) |
| [nissan-jatco-cvt-failure.md](./nissan-jatco-cvt-failure.md) | Nissan/Jatco CVTs (~2003–2018, worst 2003–2010 & 2013–2016) | Major | [あり](./nissan-jatco-cvt-failure.ja.md) |
| [toyota-zvw30-prius-egr-head-gasket.md](./toyota-zvw30-prius-egr-head-gasket.md) | Toyota Prius ZVW30 / 2ZR-FXE (2009–2015) | Major | [あり](./toyota-zvw30-prius-egr-head-gasket.ja.md) |
| [mazda-fd3s-13b-rew-compression-loss.md](./mazda-fd3s-13b-rew-compression-loss.md) | Mazda RX-7 FD3S / 13B-REW (1991–2002, all years) | Major | [あり](./mazda-fd3s-13b-rew-compression-loss.ja.md) |
| [subaru-ej20t-ringland-bearing.md](./subaru-ej20t-ringland-bearing.md) | Subaru EJ turbo WRX/STI (GC8/GDB/GRB, EJ255/257) | Major | [あり](./subaru-ej20t-ringland-bearing.ja.md) |

*(This index is maintained by hand — add your entry to the table in the same PR.)*

## Machine-readable index

[`index.yaml`](./index.yaml) mirrors the table above with structured metadata (make, platform, years, severity, tags, file paths per language) for programmatic consumption — e.g., filtering entries for a specific vehicle before injecting them into an AI session. When contributing an entry, add it to `index.yaml` in the same PR.
