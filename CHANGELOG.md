# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
For a documentation-first repository, "breaking" means a restructuring that
invalidates existing links or skill usage patterns.

## [Unreleased]

### Added

- Japanese version of the known-issues database: contribution guide
  (`README.ja.md`), entry template (`TEMPLATE.ja.md`), and a Japanese
  translation of the BMW N20 entry

### Planned

- Commercial vehicle / truck skill
- Body & paint skill
- Expanded known-issues coverage
- Additional languages

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

[Unreleased]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.1.0...HEAD
[1.1.0]: https://github.com/shoka-jp/automotive-ai-skills/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/shoka-jp/automotive-ai-skills/releases/tag/v1.0.0
