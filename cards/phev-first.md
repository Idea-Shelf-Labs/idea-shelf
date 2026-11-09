---
idea_id: phev-first
title: PHEV-first
status: ready
tags: [tech, product]
---

# PHEV-first

**Claim:** At long-dwell parking, many slow chargers should produce more electric miles per dollar than a few fast posts, best used by moderate-battery PHEVs that cover ordinary days on electricity and occasional long trips on fuel.

**Status:** ready · test specified · lab card · unfinished experiment

**Terms (once):** **PHEV** = plug-in hybrid: a grid-charged battery plus a liquid-fuel engine. **BEV** = battery-electric vehicle without an engine. **HEV** = non-plug-in hybrid. **L1 / L2 / DCFC** = Level-1 AC, Level-2 AC and DC fast charging. **Long-dwell** = parking for hours at work, overnight, apartments, streets or driveways. **Stall coverage** = working, accessible outlets relative to parking spaces. **Charge-depleting (CD)** = battery charge is being used; the engine can still run. **Charge-sustaining (CS)** = hybrid operation after the grid-charge allowance is used, not a physically empty battery. **Utility factor (UF)** = a defined share of driving attributed to battery use; label assumptions, engine-off distance and energy-based estimates are not interchangeable. **Gross / usable kWh** = total battery capacity / the portion made available to the driver. **Atkinson / Miller** = engine strategies that trade some specific output for efficiency; motors can supply acceleration torque.

Working figures and unknowns (labeled):

- **Working assumption — daily sizing:** start with **35–50 electric miles**, with **40 miles** as a test choice, not a measured optimum or a promise to cover most annual mileage. **Not found:** an independently checked current U.S. vehicle-day distribution establishing the fraction this target covers. Household or driver averages are not vehicle-day percentiles. [S1]
- **Working assumption / derived — energy:** at **0.30 kWh/mile of battery output**, 40 miles uses **12 kWh usable energy**. Assumed **86–92% wall-to-battery efficiency** gives approximately **13–14 kWh at the wall**. The **0.30 kWh/mile** figure is an example; real PHEV consumption varies a lot by vehicle. This is an illustrative energy budget, not a specification for every PHEV. Gross pack capacity is a different quantity.
- **Derived — refill:** 13–14 wall kWh divided by **1.4 kW** is **9.3–10 hours**; at **3.3 kW**, about **3.9–4.2 hours**. An **eight-hour** stay at a steady 1.4 kW supplies **11.2 kWh wall energy**, about **80–86%** of this example's required wall energy (**derived: 11.2 ÷ 13–14**), not a full forty-mile refill. That reinforces the design point: a full refill each stop is not required. Actual power, temperature, accessories, vehicle acceptance and sharing affect delivery. The **33 kW / 10-port = 3.3 kW** figure is an illustrative shared pool, not a claim that any single car draws 33 kW. **Published manufacturer example:** the June 2025 announcement for the 2026 Prius plug-in specifies roughly **11 hours at 120 V** or **4 hours on L2** under ideal conditions; this is not a universal PHEV recharge time. [S2]
- **Published assumptions / derived — infrastructure costs:** NREL's **June 2023** model inputs, based on earlier studies, sum to commercial L2 **$4,400–10,600 per port** and **150-kW DC $112,200–196,200 per port**, equipment plus installation. Cross-range division gives about **11–45 times** for these particular bands, not all DC equipment or a whole-site productivity ratio. Utility-side upgrades, energy/demand charges, maintenance and some delay-related soft costs are excluded. These are historical assumptions, not current quotes. **Not found:** a defensible all-in commercial L1 price for the proposed site. [S3]
- **Not found / working assumption / illustrative — coverage:** no universal optimum share of wired stalls is established. Port count alone does not determine usable access or site peak; simultaneous draw, building loads, managed caps and departure needs matter. **Illustrative parking facility (100 vehicles):** ten 7 kW ports total **70 kW** aggregate nameplate; one hundred 1.4 kW ports total **140 kW**. The same hundred outlets can instead share one **33 kW** connection (about **0.33 kW** each if all draw at once; managed sharing raises per-vehicle power when fewer cars charge). The number of accessible connections need not equal the electrical capacity available to all of them simultaneously. Installation and operating cost per connection remain a **labeled unknown** — no site quotes are claimed here. The refill bullet's **33 kW / 10-port = 3.3 kW** example is the same sharing idea at a smaller scale.
- **Published — incremental plug-in use:** European fuel-use observations and a manufacturer-specific North American charging sample show different outcomes. They inform the additional grid-electric benefit, not whether hybridization itself works. The Appendix preserves their populations, measurement definitions and vintages. [S4–S7]
- **Published / derived / not found — battery allocation:** IEA's **2026** outlook reports **2025** average U.S. packs of about **90 kWh for BEVs** and less than **20 kWh for PHEVs**. This is capacity, not petroleum savings per kilogram. Dividing **60 kWh** among **four 15-kWh gross packs** equips four PHEVs rather than one 60-kWh BEV. With equal annual mileage, their engine-off electric distance exceeds the BEV's only if their average engine-off share exceeds **25%**: four times share must exceed one. This illustration ignores efficiency, chemistry, degradation, extra engines and cost. **Illustrative fleet pack-capacity comparison:** one million 75 kWh BEVs install **75 GWh**; one million 20 kWh PHEVs install **20 GWh** — about **73% less** installed pack capacity (**derived: (75−20)/75**). This is pack capacity only, not equal electric miles, fuel use or lifecycle performance. Added engines, fuel systems and maintenance offset part of any material or cost saving and must be counted separately. **Not found:** a matched demonstration that the package beats HEVs or BEVs per kilogram of each constrained material. [S8]
- **Headline test metric — working proposal:** electric miles captured per kWh of installed battery capacity. A smaller pack that is fully used on ordinary days can be more productive than a larger pack that rarely depletes. Optimal pack size among about **10, 15, 20 or 30 kWh** remains an **open question**; it depends on the daily driving distribution, charging access and vehicle efficiency. No measured optimum or invented result is claimed here.

