# Diesel Specialist

**English** | [日本語](./README.ja.md)

An AI skill for modern and older diesel engines — common rail systems, emissions aftertreatment (DPF/EGR/SCR), glow plugs, turbochargers, and diesel-specific diagnosis and maintenance.

## Description

The Diesel Specialist covers what gasoline-engine experience doesn't: high-pressure common rail fuel systems, diesel particulate filter regeneration, AdBlue/DEF systems, and the failure patterns unique to compression ignition. It helps diagnose hard starts, smoke, power loss, and emissions warnings, and builds maintenance habits that prevent the expensive failures diesels are known for — clogged DPFs, worn injectors, and EGR-choked intakes.

**Audience:** Diesel car, truck, and van owners; technicians expanding from gasoline work; fleet operators running diesel vehicles.

## Capabilities

- **Fuel system** — common rail principles and pressures, injector failure symptoms (knock, hard start, smoke, imbalance readings), lift pump vs. high-pressure pump diagnosis, fuel contamination response (water, wrong fuel, bacterial growth), filter service intervals and priming procedures
- **Aftertreatment** — DPF operation, passive vs. active vs. forced regeneration, causes of failed regens and clogging (short trips, wrong oil, upstream faults), EGR fouling symptoms and cleaning options, SCR/AdBlue (DEF) systems: consumption rates, crystallization, quality warnings and countdown limits
- **Cold starting** — glow plug testing and replacement, intake heaters, winter fuel (gelling, cloud point, anti-gel additives), battery and cranking-speed demands of diesel compression
- **Turbochargers** — variable geometry (VGT/VNT) sticking, boost leak diagnosis, oil feed problems, overboost/underboost codes
- **Diagnosis** — white/blue/black smoke interpretation, excessive fuel consumption, limp mode triggers, diesel runaway awareness and response
- **Maintenance** — oil specifications matter more on diesels (low-SAPS for DPF-equipped engines), timing belt/chain intervals, valve adjustments on older engines, coolant and injector seal considerations
- **Ownership decisions** — whether a diesel fits the owner's driving pattern (short-trip DPF risk), used diesel inspection points, and typical high-mileage cost curves

## Example Prompts

```text
My 2016 VW Golf TDI shows the DPF warning light and I mostly drive short
city trips. What's happening and what are my options before it needs a
forced regeneration?
```

```text
Diesel hard-starts only on cold mornings, cranks fine, lots of white smoke
until it warms up. 2012 Isuzu D-Max. Where do I start?
```

```text
The AdBlue warning says 1,000 km until no-restart. Refilling didn't clear
it. What does that mean and what should I check?
```

```text
I accidentally put 10 liters of gasoline in my diesel tank, then topped up
with diesel. Tank is now about 15% gasoline. Drive it or drain it?
```

```text
What maintenance schedule differences should I follow for a diesel van
used for daily deliveries versus the gasoline schedule I'm used to?
```

## Recommended Workflow

1. **Identify the engine and emissions equipment.** Year, make, model, engine code if known, and whether it has DPF/EGR/SCR (roughly: DPF standard from ~2009 in the EU, AdBlue common from ~2015).
2. **Describe the driving pattern.** Short trips vs. highway is the single biggest factor in diesel aftertreatment health.
3. **Report warnings precisely.** DPF, AdBlue, and emissions warnings escalate in stages — note exactly which message or light, and any countdown.
4. **Share live data when possible.** DPF soot load, differential pressure, and rail pressure readings sharply narrow diagnosis.
5. **Act before escalation.** Many diesel systems (DPF overfill, AdBlue countdown) pass a point where DIY options end and forced dealer intervention begins — ask "how long do I have?"
6. **Verify fixes with a regen or drive cycle** and confirm the relevant readings return to normal.

## Limitations

- **Emissions system removal or defeat is off-limits.** DPF/EGR/AdBlue deletes are illegal for road use in most jurisdictions; this skill explains, diagnoses, and repairs these systems but will not advise on removing them.
- **High-pressure fuel systems are dangerous.** Common rail pressures can exceed 2,000 bar — never crack a live injector line; injuries from injection events are severe. Testing procedures that involve pressurized components belong to equipped professionals.
- **Forced regeneration and injector coding typically require dealer-level scan tools** — the skill tells you when you've reached that boundary.
- **Specifications vary widely** (oil specs, DPF thresholds, AdBlue logic) by manufacturer and market; verify against factory documentation.
- **Older mechanical-injection diesels** (rotary/inline pumps) are covered conceptually, but pump rebuilds are specialist work.

## Related Skills

- [Mechanic Assistant](../mechanic-assistant/) — general repair procedures shared with gasoline vehicles
- [OBD-II Diagnostic Assistant](../obd2-diagnostic-assistant/) — diesel DTCs and live data interpretation
- [Fleet Manager](../fleet-manager/) — managing diesel maintenance across multiple vehicles
