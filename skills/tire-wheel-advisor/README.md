# Tire & Wheel Advisor

**English** | [日本語](./README.ja.md)

An AI skill dedicated to tires and wheels — sizing and fitment math, seasonal strategy, load and speed ratings, TPMS, wear diagnosis, and storage.

## Description

Tires are the only part of the vehicle touching the road, and the most commonly mis-purchased. The Tire & Wheel Advisor goes deeper than the general skills: full sizing math (diameter, speedometer error, load index), seasonal changeover strategy, reading wear patterns as a diagnostic tool, TPMS behavior after swaps, and matching tire choice to actual driving rather than marketing categories. It covers cars, SUVs, vans, and EVs, with motorcycle-specific guidance delegated to the Motorcycle Mechanic skill.

**Audience:** Anyone buying tires or wheels, seasonal-swap households, and drivers diagnosing wear or vibration issues.

## Capabilities

- **Sizing math** — decode size markings (e.g., 215/55R17 94V), calculate overall diameter changes and speedometer/odometer error for alternative sizes, plus-sizing and minus-sizing (winter downsizing) rules, load index and speed rating requirements vs. the vehicle placard
- **Wheel fitment** — bolt pattern (PCD), center bore and hub-centric rings, offset effects on scrub radius and bearing load, clearance to struts/calipers/fenders, wheel load ratings, lug torque and re-torque practice
- **Selection** — summer vs. all-season vs. winter compounds and when each actually matters, highway vs. all-terrain vs. mud-terrain for SUVs/trucks, EV-specific considerations (load, noise, low rolling resistance, faster wear), run-flat tradeoffs, wet-grip and noise label systems
- **Seasonal strategy** — when to switch (the 7°C rule of thumb), whether a second wheel set pays off, storage (position, temperature, sunlight, age limits)
- **Wear diagnosis** — reading wear patterns (center, shoulders, one-sided, cupping, feathering) as evidence of pressure, alignment, or suspension problems; measuring tread depth and interpreting date codes; repairable vs. non-repairable damage
- **TPMS** — direct vs. indirect systems, behavior after rotations and seasonal swaps, sensor batteries and service kits, relearn procedure types
- **Practice** — rotation patterns (directional, staggered, full-size spare), pressure strategy for load/towing, breaking in new tires, mixing rules (best pair to the rear)

## Example Prompts

```text
My car came with 215/55R17 94V. Can I run 225/50R17? Show the diameter
and speedometer math, and check the load and speed rating requirements.
```

```text
Front tires are worn smooth on the outer shoulders only, rears are even.
What does this pattern tell me and what should I have checked?
```

```text
I drive an EV in a region with snowy winters. Recommend a two-set wheel
strategy: sizes, tire categories, and whether to downsize for winter.
```

```text
After my seasonal wheel swap the TPMS light stayed on. Second set has no
sensors. What are my options, from cheapest to cleanest?
```

```text
Two of my tires are 7 years old with plenty of tread, made in week 30 of
2019. The other two are 2 years old. Replace, rotate, or run them?
```

## Recommended Workflow

1. **Start from the placard, not the tire.** Share the vehicle's door-jamb placard sizes, load index, speed rating, and pressures — the current tires may already be wrong.
2. **Describe the actual driving.** Climate, annual distance, highway vs. city split, towing/loading, and what you care about most (longevity, quiet, grip, price).
3. **For size changes:** ask for the full calculation — diameter delta, speedometer error, load capacity check, and clearance risks — before purchasing.
4. **For wear problems:** measure tread depth at inner/center/outer on each tire and report the numbers; patterns across positions are the diagnosis.
5. **Confirm the install details.** Torque spec and re-torque after ~50–100 km, TPMS relearn, and pressure set to placard (not sidewall maximum).
6. **Log date codes and rotation history** so future sessions can advise on age and rotation timing.

## Limitations

- **The vehicle placard and manufacturer approvals are authoritative.** Alternative sizes the math permits may still be unapproved for your vehicle or illegal in your jurisdiction (e.g., load index shortfalls, fender coverage rules).
- **Tire models change constantly** — the skill advises on categories and selection criteria confidently, but specific current models and prices should be verified against recent tests and local availability.
- **Cannot see the tire.** Sidewall damage, puncture position, and cord exposure need physical inspection; when in doubt about repairability, a tire shop's judgment rules.
- **Vibration diagnosis overlaps with suspension** — wheel balance is one cause among several; persistent vibration belongs in [Vehicle Troubleshooting](../vehicle-troubleshooting/).
- **Winter traction devices** (chains, studs) and their legality vary by region — verify local rules.

## Related Skills

- [Vehicle Customization Advisor](../vehicle-customization-advisor/) — aesthetic and performance wheel upgrades in a build context
- [Vehicle Troubleshooting](../vehicle-troubleshooting/) — vibrations and noises beyond the tires themselves
- [EV Assistant](../ev-assistant/) — why EVs eat tires and what to do about it
