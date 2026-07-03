# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
For a documentation-first repository, "breaking" means a restructuring that
invalidates existing links or skill usage patterns.

## [Unreleased]

### Added

- Known-issue entries (EN+JA): Nissan/Jatco CVT premature failure
  (`nissan-jatco-cvt-failure`), Toyota ZVW30 Prius EGR clogging and head
  gasket failure (`toyota-zvw30-prius-egr-head-gasket`)

### Planned

- Complete Spanish coverage of all skills
- Motorhome/RV habitation systems skill
- Welding & fabrication basics skill

## [1.4.0] - 2026-07-03

### Added

- **Claude Code native support**: `SKILL.md` in every skill folder and a
  plugin marketplace definition (`.claude-plugin/`) — install with
  `/plugin marketplace add shoka-jp/automotive-ai-skills` followed by
  `/plugin install automotive-ai-skills@automotive-ai-skills`
- **OpenAI Codex support**: repository-level `AGENTS.md` (auto-loaded by
  Codex, routes questions to skills and enforces safety rules) and a
  Codex guide (`integrations/codex.md`) covering in-repo, global, and
  per-skill custom prompt setups
- Skill Authoring Guide now documents the `SKILL.md` requirement

- GitHub Pages documentation site with SEO metadata (`_config.yml` with
  jekyll-seo-tag and jekyll-sitemap), `robots.txt`, and an `llms.txt`
  index for AI/LLM crawlers (generative engine optimization)
- Custom site design in a factory-service-manual visual language
  (spec-plate hero, 16-section skill index, shared docs layout)
- Language auto-routing: browser-language redirect on the landing page
  (ja/es, loop-safe) and automatic `hreflang` alternates across all
  translated page pairs for search-level language targeting

## [1.3.0] - 2026-07-03

### Added

- **2 new skills** (English + Japanese): Towing & Trailer Advisor,
  Car Audio & Electronics Assistant — 16 skills total
- **Spanish skill translations** for 4 core skills: Mechanic Assistant,
  OBD-II Diagnostic Assistant, Vehicle Maintenance Planner, Used Car
  Inspector (`README.es.md`; registered in each `skill.yaml`)
- **Machine-readable known-issues index** (`data/known-issues/index.yaml`)
  with make/platform/years/severity/tags metadata per entry

### Changed

- Garage Assistant combined system prompt routes to the two new skills
- Known-issues contribution flow now includes updating `index.yaml`

## [1.2.0] - 2026-07-03

### Added

- **2 new skills** (English + Japanese): Commercial Vehicle & Truck
  Assistant, Body & Paint Assistant — 14 skills total
- **3 new known-issue entries**, all bilingual: Toyota 2AZ-FE oil
  consumption, Subaru EJ25 head gasket leaks, Honda i-DCD DCT judder
- Japanese version of the known-issues database: contribution guide
  (`README.ja.md`), entry template (`TEMPLATE.ja.md`), and a Japanese
  translation of the BMW N20 entry
- **Spanish README** (`README.es.md`) — first step toward additional
  languages; skill-content translation marked community-driven

### Changed

- Garage Assistant combined system prompt routes to the two new skills

## [1.1.0] - 2026-07-03

### Added

- **4 new skills** (English + Japanese): Diesel Specialist, Classic Car
  Restorer, Fleet Manager, Tire & Wheel Advisor — 12 skills total
- Machine-readable `skill.yaml` definitions in every skill folder, with
  schema documented in the Skill Authoring Guide
- Japanese translations of all three example conversations (`*.ja.md`)
- Community known-issues database (`data/known-issues/`) with template
  and first entry (BMW N20 timing chain)
- Integrations folder: Claude Project single-skill template and a
  combined "Garage Assistant" system prompt
- Issue templates (inaccuracy/safety report, new skill proposal) and a
  pull request template with the contribution checklist

### Changed

- Skill Authoring Guide now requires `skill.yaml` and a Japanese README
  for new skills

## [1.0.0] - 2026-07-03

### Added

- Initial release with 8 skills:
  - Mechanic Assistant
  - OBD-II Diagnostic Assistant
  - Vehicle Maintenance Planner
  - Used Car Inspector
  - Vehicle Troubleshooting
  - Vehicle Customization Advisor
  - EV Assistant
  - Motorcycle Mechanic
- Skills index with a "Which skill do I need?" selection guide
- Project documentation: README (English and Japanese), CONTRIBUTING,
  CODE_OF_CONDUCT (Contributor Covenant 2.1), SECURITY, safety disclaimer
- Guides: getting started, skill authoring guide, FAQ
- Example conversations: P0420 diagnosis, used car inspection,
  maintenance catch-up plan
- Japanese translations of all 8 skills (`README.ja.md` in each skill folder)
- Japan-specific guides in `docs/ja/`: pre-shaken (vehicle inspection)
  self-check checklist and a Japan market guide with terminology glossary
- MIT license

[Unreleased]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.4.0...HEAD
[1.4.0]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/shoka-jp/automotive-ai-skills/releases/tag/v1.0.0