## 1. The problem

A car can sit beside a charger it cannot reach while other cars spend hours without an outlet. Speed helps a passing vehicle; reliable access helps a parked one. Workplaces, overnight parking, apartments, streets and driveways can all offer long stays, though each needs its own electrical and access plan.

The broader framing is **distributed electrification** rather than maximizing electric range on every individual vehicle: many cars with modest packs sized for regular days, replenished slowly during time they already spend parked; hybrid drivetrains keep long-distance capability; managed charging limits expensive electrical upgrades; and liquid fuel remains a second energy pathway. This is not a claim that PHEVs should replace BEVs. Complete cost, actual energy prices, range needs and driver preference still decide the fit.

Start with hybridization. Regenerative braking recovers some slowing energy; motor assistance, engine load management and stop/start can reduce combustion fuel use without an external charge. Gains depend on drivetrain design and duty cycle. A PHEV retains those functions after using its grid-charge allowance. The plug adds another benefit: substituting grid-electric travel for fuel-driven travel. [S12, S13]

The proposal pairs that efficient hybrid with a modest battery and dependable charging. Actual prices and driver preferences determine when plugging in makes sense. Price response is a mechanism to test, not a universal behavior already established. An unplugged PHEV has not lost the mechanisms of hybridization, though its additional plug and battery may fail to earn their cost.

## 2. The insight

At long dwell, spread useful access before buying speed vehicles cannot use. Match energy needed to available time, vehicle acceptance and the site's power budget. Pair that access with a moderate battery and fuel range for longer journeys.

Under comparable chemistry, packaging and engineering, a smaller pack has less mass, material and battery cost than a larger one. That is not proof of a lighter or cheaper complete PHEV: its engine, fuel system and transmission also carry mass, manufacturing cost and maintenance. Compare complete cars serving the same need.

Saving some battery charge for later stop-and-go travel on a known mixed route may save fuel. That is a working assumption to compare with charge-first operation, not a universal instruction to use the engine on highways. Electric highway driving can still be advantageous.

