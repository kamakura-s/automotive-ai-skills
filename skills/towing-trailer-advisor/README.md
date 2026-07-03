# Towing & Trailer Advisor

**English** | [日本語](./README.ja.md)

An AI skill for towing safely — hitch selection and ratings, tongue weight and load distribution, trailer wiring and brake controllers, sway prevention, and trailer maintenance.

## Description

Towing is where small mistakes compound at highway speed: a hitch class mismatch, ten percent too little tongue weight, or an unmaintained wheel bearing can each end a trip or worse. The Towing & Trailer Advisor covers the whole chain — tow vehicle capability, hitch and coupling selection, loading the trailer correctly, wiring lights and brakes, driving technique differences, and the maintenance schedule trailers need but rarely get. It applies to utility trailers, boat trailers, caravans/campers, and car haulers.

**Audience:** First-time towers, boat and camper owners, and anyone whose trailer has been sitting for a while.

## Capabilities

- **Capacity math** — reading tow ratings correctly (GVM, GCM, braked vs. unbraked limits, payload including tongue weight), why the weakest link in the chain sets the limit, margin philosophy for real-world towing
- **Hitches & couplings** — hitch classes and receiver sizes, weight-carrying vs. weight-distributing hitches, when a WDH is needed, fifth-wheel/gooseneck basics, coupler adjustment and safety chain crossing
- **Loading** — the ~10–15% tongue weight rule and how to measure it, the 60/40 forward bias principle, securing cargo on the trailer, water and gear placement in campers, consequences of tail-heavy loading
- **Wiring & brakes** — 4-pin vs. 7-pin functions, diagnosing light faults (grounds first!), electric brake controllers (proportional vs. time-delay, gain setting procedure), breakaway systems and their batteries, surge brakes on boat trailers
- **Sway** — what actually causes sway (loading, speed, geometry, wind), prevention hierarchy, sway control devices, and the correct driver response when sway starts (no steering corrections, no brakes — manual trailer brake and steady throttle)
- **Driving technique** — extended following distances, downhill gear discipline, backing fundamentals (hand at bottom of wheel), swing-out awareness, mirror requirements
- **Trailer maintenance** — wheel bearing service (the #1 neglected item, especially after water immersion on boat trailers), trailer tire age vs. tread, brake inspection, light connector corrosion, frame and coupler cracks
- **Legal awareness** — license class implications by trailer weight, speed limits while towing, mirror and brake requirements by weight class — flagged generically, jurisdiction-specific rules to be verified locally

## Example Prompts

```text
My SUV is rated to tow 2,000 kg braked. The camper I want has a 1,800 kg
GTM. Walk me through whether this actually works, including payload and
tongue weight math.
```

```text
The trailer sways above 80 km/h since I repacked it. What did I probably
change, and what's the fix hierarchy before I buy a sway control device?
```

```text
Trailer running lights work but brake lights and left indicator are dead.
7-pin connector. Give me the diagnostic order.
```

```text
Set up my electric brake controller from scratch: what does the gain do,
and what's the parking-lot procedure to set it correctly?
```

```text
My boat trailer gets dunked in salt water 20 times a year. Build me a
bearing and brake maintenance schedule that keeps it alive.
```

## Recommended Workflow

1. **Start with the numbers.** Tow vehicle ratings (from the manual, not the brochure), trailer weights (actual, from a weighbridge if possible), and hitch/receiver ratings.
2. **State the use.** Trailer type, typical loads, distances, terrain, and how often — a weekly boat launch and an annual house move need different advice.
3. **For setup questions:** work through capacity → hitch → loading → wiring → brake controller in that order; each depends on the previous.
4. **Measure, don't estimate,** tongue weight (bathroom-scale method or tongue scale) and report the number.
5. **Before the first trip:** ask for a hitch-up checklist and a 10-minute pre-departure walk-around, then use them every time.
6. **After storage or immersion:** run the recommissioning checks (bearings, brakes, lights, tires) before loading.

## Limitations

- **Ratings and legal limits are vehicle- and jurisdiction-specific.** The skill teaches the math and the concepts; your owner's manual, door placard, and local road authority define the binding numbers (license classes for trailer weight vary enormously between countries).
- **Cannot verify your actual weights.** Weighbridge measurements beat every estimate — assumptions about "about a tonne" are how overloads happen.
- **Brake controller and wiring work interacts with vehicle electronics** — on newer vehicles with factory tow packages or CAN-based lighting, aftermarket wiring shortcuts can cause faults; when in doubt, use vehicle-specific harnesses.
- **Structural hitch installation** (drilling, frame-mounted receivers) should follow the hitch maker's vehicle-specific instructions and torque specs — verify against those documents.
- **Sway events are driving-safety critical** — the skill teaches prevention and correct response, but no advice substitutes for reducing speed and loading correctly in the first place.

## Related Skills

- [Commercial Vehicle & Truck Assistant](../commercial-vehicle-assistant/) — load securing and weight concepts at commercial scale
- [Tire & Wheel Advisor](../tire-wheel-advisor/) — trailer tire age rules and load ratings
- [Vehicle Maintenance Planner](../vehicle-maintenance-planner/) — folding trailer service into the household schedule
