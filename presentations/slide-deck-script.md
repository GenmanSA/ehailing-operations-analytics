# E-hailing Operations Analytics — Slide Deck Script

**Format:** 12-slide presentation with slide copy and speaker notes  
**Focus:** Gauteng, South Africa  
**Period:** Driver experience, 2018–2025; modeled comparisons, 2016–2026

> **Presenter guidance:** Keep observed field captures, model assumptions, and simulated outputs clearly distinct. The simulation contains 2,000,000 synthetic trip records and 1,500 synthetic driver profiles; it is not platform data. The field dataset contains 19 dispatch/receipt captures and four campaign or wallet records, which are illustrative and not representative of the market. Replace any modeled headline with a verified result from the latest run before presenting.

---

## Slide 1 — Title

### On-slide text
**E-hailing Operations in Gauteng**  
Driver economics, fleet costs, and pickup safety  

A driver-led exploratory analysis | 2018–2025 experience · 2016–2026 modeled comparisons

**Karabo Eugene Hlahla**  
Pretoria, Gauteng, South Africa

### Suggested visual
Use a clean title slide with a Gauteng map or one strong project visual. Avoid an overcrowded collage.

### Speaker notes
“Hello, and thank you for taking the time to hear about this project. I worked as an Uber and Bolt partner driver from 2018 through 2025. That experience led me to examine how fares, fuel, unpaid pickup distance, vehicle costs, and pickup safety interact. This is an exploratory analysis: it combines a small set of firsthand captures with a larger synthetic simulation, and I’ll be clear about which is which.”

---

## Slide 2 — The question

### On-slide text
**Are e-hailing trips sustainable after the full cost of operating is counted?**

- What remains after platform deductions and fuel?
- How do unpaid pickup distance and vehicle wear change the picture?
- How exposed are drivers and owners to demand, safety, and cost risk?
- Which proposed changes are worth testing?

### Suggested visual
A simple trip-economics flow: rider fare → platform deductions → driver payout → fuel, wear, lease and other costs → driver net.

### Speaker notes
“The question is not only what a trip pays. It is what remains after the costs and unpaid work required to complete it. I also look beyond the driver to vehicle-owner economics and pickup safety. The goal is to identify questions and interventions that deserve better data and real-world testing—not to claim that this exploratory model settles them.”

---

## Slide 3 — Evidence and scope

### On-slide text
**Two evidence types; different jobs**

**Field captures**  
19 dispatch/receipt records + 4 campaign or wallet records

**Synthetic scenarios**  
2,000,000 simulated trips + 1,500 synthetic driver profiles

**Experience**  
Partner driving on Uber and Bolt, 2018–2025

### Suggested visual
Three clearly separated cards labeled “Driver experience,” “Field captures,” and “Synthetic simulation.”

### Speaker notes
“The field captures are firsthand snapshots, but they are a small convenience sample, not a representative survey. The large dataset is synthetic: its size helps explore the behavior of the programmed assumptions, but it does not make the results observed market facts. My driving experience covers 2018 through 2025; comparisons extending from 2016 to 2026 are analytical scenarios, not a claim of continuous personal records across that period.”

---

## Slide 4 — What determines trip economics?

### On-slide text
**Headline fare is not the same as operating return**

A more complete trip calculation considers:

- Driver payout after platform deductions
- Paid trip distance and unpaid pickup distance
- Fuel and vehicle wear
- Tolls, deadhead/return travel, and time
- Lease, finance, insurance, and downtime where relevant

### Suggested visual
Use an annotated trip diagram showing pickup distance, paid trip route, and possible return/deadhead. Add a small formula: `Net operating result = payout − operating costs`.

### Speaker notes
“A fare per paid kilometre can be misleading if the driver must travel to the pickup without compensation or return from a low-demand destination. The project estimates fuel and service-and-wear costs for the captured trips, but no single calculation includes every cost a driver may face. For that reason, I describe these as modeled operating results, not a universal measure of profit.”

---

## Slide 5 — Field captures: examples, not prevalence

### On-slide text
**The captured offers show why trip-level cost accounting matters**

- Compare paid distance with total driven distance.
- Include pickup distance and tolls where recorded.
- Apply the project’s stated fuel and wear assumptions.
- Treat each record as an example—not a market-wide rate.

### Suggested visual
Use `visuals/pair10_primary_field_research_validation.png` or `visuals/pair11_algorithmic_decay_and_unpaid_pickup.png`. Add a visible note: “19 captured records; convenience sample; illustrative cost assumptions.”

### Speaker notes
“These captures let us inspect individual offers more carefully. For each one, the project compares the offer with total distance that may need to be driven, then applies explicit fuel and vehicle-wear assumptions. The examples can reveal questions worth investigating, such as low effective return or long unpaid approaches. With only 19 records, however, they cannot establish how common those outcomes are across either platform.”

---

## Slide 6 — The historical comparison

### On-slide text
**A 2016–2026 comparison is a scenario until its inputs are sourced**

- The code uses assumed fare, commission, and fuel inputs for each period.
- Nominal rand values do not account for inflation.
- Archived tariffs and dated fuel-price sources are needed for a historical claim.
- Sensitivity analysis can show how conclusions change when inputs vary.

### Suggested visual
If retaining `visuals/pair3_driver_exploitation_and_leases.png`, label every value “model input” or “scenario output” and include the source/status of each input. Otherwise, use a comparison table with columns for value, year, source, and evidence status.

### Speaker notes
“The project contains a 2016-versus-2026 model, but those figures should be treated as scenario inputs unless they are backed by dated sources. The current comparison is nominal, so inflation also matters. Before making a claim about a decade-long market trend, I would validate platform tariff records, commission details, and fuel prices for each period, then compare them in both nominal and inflation-adjusted terms.”