**Serious rival:** an efficient HEV where the added plug does not pay or useful charging is absent; it already offers hybrid benefits with a smaller battery. A sensibly sized, affordable BEV can use the same long-dwell outlets and remove the combustion drivetrain. This card differs by keeping the hybrid baseline, adding a modest pack for ordinary-day electric miles, and letting complete cost, actual energy prices, range needs and driver preference decide the fit rather than assuming one vehicle class wins everywhere.

## 3. The proposal

### Vehicle and powertrain

Use the moderate range band as a starting test, not the only legitimate battery size. Choose an efficient charge-sustaining hybrid architecture. Atkinson or Miller operation, power-split/eCVT systems and competing hybrid designs are candidates, not mandatory specifications. Motors can assist acceleration while the engine operates efficiently. No new efficiency percentage follows merely from naming an architecture. [S12, S13]

Provide separate electric-range, wall-energy and charge-sustaining MPG information. There is no proposed mandated MPG floor, vendor or compulsory charging habit. **Not found:** a measured effect showing labels alone change purchasing or charging enough to deliver the intended outcome.

Licensing is one possible route, not a complete production powertrain. Toyota's **3 April 2019** announcement offered patent licenses through **end-2030** under negotiated terms, with technical support charged separately. It does not establish current uptake, a production contract or a guaranteed efficiency gain. [S9]

Compare any route-aware charge-saving control with charge-first operation on matched journeys. Account for fuel, wall energy and engine-off distance, including heating, safety and battery-protection engine starts.

### Market choice and cost per mile

Compare the price the driver actually pays with actual route-specific efficiency:

- Fuel-only CS energy cost per mile = gasoline price per gallon divided by actual CS miles per gallon.
- Engine-off electric energy cost per mile = wall kWh per mile multiplied by the applicable price per kWh.
- If using battery-output energy instead, divide it by charging efficiency first. Do not add losses again to wall-metered use.
- For blended travel, add actual fuel and wall-electricity bills before dividing by miles. Allocate session, time-based and extra parking charges over miles served; include subscriptions where they change the choice.

Cheap electricity can reward charging; expensive tariffs, little dwell or someone else paying for fuel can change the decision. Measure response rather than imposing a charging quota. These are marginal energy comparisons. For ownership, count purchase cost minus resale value, plus interest/fees, maintenance, insurance and charging equipment over the same period and mileage. Do not count both full purchase price and depreciation as separate capital costs.

### Parking lots

Provide working, reachable outlets, clear prices, billing and repairs. Use L1 where dwell suits the energy needed; use shared or managed L2 where it does not. Home charging remains an option where practical. Wiring alone is not evidence of changed behavior.

Compare infrastructure the enrolled cars can use. An AC-only PHEV cannot test a DC-only control arm. Use compatible AC comparisons; assess DC separately with compatible vehicles. Sharing can expand access without a feeder sized for every port's simultaneous nameplate draw, but actual delivery remains limited by the site, circuits, cables, phases, ports and onboard chargers. Report completion times and coincident demand: many slow ports do not automatically reduce peak load. [S16, S17]

### Energy independence, preparedness and supply security

**Energy independence:** useful grid-electric miles can reduce ordinary petroleum demand and exposure to oil supply while retaining efficient fuel travel for longer journeys. This is diversification, not complete independence from fuel, imported resources or electricity supply. [S14]

**Disaster preparedness:** stored fuel and battery energy offer different transportation paths. Fuel can help when charging is unavailable; battery energy can support electric trips when fuel access is constrained, where the vehicle allows it. Starting energy differs from access to replenishment. Shared outages can disable charging and fuel pumps; roads and supplies can fail. A charged BEV also stores energy. Dual capability does not guarantee mobility or household backup power. [S14, S15]

**National security:** less ordinary petroleum use and more than one energy route can reduce supply exposure. Optional compatibility with domestically producible liquid fuels can add a route only where compatible fuel and distribution exist. Capability is not supply, assured low-carbon fuel or guaranteed resilience. Feedstock, land, water, seasonal blends and distribution need their own assessment. Vehicle-to-home power requires model-specific equipment and verified ratings.

### Public support for useful electric travel

