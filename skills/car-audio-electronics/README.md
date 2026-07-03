# Car Audio & Electronics Assistant

**English** | [日本語](./README.ja.md)

An AI skill for aftermarket audio and 12V electronics — head unit replacement, speaker and amplifier installs, dash cams and accessory wiring, power and grounding done right, and knowing where modern CAN-bus vehicles say no.

## Description

Twelve-volt work is the most common gateway into DIY — and the most common source of parasitic drains, blown amplifiers, and mysteriously angry vehicle electronics. This skill covers planning and executing audio upgrades (head units, speakers, amps, subs, sound deadening), wiring accessories properly (dash cams, radar detectors, lighting, inverters), and the discipline of power, ground, and fusing that separates clean installs from fire hazards. It is explicit about the modern complication: on CAN-bus vehicles, the days of freely tapping wires are over.

**Audience:** First-time head unit swappers through multi-amp system builders, plus anyone hardwiring a dash cam.

## Capabilities

- **Head units** — sizing (single/double DIN, floating displays), vehicle-specific harness adapters and why you never cut factory plugs, steering wheel control interfaces, retained accessory power, antenna and reversing camera adapters, factory-amp bypass or integration
- **Speakers** — component vs. coaxial, sensitivity and power matching, baffle and depth checks, why door speakers need sound deadening to perform, high-level vs. RCA inputs
- **Amplifiers & subwoofers** — gain setting properly (it is not a volume knob), power wire gauge and fusing within 30 cm of the battery, ground point quality, RCA routing away from power, enclosure types (sealed vs. ported) and their honest tradeoffs, DSP basics
- **Accessory wiring** — dash cams and hardwire kits (add-a-fuse on the right circuit type: ignition-switched vs. constant), parking-mode drain math and low-voltage cutoffs, radar detectors, USB and inverter loads, LED retrofits and load resistors
- **Electrical discipline** — calculating current draw, choosing wire gauge, every positive wire fused at the source, grounding to bare metal, relay usage for high loads, avoiding ground loops (alternator whine diagnosis)
- **CAN-bus awareness** — why probing and tapping unknown wires on modern vehicles can trigger faults or damage modules, using interface modules instead, which circuits are still safe to touch, and when the answer is "dealer-level integration or don't"
- **Troubleshooting** — alternator whine, turn-on pops, parasitic drain hunting after an install, blown fuse forensics
- **Security & convenience** — basic alarm/immobilizer awareness, keyless entry retrofits (with the explicit boundary that anti-theft *bypass* is out of scope)

## Example Prompts

```text
Replacing the factory head unit in a 2016 Mazda 3 with a wireless CarPlay
unit. What adapters do I need so steering wheel controls and the factory
camera keep working?
```

```text
Plan the wiring for a 600W RMS amp and sub: wire gauge, fuse size and
location, ground point, and where the RCA cables should run.
```

```text
I hardwired a dash cam and now the battery dies after 4 days parked.
Walk me through finding and fixing the drain.
```

```text
My new amp has an adjustable gain, bass boost, and a filter switch.
Give me the correct setup procedure that doesn't rely on guessing.
```

```text
I want brighter interior and reverse lights on a 2020 vehicle. What can
I safely change myself, and where does CAN-bus make this complicated?
```

## Recommended Workflow

1. **Identify the vehicle and its electronics level.** Year, make, model, trim, factory amp/screen presence — this determines adapter needs and CAN constraints before anything else.
2. **State the goal and budget honestly.** "Clearer sound at normal volume" and "competition bass" are different builds; the skill will size components and wiring to the goal.
3. **Plan power first.** Total current draw, wire gauge, fusing, and ground points get decided before any parts order.
4. **Install in test stages.** Bench-test or partially connect before final assembly; verify no warning lights and correct function at each stage.
5. **After install:** measure parasitic drain (should typically be under ~50 mA after modules sleep) and re-check fuses seated and rated correctly.
6. **Document the wiring** — future you, the next owner, and the next troubleshooting session all need to know what was tapped where.

## Limitations

- **Vehicle-specific wiring must be verified.** Wire colors and circuit functions vary by market and trim; always confirm with a multimeter and vehicle-specific documentation rather than trusting generic color charts.
- **CAN-bus and module-level integration has hard limits** — some functions (factory screens, digital amps, virtual cockpits) integrate only via dedicated interface hardware or not at all; the skill says so rather than pretending.
- **Anti-theft systems are a boundary.** The skill covers adding security, not bypassing immobilizers, defeating alarms, or key cloning — such requests are declined.
- **Airbag (SRS) wiring is untouchable.** Yellow connectors and harnesses are off-limits; work near them (dash disassembly) follows battery-disconnect and wait-time rules.
- **Sound quality judgments are subjective and room-dependent** — the skill optimizes the engineering; final tuning is your ears' job.
- **High-power systems interact with the charging system** — big amp installs may need alternator and battery consideration the skill will flag but a specialist should size.

## Related Skills

- [Vehicle Customization Advisor](../vehicle-customization-advisor/) — audio as part of a broader build plan
- [Vehicle Troubleshooting](../vehicle-troubleshooting/) — electrical symptom diagnosis beyond the install itself
- [Mechanic Assistant](../mechanic-assistant/) — interior disassembly and reassembly technique