---

## Slide 7 — Demand variability

### On-slide text
**Demand timing is an important hypothesis to test**

- The model assigns different demand weights to salary windows, event dates, weekends, and other days.
- Those weights are assumptions, not measured platform demand.
- Real trip, online-time, and earnings records are needed to measure actual cycles.

### Suggested visual
Use `visuals/pair2_payday_and_stadium_spikes.png` only with a prominent “synthetic scenario” label. Better: show a proposed analysis plan beside the modeled chart.

### Speaker notes
“The simulation explores how different assumptions about payday periods, event days, and mid-month demand could affect trip patterns. It does not verify that those patterns occurred at the modeled size. To answer this properly, we would need dated trip or driver-session data across multiple months, with a clear definition of revenue, online hours, and completed trips.”

---

## Slide 8 — Pickup safety and reliability

### On-slide text
**Safer pickup design is a proposal to evaluate—not a proven result**

- The model assigns different cancellation and incident probabilities to zone categories.
- Those probabilities are assumptions in the simulation.
- Designated pickup points may be worth piloting with drivers, passengers, and local stakeholders.
- Measure safety, wait time, accessibility, cancellations, and trip completion.

### Suggested visual
Use a Gauteng map or a simplified pickup-zone concept. If showing `visuals/pair14_smart_safety_pickup_zones_impact.png`, label the comparison “modeled intervention scenario,” not observed impact.

### Speaker notes
“The project proposes designated or safer pickup locations in areas where pickup friction may be a concern. The modeled reductions in cancellations or incidents are not measured intervention outcomes; they follow from probability settings in the code. A responsible next step would be a limited, co-designed pilot with safeguards and a comparison method, while also checking that pickup points remain accessible and do not create new risks.”

---

## Slide 9 — Vehicle-owner economics

### On-slide text
**High mileage makes owner economics sensitive to assumptions**

- Lease revenue must be weighed against finance, insurance, maintenance, tracking, and depreciation.
- Service frequency and annual mileage strongly affect estimated costs.
- Owner outcomes in this project are modeled scenarios.
- Validate costs with invoices, finance statements, insurance quotes, and actual mileage.

### Suggested visual
Use `visuals/pair9_vehicle_owner_financial_trap.png`, with a footnote listing which costs are assumed and which are sourced.

### Speaker notes
“The owner model makes visible how recurring costs can change the economics of a vehicle placed into high-mileage service. But its output depends on assumptions about lease collection, service frequency, financing, insurance, and depreciation. To make this decision-useful for a fleet investor, I would replace those assumptions with real costs from a defined sample of vehicles and model low, central, and high cases.”

---

## Slide 10 — Intervention scenarios

### On-slide text
**Three ideas for testing**

1. **Predictable platform fee:** compare a flat subscription with percentage-based deductions.
2. **Transparent, cost-aware pricing:** test how base fares, distance, pickup, and return costs affect trip acceptance and completion.
3. **Safer pickup design:** pilot designated pickup options in selected locations.

**These are proposals, not validated business outcomes.**

### Suggested visual
Use a three-column framework: idea → mechanism → evidence required. Avoid presenting projected weekly take-home as guaranteed.

### Speaker notes
“The project explores three intervention families: a predictable flat fee, more transparent pricing that recognizes trip costs, and safer pickup design. Each could have trade-offs for drivers, passengers, fleet owners, and a platform. The simulation helps organize hypotheses, but it cannot prove commercial viability. Each proposal needs a clear unit-economics test and operational pilot.”

---

## Slide 11 — What would make the findings stronger?

### On-slide text
**Next steps: move from exploratory analysis to validation**

- Add dated, traceable sources for every historical and cost input.
- Expand field records with a consistent collection template.
- Record trip, pickup, total distance, time, payout, deductions, and relevant costs.
- Publish model assumptions and sensitivity ranges.
- Reconcile labels, record counts, calculations, and charts.
- Test interventions with a defined comparison group and safety measures.

### Suggested visual
A simple maturity path: “Exploratory model → Validated data → Pilot → Evaluation.”

### Speaker notes
“The most valuable next phase is data quality and validation. I would expand the field log, make assumptions traceable, add sensitivity analysis, and check that all record counts and chart labels agree with the source data. If an intervention is piloted, its evaluation should be designed in advance, with outcomes and safety safeguards defined before results are collected.”

---

## Slide 12 — Closing

### On-slide text
**A better e-hailing model starts with transparent evidence**

Fairer economics, safer operations, and sustainable vehicles are connected questions.

**Discussion:** What data or pilot would best test these ideas?

### Suggested visual
A restrained closing image or the project’s strongest field-data visual, with a link to the repository.

### Speaker notes
“My experience motivated this work, and the analysis has helped me organize the operational questions I want to investigate. The field captures are a starting point, and the simulations are a way to explore scenarios—not a substitute for representative data. I hope the next step is to validate the economics and test practical safety and pricing ideas with the people affected. Thank you. I welcome your questions and feedback.”

---

## Source visuals in the repository

- `visuals/pair2_payday_and_stadium_spikes.png`
- `visuals/pair3_driver_exploitation_and_leases.png`
- `visuals/pair9_vehicle_owner_financial_trap.png`
- `visuals/pair10_primary_field_research_validation.png`
- `visuals/pair11_algorithmic_decay_and_unpaid_pickup.png`
- `visuals/pair14_smart_safety_pickup_zones_impact.png`
- `visuals/pair15_bro_r600_flat_subscription_and_owner_turnaround.png`

Before presenting, regenerate visuals from the current analysis and check that their titles, labels, units, sample sizes, and assumptions are accurate. Several chart titles in the current script present simulated outputs in definitive language; relabel those clearly as modeled scenarios.