**Working policy proposal:** public support should make room for efficient modest-battery PHEVs and useful charging access, alongside other ways to meet the same travel needs. The budget aim is broader reach: if proposed support and program cost per vehicle are lower, a fixed budget can offer support to more households. A smaller pack does not itself set the payment or establish more fuel displaced per public dollar.

Compare packages on additional useful electric travel and petroleum displaced per public dollar, practical charging access, buyer cost and complete-vehicle cost. Use the efficient HEV and a right-sized BEV as serious alternatives; include charging access and other mobility investments where they serve the same need. Count useful longer-range capability too. Record actual fuel and wall-energy use, compare supported purchases with what would have happened without support, and verify performance before claiming a national result. Drivers retain the choice between fuel and electricity.

A candidate first-40-electric-mile cap and a continuous logarithmic battery credit are different, unselected designs. Payment per kWh, payment per rated electric mile, flat support, eligibility including BEVs or HEVs, and any link to measured use remain open. No rate, current-law entitlement, regulatory multiplier or current funding allocation is assumed. The support proposal does not establish 40 miles as an optimum.

## 4. Why this

The attraction is distributed electrification: an efficient hybrid even when running on fuel, a modest battery instead of a large-pack burden, broadly available slow outlets during ordinary parking, managed charging that limits feeder upgrades, and liquid range as a second energy pathway. Market prices and driver choice are the organizing mechanism. Established hybrid mechanisms do not depend on external charging; additional grid-electric mileage does. The card does not argue that PHEVs should replace BEVs.

**Published product comparison, not a measured ownership result:** June 2025 announcements for model-year 2026 list the Prius plug-in SE at **$33,775 base MSRP**, a **13.6-kWh** battery, **44-mile** manufacturer-estimated electric range and up to **52 MPG** combined hybrid operation. The Prius HEV LE starts at **$28,550** and up to **57 MPG** combined. The **$5,225** difference is derived from base MSRPs, not matched-equipment transaction prices; both exclude processing/handling. These are dated specifications/estimates, not inventory or observed owner MPG. An owner who rarely charges still needs to compare the plug-in premium and fuel-mode use with the HEV. [S2, S10]

**Counterevidence:** a July 2025 EU lifecycle model estimates **163 g CO2e/km** for PHEVs, **63 for BEVs** and **188 for HEVs**, for medium-segment cars sold in 2025 using modeled lifetime use and a projected **2025–2044 EU electricity mix**. It strongly favors BEVs per vehicle on emissions; it does not test this fixed-battery-budget proposal or measure U.S. lifetimes. The package is not established as inherently cleaner or cheaper than BEVs. [S11]

Battery chemistry also matters: a smaller pack does not automatically save every constrained mineral compared with a larger pack of another chemistry. LFP avoids nickel and cobalt but still uses other materials and has supply-chain exposure. Capacity ratios alone are not mineral-saving ratios. [S8]

## 5. How you'd know

Score three comparisons separately: hybrid versus a comparable non-hybrid; PHEV versus HEV for the extra plug/battery; and complete PHEV versus BEV ownership. A good charging-lot result proves none of those vehicle comparisons by itself.

- **Vehicle use:** actual fuel and wall energy, engine-off electric distance/total distance, CD distance separately, charging events/driving days, CS MPG and battery throughput. Separate private/company users, home access, routes, weather and vehicle types. Charging frequency is not electric-mile share; fuel with charge remaining can reflect rational prices, heating or control needs.
- **Access and power:** working outlets, usable opportunities, faults, conflicts, dwell, refill completion, feeder allocation and actual coincident site demand. A blocked or broken port is not useful access.
- **Cost:** dated bids/invoices for equipment, wiring, utility work, software, maintenance, energy and demand charges. Compare incremental electric travel per incremental all-in infrastructure dollar over the same horizon, alongside gallons displaced.
- **Allocation and support (headline test metric):** electric miles captured per kWh of installed battery capacity, plus additional travel/fuel displacement per public dollar, gross battery kWh and, with a bill of materials, kilograms of each named material. Include extra engines, full vehicle costs, manufacturing and electricity supply when claiming lifecycle benefit. Compare pack sizes (about 10, 15, 20 or 30 kWh) on that productivity metric rather than assuming a larger pack is always better. Supported sales alone do not establish additional purchases or displacement.

