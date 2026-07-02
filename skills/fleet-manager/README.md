# Fleet Manager

**English** | [日本語](./README.ja.md)

An AI skill for managing multiple vehicles — maintenance scheduling across a fleet, cost tracking and TCO analysis, downtime planning, driver check routines, and replacement timing.

## Description

The Fleet Manager scales single-vehicle maintenance thinking to fleets of two to two hundred: staggering services so vehicles aren't all down at once, tracking cost per kilometer to spot problem vehicles, building driver inspection routines that catch faults early, and deciding when repairing stops making sense and replacement begins. It works for delivery vans, company cars, trade utes and trucks, and equally well for a family managing several private vehicles.

**Audience:** Small business owners and fleet coordinators, tradespeople running work vehicles, and households managing multiple cars.

## Capabilities

- **Scheduling** — build maintenance calendars across multiple vehicles, stagger major services to protect availability, group work by vehicle or by visit to reduce shop trips, plan seasonal work (tires, inspections) as batches
- **Cost management** — set up cost-per-km/mile tracking, separate fixed vs. running costs, benchmark vehicles against each other to find outliers, budget forecasting for known upcoming services, DIY vs. outsource vs. service-contract tradeoffs
- **Downtime planning** — identify single points of failure ("only one van fits the racking"), spare-vehicle math, prioritizing repairs by operational impact rather than mechanical severity
- **Driver routines** — daily/weekly walk-around checklists appropriate to vehicle type, defect reporting habits that actually get used, fluid and tire routines for non-mechanical drivers
- **Records** — design a minimal record system (spreadsheet-level) that preserves warranty claims, resale value, and cost analysis; what data each service entry needs
- **Lifecycle decisions** — repair-vs-replace analysis on aging vehicles, optimal replacement timing by cost curve, buying considerations for fleet use (parts commonality, dealer network), disposal timing and preparation
- **Compliance awareness** — inspection deadlines, load and licensing basics, record-keeping obligations (flagged generically; local rules vary)
- **Mixed fleets** — handling gasoline, diesel, and EVs in one fleet: different service patterns, fueling/charging logistics, and driver training needs

## Example Prompts

```text
I run 5 delivery vans (3 diesel, 2 EV) doing 40,000 km/year each. Build a
maintenance calendar that never has more than one van off the road.
```

```text
Design a 5-minute daily walk-around checklist my drivers will actually do,
plus a defect report format that reaches me the same day.
```

```text
Van #3 cost 4x the fleet average in repairs this year. Here's the history:
[paste]. Is this a lemon pattern or bad luck? Repair or replace?
```

```text
Set up a spreadsheet structure for tracking costs across 8 vehicles that
lets me compare cost-per-km and spot trends. What columns do I need?
```

```text
Our family runs 3 cars with different ages and mileages. Combine them
into one seasonal maintenance plan with a shared budget forecast.
```

## Recommended Workflow

1. **Inventory the fleet.** For each vehicle: year, make, model, fuel type, current mileage, annual mileage, role, and known condition.
2. **State the operational constraints.** How many vehicles can be down at once, budget cycle, who does the driving, in-house wrenching capability.
3. **Start with the calendar and the checklist.** These two artifacts deliver most of the value fastest.
4. **Feed data back monthly.** Update mileages and costs; ask for outlier and trend analysis as history accumulates.
5. **Run repair-vs-replace analysis** whenever a vehicle needs a repair exceeding roughly 30–50% of its value — before authorizing the work.
6. **Review annually.** Fleet composition, replacement pipeline, and whether the record system is actually being maintained.

## Limitations

- **No persistent database.** The assistant works with the records you paste in each session — the record-keeping system it designs for you is the real memory.
- **Cost figures are estimates**; labor rates, parts prices, and resale values vary by region and time. Use your own actuals wherever possible.
- **Compliance specifics are jurisdiction-dependent** (commercial inspection regimes, tachograph/logging rules, licensing) — the skill flags categories, local authorities define requirements.
- **Not a telematics or fleet-software replacement** for larger fleets; it complements spreadsheet-scale operations and helps you decide when to graduate to dedicated software.
- **Individual vehicle diagnosis belongs to the other skills** — hand off symptoms to [Vehicle Troubleshooting](../vehicle-troubleshooting/) or [OBD-II Diagnostic Assistant](../obd2-diagnostic-assistant/).

## Related Skills

- [Vehicle Maintenance Planner](../vehicle-maintenance-planner/) — the single-vehicle engine this skill multiplies
- [Diesel Specialist](../diesel-specialist/) — diesel-specific care for work vehicles
- [EV Assistant](../ev-assistant/) — charging logistics and EV maintenance in mixed fleets
