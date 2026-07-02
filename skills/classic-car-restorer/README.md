# Classic Car Restorer

**English** | [日本語](./README.ja.md)

An AI skill for classic and vintage vehicles — points ignition, carburetors, rust assessment, obsolete parts sourcing, and the judgment calls of restoration versus preservation.

## Description

The Classic Car Restorer covers the technology that predates OBD ports and the decisions that don't exist with modern cars: how to tune points and condensers, rebuild and jet carburetors, judge whether rust is cosmetic or structural, hunt down parts that haven't been made in decades, and decide what level of restoration a car deserves — concours-correct, sympathetic preservation, or restomod. It also covers the realities of running a classic: storage, fuel compatibility, and keeping a 50-year-old car safe in modern traffic.

**Audience:** First-time classic buyers, restorers at any stage of a project, and owners keeping an older vehicle on the road.

## Capabilities

- **Ignition** — points/condenser theory, gap and dwell setting, timing with a strobe light, coil and ballast resistor testing, when and how to convert to electronic ignition (and what originality it costs)
- **Carburetion** — how carburetors meter fuel, rebuild walkthroughs, jetting and mixture tuning by plug reading, multiple-carb synchronization, ethanol-fuel compatibility problems and fuel system material upgrades
- **Rust and body** — distinguishing surface rust, scale, and perforation; structural areas that fail inspection or endanger safety (chassis rails, suspension mounts, sills); assessment before purchase; treatment options from converters to cut-and-weld
- **Electrics** — dynamo/generator vs. alternator, positive-ground systems, cloth wiring hazards, adding discreet modern protection (relays, fuses, cutoff switches)
- **Mechanical** — drum brake service and adjustment, kingpins and grease points, non-synchro gearbox technique, engine break-in after rebuild
- **Parts sourcing** — NOS vs. reproduction vs. used, interchange research, judging reproduction quality, clubs and marque specialists as resources, having parts remade (casting, machining) as a last resort
- **Strategy** — restoration triage and sequencing (mechanical before cosmetic), budgeting honestly, originality vs. usability tradeoffs, documentation for provenance and value
- **Ownership** — long-term storage, recommissioning after storage, ethanol-era fuel choices, insurance (agreed value) and historic registration concepts

## Example Prompts

```text
I'm looking at a 1972 MGB with "some rust in the sills." How do I tell
whether this is cosmetic or a structural deal-breaker before buying?
```

```text
Walk me through setting points gap and ignition timing from scratch on a
1968 Ford with a V8. I have feeler gauges and a timing light.
```

```text
My rebuilt carburetor runs rich at idle but leans out at speed. How do I
read the spark plugs and which circuit do I adjust?
```

```text
The car will be stored for 8 months over winter. Give me a proper
storage checklist and a recommissioning checklist for spring.
```

```text
Brake parts for my 1965 Prince Skyline are unobtainable. What are my
options, from interchange research to having parts remade?
```

## Recommended Workflow

1. **Identify the vehicle and its state.** Year, make, model, engine, how original it is, whether it runs, and how long it has been off the road.
2. **State your goal.** Concours restoration, reliable driver, sympathetic preservation, or restomod — advice differs radically between them.
3. **Assess before disassembling.** Ask for an assessment checklist first; cars come apart much faster than they go back together.
4. **Work in the right order.** Get a sequencing plan: safety systems and structure first, drivetrain second, cosmetics last.
5. **Document everything.** Photograph before disassembly, bag and label fasteners, keep receipts — the assistant can help you build a documentation habit.
6. **Verify old specs carefully.** Period manuals contain errors and units differ (BSF/Whitworth, positive ground); cross-check values against marque club knowledge.

## Limitations

- **Marque-specific knowledge has limits.** Production changes, factory quirks, and known fixes for specific classics live in owners' clubs and marque forums — the assistant complements them, not replaces them.
- **Cannot judge rust or metal condition remotely.** Descriptions and photos help, but a magnet, a pick, and an inspection lift are the real tools.
- **Structural welding, brake hydraulics, and steering on old cars are safety-critical** — have this work done or inspected by professionals; classic cars lack every modern crash protection.
- **Value and originality judgments are subjective and market-dependent** — for significant cars, consult marque experts and appraisers before irreversible changes.
- **Period specifications may be in obsolete units or standards** (Whitworth fasteners, degrees dwell) — conversion errors are a real risk; verify twice.

## Related Skills

- [Mechanic Assistant](../mechanic-assistant/) — modern-vehicle repairs and shared fundamentals
- [Used Car Inspector](../used-car-inspector/) — purchase inspection methods, adapted here for classics
- [Vehicle Customization Advisor](../vehicle-customization-advisor/) — restomod planning shares its build-order discipline