Record who pays, the actual fuel-versus-wall price difference, what the driver chose and whether access prevented the cheaper choice. Continued fuel use when electricity is dearer can be rational, not failure of hybridization.

## 6. First test

Start with a **90-day logged pilot — working test duration** at comparable long-dwell sites or randomized groups within a site. Record a baseline and stratify home access, ownership, route and vehicle; compare tariffs, eligibility and access hours.

- **A:** fewer compatible AC outlets with higher available power per outlet.
- **B:** more lower-power or managed AC outlets within a comparable total infrastructure budget.

Use actual bids and a common cost horizon. Define outcomes and missing-data treatment before collecting results. Compare useful electric distance per dollar, electric miles captured per installed battery kWh, gallons displaced, access, refill completion (including partial refills) and coincident peak. Include compatible BEVs to test whether the outlet pattern works independently of the PHEV proposal, and efficient HEVs for matched fuel/cost comparisons. A DC arm belongs only in a compatible population.

Observe price-led choices without a compulsory charging quota. Test route-aware versus charge-first control separately. The pilot can test feasibility and local effects; seasonal follow-up and a larger sample are needed before annual or national conclusions. If the plug does not earn its cost, the HEV may win; if a BEV meets the same need at lower complete cost, that is a valid result.

## 7. Open questions

- Which modern vehicle-day distribution and seasonal routes justify the starting pack band?
- What pack size (about 10, 15, 20 or 30 kWh) maximizes electric miles captured per installed kWh for a given daily-driving distribution, charging access and vehicle efficiency? No optimum is claimed here.
- What are all-in install and operating costs per accessible low-power connection versus fewer higher-power ports at the same site? Cost per connection remains unknown without site quotes.
- Who plugs in when prices and access favor it, and how do private/fleet users differ?
- Does route-aware control outperform charge-first operation on matched journeys?
- Which local all-in bids, feeder constraints and car acceptance limits govern usable access?
- Does allocation survive chemistry-specific materials, extra engines and equal-budget comparisons?
- Do labels alone produce a useful change in purchasing or charging?
- Which disruption scenarios benefit from dual stores after allowing for pumps, roads and starting charge/fuel?
- Which support design, payment amount and eligibility best serve additional useful travel and petroleum displacement? The capped-range and logarithmic proposals remain unresolved.

## 8. Why it might not work

- The additional plug/battery does not earn enough useful service, or a favorable energy price fails to attract use.
- Heating, power demand and control strategy produce fuel use during battery depletion.
- Wiring, utility work, billing and repairs make access expensive or unreliable.
- Shared power, short dwell or cold prevent the intended replenishment; simultaneous demand erases an assumed peak advantage.
- An efficient HEV or sensibly sized BEV meets the same need at lower complete cost or impact.
- A second energy capability lacks available supply, or the same disruption blocks both routes.
- Public support pays for purchases that would have happened anyway, or lower-cost awards do not produce greater additional benefit per dollar.

These outcomes test the incremental plug, pack, access and support proposal; they do not undo the established hybrid mechanisms.

## 9. Stress-test

**“Forty miles covers ordinary life.”** It is a design target, not a measured percentile or annual-coverage promise. Household, driver, vehicle-day and annual denominators cannot be swapped. [S1]

**“No charging means no hybrid benefit.”** Hybrid mechanisms do not require an external charge. Charging is needed for the extra grid-electric service, whose realized use must be scored separately. [S13]

**“Drivers always choose the cheaper source.”** Price response is intended, not universal. Actual route costs, who pays, access and convenience belong in the test.

**“Battery depletion means engine-off driving.”** CD can include fuel use. Keep engine-off distance, CD distance, energy share and weighting definitions distinct; fuel-only consumption is not total energy or MPGe. [S4]

**“A small pack makes the whole car lighter and cheaper.”** The pack saving is conditional on comparable engineering; the combustion drivetrain still counts. A battery-allocation illustration is not a demonstrated national oil saving.

**“Many slow always wins.”** Only compare where dwell and acceptance suit the service. Fast charging remains useful en route and for quick turnaround. Reject the lot hypothesis if compatible higher-power infrastructure wins on useful electric travel per all-in dollar.

**“A budget cap settles the support case.”** A smaller pack does not determine the award amount or cause additional travel. Compare what the spending changes, including alternatives and useful longer range, before selecting a design.

**Verdict:** the thesis is distributed electrification built on an efficient hybrid with a modest plug-in pack, plentiful long-dwell access and market-led choice of the cheaper energy source — not a claim that PHEVs should replace BEVs. Hybrid mechanisms are established; electric miles captured per installed battery kWh, the best pack size, price response and added value of plug/access/support are comparisons to score. The Claim's “best used by” is a comparative proposal, not a demonstrated universal winner.

## Appendix: Sources

### Observed incremental plug-in use

**Published:** a **February 2026** European analysis uses OBFCM records from **2021–2023**. Its table 3 covers about **981,000 PHEVs**: vehicle-mean fuel consumption **5.89 L/100 km** versus **1.53 L/100 km WLTP**, with mean CD-mode fuel consumption **2.82 L/100 km**. These are fuel-only figures, not total energy or lifecycle emissions, a U.S. estimate or a test of the proposed lot. [S4]

The same table's **km-weighted** CD distance is **39.0%**, engine-off CD distance about **27.4%**, and energy-based share **31.0%**. Its **6.12 L/100 km** km-weighted fuel mean differs from the **5.89** vehicle mean. Dividing incompatible weightings would manufacture a misleading comparison. [S4]

**Published, manufacturer-specific:** Toyota's **20 May 2026** summary covers more than **6,000** U.S./Canadian RAV4 Prime and Lexus NX PHEVs, model years **2021–2024**. It estimates charging on about **seven in ten driving days** for Toyota and **eight–nine in ten** for Lexus; **9%** and **4%**, respectively, rarely charge. Those are frequency estimates, not electric-mile shares. Exact observation dates and ownership mix are not verified from the summary. [S5]

**Published abstract only / not found:** the related SAE paper, published **7 April 2026**, describes one full calendar year for hundreds of North American vehicles. Its public abstract does not disclose the observation year; full sampling methods are not independently checked. Do not equate its sample with the manufacturer's larger summary sample. [S6]

**Published historical comparison:** a **2022** ICCT/Fraunhofer study of about **9,000** European PHEVs estimates electric-driving shares of **45–49% for private cars** and **11–15% for company cars**. Its mixed older datasets are not 2026 measurements or interchangeable with North American charging-day frequency. [S7]

These studies constrain the additional electric service; they do not test whether regenerative braking or hybrid engine management works.

### Source register and vintages

- **S1 — published survey:** FHWA, *2022 NHTS Summary of Travel Trends*, **January 2024**; travel collected **January 2022–January 2023**. Means do not establish the missing current vehicle-day percentile. [Report](https://nhts.ornl.gov/assets/2022/pub/2022_NHTS_Summary_Travel_Trends.pdf).
- **S2 — published manufacturer announcement:** Toyota, **16 June 2025**, model-year **2026 Prius plug-in** specifications and estimates; launch MSRP, not transaction quotes or measured owner use. [Announcement](https://pressroom.toyota.com/toyota-prius-plug-in-hybrid-gets-edgier-with-new-nightshade-edition/).
- **S3 — published model inputs:** NREL, *The 2030 National Charging Network*, **June 2023**, §2.3.4/table 5, printed p. 33; earlier historical studies underlie its cost assumptions. [Report](https://docs.nlr.gov/docs/fy23osti/85654.pdf).
- **S4 — published observational analysis:** Fraunhofer ISI / Öko-Institut / ifeu, *Regulatory adjustments for plug-in hybrid vehicles in Europe*, **18 February 2026**; §§2.1–2.2/table 3, reporting/registration records **2021–2023**, deduplicated to each vehicle's latest record. [Report](https://publica-rest.fraunhofer.de/server/api/core/bitstreams/ac662473-acb6-462a-900d-b7066eb460c8/content).
- **S5 — published manufacturer summary:** Toyota, *Do Plug-In Hybrid Owners Actually Plug In?*, **20 May 2026**, model years **2021–2024**, exact observation dates not specified; charging inferred rather than a direct electric-mile-share finding. [Summary](https://pressroom.toyota.com/do-plug-in-hybrid-owners-actually-plug-in/).
- **S6 — published abstract only:** SAE **2026-01-0429**, **7 April 2026**; a full calendar year, observation year undisclosed in the public abstract. [Abstract](https://saemobilus.sae.org/papers/identifying-patterns-real-world-charging-frequency-a-sample-plug-hybrid-electric-vehicles-north-america-2026-01-0429).
- **S7 — published historical observational comparison:** ICCT/Fraunhofer, *Real-world usage of plug-in hybrid vehicles in Europe: A 2022 update*, **2022 publication**, heterogeneous earlier private/company datasets. [Registry and abstract](https://publica.fraunhofer.de/entities/publication/f7607ab2-d7d2-42dd-80fe-2cd229fa1b51).
- **S8 — published market analysis:** IEA, *Global EV Outlook 2026*, battery chapter; **2026 publication**, **2025** deployment and pack-capacity observations. Chemistry and capacity do not establish matched material or fiscal efficiency. [Chapter](https://www.iea.org/reports/global-ev-outlook-2026/electric-vehicle-batteries).
- **S9 — historical manufacturer offer:** Toyota, **3 April 2019**, patent licensing and separately charged technical support; stated offer through end-2030, not a verified current supply contract. [Announcement](https://global.toyota/en/newsroom/corporate/27512455.html).
- **S10 — manufacturer announcement:** Toyota, **16 June 2025**, model-year **2026 Prius HEV** launch prices and estimates. [Announcement](https://pressroom.toyota.com/electrified-trailblazer-the-toyota-prius-celebrates-25-years-in-the-u-s/).
- **S11 — lifecycle model:** ICCT, **8 July 2025**, EU medium-segment 2025 cars and projected lifetime energy mixes; not measured lifetime totals. [Report](https://theicct.org/publication/electric-cars-life-cycle-analysis-emissions-europe-jul25/).
- **S12 — mechanism explanation:** Toyota UK, **14 January 2015**, updated **26 July 2024**; simulated Atkinson operation and motor assistance, not proof that a named cycle is necessary. [Explanation](https://mag.toyota.co.uk/toyota-use-atkinson-cycle-engines/).
- **S13 — established mechanisms:** DOE Alternative Fuels Data Center and DOE/EPA, undated engineering guidance; no universal percentage gain implied. [Hybrid explanation](https://afdc.energy.gov/vehicles/electric-basics-hev) · [Mechanisms](https://www.fueleconomy.gov/feg/hybridtech.shtml).
- **S14 — energy diversification explanation:** DOE AFDC, *Electric Vehicle Benefits and Considerations*, undated guidance; energy-security and infrastructure-availability sections. Diversification is not a measured vehicle-class resilience guarantee. [Explanation](https://afdc.energy.gov/fuels/electricity-benefits).
- **S15 — historical supply-dependency explanation:** EIA, *Weather and other events can cause disruptions to gasoline infrastructure and supply*, **1 February 2013**; electricity dependencies across refining, distribution and retail, not a new outage measurement. [Explanation](https://www.eia.gov/TodayinEnergy/detail.php?id=9811).
- **S16 — manufacturer mechanism guidance:** MENNEKES, *Wallboxes and charging columns with load management*, undated; dynamic building-load measurement and phase-aware current allocation, not guaranteed utilization or optimal completion. [Explanation](https://www.mennekes.org/emobility/products/load-balancing/).
- **S17 — infrastructure planning guidance:** DOE AFDC, *Workplace Charging for Electric Vehicles*, undated; access, vehicle needs, equipment, pricing and ongoing management. [Guidance](https://afdc.energy.gov/fuels/electricity-charging-workplace).
