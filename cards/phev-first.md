---
schema: idea-shelf/card@2
id: phev-first
title: "PHEV first: distributed electrification"
version: 2.0.0
updated: 2026-11-26
status:
  editorial: published
  evidence: test-specified
claim: >-
  At long-dwell parking, many slow chargers should produce more electric miles per dollar than a few fast posts, best used by moderate-battery PHEVs that cover ordinary days on electricity and occasional long trips on fuel.
summary: >-
  Most cars sit parked for hours at work, at home or overnight. This card proposes spreading
  many low-power outlets across those spaces instead of installing a few fast chargers, and
  pairing them with efficient plug-in hybrids whose modest batteries cover ordinary days while
  the engine handles long trips. It builds on established hybrid efficiency, treats the plug
  and battery as an increment that must earn its cost, and specifies a logged pilot that
  scores electric miles per dollar and per installed battery kWh.
domains: [transport, energy, resilience]
patterns: [converge-on-proven, fund-the-high-value-increment, reward-performance, remove-single-points-of-failure]
readiness: deployed
geography: [US]
why_not_yet: >-
  The plug has not reliably earned its premium: many plug-in hybrid owners charge too little,
  most of all where someone else pays for fuel [F16, F22], while North American evidence is
  more favourable but manufacturer-specific [F20]. Site owners carry wiring, billing, repair
  and management costs, and the all-in cost per low-power connection is unknown without site
  bids [F13]. Price-led charging is intended, not yet shown, and no support design has been
  chosen that pays for additional electric travel rather than battery size.
coalition:
  - actor: Drivers who park for hours at work, at home or overnight
    gains: Lower energy cost per mile on ordinary days where electricity is the cheaper source, with liquid-fuel range kept for long trips and no compulsory charging habit.
  - actor: Workplace, apartment and parking-facility owners
    gains: A way to offer charging at many spaces within a fixed electrical budget by sharing a managed connection, instead of sizing the feeder for every port [F8, F15, S16, S17].
  - actor: Utilities and grid operators
    gains: Slow, managed load spread across long stays, if load management caps coincident site demand; many slow ports do not lower peak on their own.
  - actor: Automakers and hybrid powertrain suppliers
    gains: A market for efficient charge-sustaining hybrids with modest packs, competing on labelled electric range and charge-sustaining fuel economy rather than on a mandated vendor.
  - actor: Public budget holders and energy-security interests
    gains: Less ordinary-day petroleum demand and a second energy pathway, with any support compared per public dollar against efficient hybrids and right-sized battery-electric cars [S14].
boundary: >-
  Public support, if any, targets additional useful electric travel and accessible long-dwell
  outlets, and is compared per public dollar with efficient hybrids, right-sized battery-electric
  cars and other mobility spending. It does not pay for battery capacity beyond what ordinary days
  use, mandate a vendor, a fuel-economy floor or a charging quota, or assume any current-law
  entitlement. A first-40-electric-mile cap [F1] and a continuous battery credit are both
  unselected candidate designs.
resilience: >-
  Dependence on a single energy pathway for everyday mobility: the vehicles keep both grid
  electricity and liquid fuel. This diversifies supply exposure; it does not guarantee mobility
  when one disruption disables both pumps and chargers [S14, S15].
losers:
  - who: Fast-charging providers at long-dwell sites
    mitigation: Fast charging stays the right tool en route and for quick turnaround; the pilot rejects the slow-outlet arm if compatible higher-power charging wins per all-in dollar.
  - who: Fuel retailers and refiners
    mitigation: Ordinary-day gasoline volumes fall gradually, while liquid fuel is still sold for long trips, charge-sustaining operation and preparedness reserves.
  - who: Drivers who cannot park for hours or who need long electric range
    mitigation: They gain little from long-dwell outlets; battery-electric cars and fast charging remain eligible alternatives, since the card does not argue that plug-in hybrids replace them.
  - who: Taxpayers, if support pays for purchases that would have happened anyway
    mitigation: Compare supported purchases with a counterfactual and verify measured fuel and wall-energy use before scaling any program.
rival:
  name: An efficient non-plug-in hybrid, or a right-sized battery-electric car on the same outlets
  why_not: >-
    The hybrid keeps the hybrid gains without the plug premium [F26] but displaces no fuel with
    grid electricity, which frequent chargers do [F20, F21]. The battery-electric car is cleaner
    per vehicle in an EU life-cycle model [F23] but installs far more battery per vehicle [F27,
    F28]; per installed kWh, a modest pack used daily can deliver more electric miles [F29, F30].
    These are illustrations, not a matched result [F33]; the pilot scores both rivals.
first_test:
  design: >-
    Logged pilot [F35] at comparable long-dwell sites, or randomized groups within one site, with
    a baseline and stratification by home access, ownership, route and vehicle. Arm A: fewer
    compatible AC outlets with more power each. Arm B: more lower-power or managed AC outlets
    within a comparable all-in budget, using actual bids and a common cost horizon. Enrol
    compatible battery-electric cars and efficient hybrids as comparisons; no charging quota;
    any DC arm only with compatible vehicles. Outcomes and missing-data rules fixed in advance.
  cost_band: $100k-1M
  duration: 90 days logged (working assumption), then seasonal follow-up before annual or national conclusions
  success: >-
    Arm B delivers more engine-off electric miles per all-in infrastructure dollar than arm A,
    with refill completion (partial refills counted) and coincident peak inside the site budget,
    and enrolled plug-in hybrids show high electric miles per installed battery kWh [F31].
  kill: >-
    Compatible higher-power AC outlets (arm A) deliver equal or more useful electric travel per
    all-in dollar than arm B; or the plug and battery of enrolled plug-in hybrids do not earn
    their cost against matched hybrids; or battery-electric cars meet the same need at lower
    complete cost.
  kill_terms: [equal or more, earn, complete cost]
terms:
  PHEV: Plug-in hybrid electric vehicle, a grid-charged battery plus a liquid-fuel engine.
  BEV: Battery-electric vehicle, with no engine.
  HEV: Non-plug-in hybrid electric vehicle.
  L1 / L2 / DCFC: Level 1 AC, Level 2 AC and DC fast charging.
  Long-dwell: Parking for hours at work, overnight, at apartments, on streets or in driveways.
  Stall coverage: Working, accessible outlets relative to parking spaces.
  Charge-depleting (CD): Operation while grid charge is being used; the engine can still run.
  Charge-sustaining (CS): Hybrid operation after the grid-charge allowance is used; the battery is not physically empty.
  Engine-off distance: Distance driven with the combustion engine off; a subset of CD distance.
  Utility factor (UF): A defined share of driving attributed to battery use; label assumptions, engine-off distance and energy-based estimates are not interchangeable.
  Gross / usable kWh: Total battery capacity, and the portion made available to the driver.
  Wall energy: Electricity metered at the outlet, including charging losses; larger than the usable battery energy it replaces.
  Electric miles per installed kWh: Engine-off electric miles divided by installed (gross) battery capacity over the same period; the card's headline productivity metric.
  Atkinson / Miller: Engine strategies that trade some specific output for efficiency; motors can supply acceleration torque.
related: []
figures:

- id: F1
  what: Daily electric-range test target for the modest PHEV pack
  value: 40
  unit: miles of electric range
  low: 35
  high: 50
  label: working-assumption
  sources: [S1]
  note: >-
    Test choice, not a measured optimum or a promise to cover most annual mileage. The 35-50 mile
    band and the 40-mile test point are the card's own design choice; S1 supplies averages for
    context (F2) but no vehicle-day percentile (F3).
- id: F2
  what: Average daily vehicle miles traveled per household, 2022 NHTS (network-calculated distance)
  value: 39.70
  unit: vehicle-miles per household per day
  label: established
  sources: [S1]
  note: >-
    S1 table 2-8 (household) gives 39.70; table 2-9 (person) gives 21.84 vehicle-miles per driver
    per day. Travel collected January 2022 to January 2023; report dated January 2024. Household
    and driver averages are not vehicle-day percentiles.
- id: F3
  what: Share of current U.S. vehicle-days whose driving a 40-mile electric range would cover
  value: null
  unit: percent of vehicle-days
  label: not-found
  sources: []
  note: >-
    No independently checked current vehicle-day distribution was found. S1 reports means only.

- id: F4
  what: Usable battery energy for the 40-mile example
  value: 12
  unit: kWh (battery output)
  label: working-assumption
  sources: []
  note: >-
    40 miles x 0.30 kWh/mile battery output = 12 kWh. The 0.30 kWh/mile consumption is an
    illustrative example; real PHEV consumption varies a lot by vehicle. Gross pack capacity is a
    different (larger) quantity.
- id: F5
  what: Wall energy needed to replace the 40-mile example's usable energy
  value: 13.5
  unit: kWh at the wall
  low: 13
  high: 14
  label: working-assumption
  sources: []
  note: >-
    Assumed wall-to-battery efficiency 86-92%. 12 / 0.92 = 13.04; 12 / 0.86 = 13.95; quoted as
    about 13-14 kWh. Value is the midpoint, shown for the schema only.
- id: F6
  what: Time to supply the example's wall energy at 1.4 kW (Level 1 class)
  value: 9.6
  unit: hours
  low: 9.3
  high: 10
  label: working-assumption
  sources: []
  note: >-
    13 / 1.4 = 9.29 h; 14 / 1.4 = 10.0 h. At 3.3 kW: 13 / 3.3 = 3.94 h; 14 / 3.3 = 4.24 h (about
    3.9-4.2 h). Steady power assumed; temperature, accessories, onboard-charger acceptance and
    load sharing change actual delivery. Value is the midpoint (13.5 / 1.4).
- id: F7
  what: Share of the example's required wall energy supplied by an 8-hour stay at a steady 1.4 kW (partial refill)
  value: 83
  unit: percent
  low: 80
  high: 86
  label: working-assumption
  sources: []
  note: >-
    8 h x 1.4 kW = 11.2 kWh at the wall. 11.2 / 14 = 0.800; 11.2 / 13 = 0.862; so about 80-86%
    of a 13-14 kWh wall budget (F5), not a full 40-mile refill. Midpoint 11.2 / 13.5 = 0.83.
    Design point: a full refill at each stop is not required.
- id: F8
  what: Even per-port share of an illustrative 33 kW shared pool
  value: 3.3
  unit: kW per port
  label: working-assumption
  sources: [S16]
  note: >-
    33 kW / 10 ports = 3.3 kW each if all draw at once. Spread over 100 outlets: 33 / 100 = 0.33
    kW each if all draw at once; managed (load-managed) sharing raises per-vehicle power when
    fewer cars charge (mechanism per S16). Illustrative; not a claim any single car draws 33 kW.
    The lower of the outlet allocation and the car's onboard charger sets actual power.
- id: F9
  what: Manufacturer-stated full recharge time, 2026 Prius plug-in, at 120 V
  value: 11
  unit: hours
  label: established
  sources: [S2]
  note: >-
    S2 states about 11 hours at 120 V or about 4 hours on Level 2 under ideal conditions. Not a
    universal PHEV recharge time. Checked against S2 on 2026-11-25.

- id: F10
  what: Commercial Level 2 capital cost per port (hardware plus installation), NREL model input
  value: 7500
  unit: USD per port (historical, nominal)
  low: 4400
  high: 10600
  label: published-contested
  sources: [S3]
  note: >-
    S3 table 5 (p. 33): hardware $2,200-4,600 + install $2,200-6,000 = $4,400-10,600 (derived
    sums). NREL calls the bounds plausible optimistic and pessimistic estimates from an ensemble
    of earlier studies that differ. Excludes front-of-meter utility upgrades, energy and demand
    charges, maintenance and some soft costs. Not 2026 quotes. Value is the midpoint, schema only.
- id: F11
  what: 150 kW DC fast charger capital cost per port (hardware plus installation), NREL model input
  value: 154200
  unit: USD per port (historical, nominal)
  low: 112200
  high: 196200
  label: published-contested
  sources: [S3]
  note: >-
    S3 table 5: hardware $66,400-102,200 + install $45,800-94,000 = $112,200-196,200 (derived
    sums). Same exclusions as F10. Value is the midpoint, schema only.
- id: F12
  what: Cross-range ratio of 150 kW DC to commercial L2 per-port cost
  value: 21
  unit: times
  low: 11
  high: 45
  label: working-assumption
  sources: [S3]
  note: >-
    112,200 / 10,600 = 10.6 (lowest DC over highest L2); 196,200 / 4,400 = 44.6 (highest DC over
    lowest L2); about 11-45x. Midpoint ratio 154,200 / 7,500 = 20.6. Applies to these bands only;
    not a site productivity ratio or an electric-miles-per-dollar advantage.
- id: F13
  what: All-in installed and operating cost per accessible low-power connection (including commercial Level 1) at a pilot site
  value: null
  unit: USD per connection
  label: not-found
  sources: []
  note: >-
    No defensible figure found; needs dated site bids. S3 excludes L1 from commercial costs
    (table 5 note b: L1 equipment usually comes with the vehicle; only residential L1 install
    $100-1,000 is given).
- id: F14
  what: Universal optimum share of parking stalls with working outlets (stall coverage)
  value: null
  unit: percent of stalls
  label: not-found
  sources: []
  note: No universal optimum established; depends on dwell, simultaneous draw, building load and managed caps.
- id: F15
  what: Illustrative 100-vehicle parking facility, aggregate nameplate of one hundred 1.4 kW outlets
  value: 140
  unit: kW aggregate nameplate
  label: working-assumption
  sources: []
  note: >-
    Illustrative comparison. 100 x 1.4 kW = 140 kW nameplate, versus ten 7 kW ports: 10 x 7 = 70
    kW nameplate. The same 100 outlets can instead share one 33 kW connection (F8: 0.33 kW each
    if all draw). Connections need not equal simultaneous capacity. Port count alone does not set
    usable access or site peak. Cost per connection is F13 (not found).

- id: F16
  what: Real-world combined fuel consumption of European PHEVs (OBFCM 2021-2023), vehicle mean
  value: 5.89
  unit: L/100 km (fuel only)
  low: 5.76
  high: 6.12
  label: established
  sources: [S4]
  note: >-
    S4 table 3, N = 981,035 (deduplicated sample 981,139): median 5.76, mean 5.89, km-weighted
    mean 6.12 L/100 km, versus WLTP combined mean 1.53 L/100 km (median 1.40, km-weighted 1.57).
    low/high here are median and km-weighted mean, not a confidence interval. Fuel only, not total
    energy or lifecycle emissions; not a U.S. estimate.
- id: F17
  what: Real-world fuel consumption in charge-depleting (CD) mode, European PHEVs, vehicle mean
  value: 2.82
  unit: L/100 km (fuel only)
  label: established
  sources: [S4]
  note: S4 table 3 (median 2.07, km-weighted 2.98). Shows CD mode is not engine-off driving.
- id: F18
  what: Share of distance driven in CD mode, European PHEVs, km-weighted mean
  value: 39.0
  unit: percent of distance
  label: established
  sources: [S4]
  note: >-
    S4 table 3 (vehicle mean 42.4%). Energy-based share UF_ener, km-weighted: 31.0%. Keep the
    weighting and definition distinct from F19; do not divide across weightings.
- id: F19
  what: Share of distance driven in CD mode with the combustion engine off, European PHEVs, km-weighted mean
  value: 27.4
  unit: percent of distance
  label: established
  sources: [S4]
  note: >-
    S4 table 3 (vehicle mean 30.9%). The table row is labelled "Share of CD mode km with
    combustion engine from UF_real"; S4's text describes it as CD km with the engine off.
- id: F20
  what: Share of driving days with a charge, Toyota RAV4 Prime PHEVs in the U.S. and Canada
  value: 70
  unit: percent of driving days
  label: established
  sources: [S5]
  note: >-
    S5: about 7 in 10 driving days (Toyota), 8-9 in 10 (Lexus NX); 9% of Toyota and 4% of Lexus
    drivers rarely charge; more than 6,000 vehicles, model years 2021-2024. Manufacturer sample;
    charging inferred from state-of-charge changes (S6 abstract). Charging frequency is not an
    electric-mile share. Checked against S5 on 2026-11-25.
- id: F21
  what: Real-world electric driving share, European private-car PHEVs (2022 study, about 9,000 vehicles)
  value: 47
  unit: percent of distance
  low: 45
  high: 49
  label: established
  sources: [S7]
  note: 'S7 abstract: "about 45%-49% for private cars". Older heterogeneous datasets. Midpoint shown.'
- id: F22
  what: Real-world electric driving share, European company-car PHEVs (2022 study)
  value: 13
  unit: percent of distance
  low: 11
  high: 15
  label: established
  sources: [S7]
  note: >-
    S7 abstract: "about 11%-15% for company cars"; WLTP assumes 70-85% CD driving. Midpoint shown.

- id: F23
  what: Modeled life-cycle GHG emissions, EU medium-segment PHEV sold in 2025
  value: 163
  unit: g CO2e/km
  label: established
  sources: [S11]
  note: >-
    Same S11 model: BEV 63, HEV 188 g CO2e/km, using a projected 2025-2044 EU electricity mix.
    Modeled, not measured lifetime totals; not a U.S. estimate. Checked against S11 on 2026-11-25.
- id: F24
  what: Battery capacity, model-year 2026 Prius plug-in (SE)
  value: 13.6
  unit: kWh
  label: established
  sources: [S2]
  note: >-
    S2 also gives a 44-mile manufacturer-estimated electric range (SE grade). Launch
    specification, not observed owner range.
- id: F25
  what: Manufacturer-estimated combined fuel economy in hybrid operation, model-year 2026 Prius plug-in
  value: 52
  unit: mpg
  label: established
  sources: [S2, S10]
  note: >-
    Up to 52 mpg (S2); non-plug-in Prius LE up to 57 mpg combined (S10). Estimates, not observed
    owner mpg.
- id: F26
  what: Base-MSRP difference, 2026 Prius plug-in SE versus Prius HEV LE
  value: 5225
  unit: USD (launch base MSRP, excl. processing and handling)
  label: working-assumption
  sources: [S2, S10]
  note: >-
    Derived: $33,775 (S2) - $28,550 (S10) = $5,225. Base MSRPs at June 2025 launch, not
    matched-equipment transaction prices. Both prices checked against S2 and S10 on 2026-11-25.
    Later model years have different prices; a model-year 2027 plug-in has since been announced.

- id: F27
  what: Average U.S. battery-electric car pack size, 2025
  value: 90
  unit: kWh
  label: established
  sources: [S8]
  note: Capacity, not petroleum savings.
- id: F28
  what: Average U.S. plug-in hybrid pack size, 2025 (upper bound)
  value: 20
  unit: kWh (S8 says "less than 20")
  label: established
  sources: [S8]
  note: S8 states "less than 20 kWh".
- id: F29
  what: Average engine-off share above which four 15 kWh PHEVs out-drive one 60 kWh BEV electrically
  value: 25
  unit: percent of distance
  label: working-assumption
  sources: []
  note: >-
    60 kWh / 15 kWh = 4 packs. If each car travels the same distance, 4 x share > 1 (the BEV's 100%)
    when share > 0.25. Ignores efficiency, chemistry, degradation, extra engines and cost.
- id: F30
  what: Illustrative fleet comparison, installed pack capacity saved by 20 kWh PHEVs versus 75 kWh BEVs
  value: 73
  unit: percent less installed pack capacity
  label: working-assumption
  sources: []
  note: >-
    1,000,000 x 75 kWh = 75 GWh; 1,000,000 x 20 kWh = 20 GWh; (75 - 20) / 75 = 0.733. Pack
    capacity only; not equal electric miles, fuel use or lifecycle performance. Extra engines,
    fuel systems and maintenance offset part of any material or cost saving.
- id: F31
  what: Headline metric, electric miles captured per kWh of installed battery capacity (target or measured value)
  value: null
  unit: electric miles per installed kWh per year
  label: not-found
  sources: []
  note: >-
    Metric definition is the card's working proposal: engine-off electric miles divided by
    installed (gross) battery kWh over the same period. No measured or target value exists.
- id: F32
  what: Pack size that maximizes electric miles per installed kWh among about 10, 15, 20 or 30 kWh
  value: null
  unit: kWh
  label: not-found
  sources: []
  note: >-
    Open question. Depends on the daily-driving distribution (F3), charging access and vehicle
    efficiency. No optimum claimed.
- id: F33
  what: Matched demonstration that the PHEV package beats HEVs or BEVs per kilogram of each constrained material
  value: null
  unit: electric miles or fuel avoided per kg of material
  label: not-found
  sources: [S8]
  note: >-
    None found. S8 reports chemistry shares and capacity only; capacity ratios are not mineral
    ratios (LFP avoids nickel and cobalt but uses lithium and graphite).

- id: F34
  what: Toyota electrification patents offered royalty-free under the April 2019 announcement
  value: 23740
  unit: patents (approximate)
  label: established
  sources: [S9]
  note: >-
    S9: about 23,740 patents ("nearly 24,000"), grant period through the end of 2030, contracts
    on negotiated terms; technical support is fee-based. Not evidence of current uptake.
- id: F35
  what: First-test pilot duration
  value: 90
  unit: days
  label: working-assumption
  sources: []
  note: Working test duration from the card; seasonal follow-up and larger samples needed for annual or national conclusions.
sources:
- id: S1
  type: agency-report
  title: "Summary of Travel Trends: 2022 National Household Travel Survey (FHWA-HPL-24-009)"
  publisher: Federal Highway Administration (FHWA), U.S. Department of Transportation
  date: 2024-01
  url: https://nhts.ornl.gov/assets/2022/pub/2022_NHTS_Summary_Travel_Trends.pdf
  accessed: 2026-11-25
- id: S2
  type: company
  title: "Toyota Prius Plug-in Hybrid Gets Edgier with New Nightshade Edition"
  publisher: Toyota Motor North America (Toyota Pressroom)
  date: 2025-06-16
  url: https://pressroom.toyota.com/toyota-prius-plug-in-hybrid-gets-edgier-with-new-nightshade-edition/
  accessed: 2026-11-25
- id: S3
  type: agency-report
  title: "The 2030 National Charging Network: Estimating U.S. Light-Duty Demand for Electric Vehicle Charging Infrastructure (NREL/TP-5400-85654)"
  publisher: National Renewable Energy Laboratory (now National Laboratory of the Rockies), U.S. Department of Energy
  date: 2023-06
  url: https://docs.nlr.gov/docs/fy23osti/85654.pdf
  accessed: 2026-11-25
- id: S4
  type: other
  title: "Regulatory adjustments for plug-in hybrid vehicles in Europe"
  publisher: Fraunhofer ISI, Öko-Institut and ifeu
  date: 2026-02-18
  url: https://publica-rest.fraunhofer.de/server/api/core/bitstreams/ac662473-acb6-462a-900d-b7066eb460c8/content
  accessed: 2026-11-25
- id: S5
  type: company
  title: "Do Plug-In Hybrid Owners Actually Plug In?"
  publisher: Toyota Motor North America (Toyota Pressroom)
  date: 2026-05-20
  url: https://pressroom.toyota.com/do-plug-in-hybrid-owners-actually-plug-in/
  accessed: 2026-11-25
- id: S6
  type: other
  title: "Identifying Patterns of Real-World Charging Frequency for a Sample of Plug-In Hybrid Electric Vehicles in North America (SAE 2026-01-0429)"
  publisher: SAE International
  date: 2026-04-07
  url: https://saemobilus.sae.org/papers/identifying-patterns-real-world-charging-frequency-a-sample-plug-hybrid-electric-vehicles-north-america-2026-01-0429
  accessed: 2026-11-25
- id: S7
  type: other
  title: "Real-world usage of plug-in hybrid vehicles in Europe: A 2022 update on fuel consumption, electric driving, and CO2 emissions"
  publisher: International Council on Clean Transportation (ICCT) and Fraunhofer ISI
  date: 2022
  url: https://publica.fraunhofer.de/entities/publication/f7607ab2-d7d2-42dd-80fe-2cd229fa1b51
  accessed: 2026-11-25
- id: S8
  type: agency-report
  title: "Global EV Outlook 2026: Electric vehicle batteries"
  publisher: International Energy Agency (IEA)
  date: 2026
  url: https://www.iea.org/reports/global-ev-outlook-2026/electric-vehicle-batteries
  accessed: 2026-11-25
- id: S9
  type: company
  title: "Toyota Promotes Global Vehicle Electrification by Providing Nearly 24,000 Licenses Royalty-Free"
  publisher: Toyota Motor Corporation
  date: 2019-04-03
  url: https://global.toyota/en/newsroom/corporate/27512455.html
  accessed: 2026-11-25
- id: S10
  type: company
  title: "Electrified Trailblazer: The Toyota Prius Celebrates 25 Years in the U.S."
  publisher: Toyota Motor North America (Toyota Pressroom)
  date: 2025-06-16
  url: https://pressroom.toyota.com/electrified-trailblazer-the-toyota-prius-celebrates-25-years-in-the-u-s/
  accessed: 2026-11-25
- id: S11
  type: other
  title: "Life-cycle greenhouse gas emissions from passenger cars in the European Union: A 2025 update and key factors to consider"
  publisher: International Council on Clean Transportation (ICCT)
  date: 2025-07-08
  url: https://theicct.org/publication/electric-cars-life-cycle-analysis-emissions-europe-jul25/
  accessed: 2026-11-25
- id: S12
  type: company
  title: "Why does Toyota use Atkinson cycle engines?"
  publisher: Toyota (GB) PLC, Toyota UK Magazine
  date: 2015-01-14
  url: https://mag.toyota.co.uk/toyota-use-atkinson-cycle-engines/
  accessed: 2026-11-25
- id: S13
  type: agency-report
  title: "Hybrid Electric Vehicles (Alternative Fuels Data Center)"
  publisher: U.S. Department of Energy, Alternative Fuels Data Center
  date: undated
  url: https://afdc.energy.gov/vehicles/electric-basics-hev
  accessed: 2026-11-25
- id: S14
  type: agency-report
  title: "Electric Vehicle Benefits and Considerations (Alternative Fuels Data Center)"
  publisher: U.S. Department of Energy, Alternative Fuels Data Center
  date: undated
  url: https://afdc.energy.gov/fuels/electricity-benefits
  accessed: 2026-11-25
- id: S15
  type: agency-report
  title: "Weather and other events can cause disruptions to gasoline infrastructure and supply (Today in Energy)"
  publisher: U.S. Energy Information Administration (EIA)
  date: 2013-02-01
  url: https://www.eia.gov/TodayinEnergy/detail.php?id=9811
  accessed: 2026-11-25
- id: S16
  type: company
  title: "Wallboxes and charging columns with load management"
  publisher: MENNEKES
  date: undated
  url: https://www.mennekes.org/emobility/products/load-balancing/
  accessed: 2026-11-25
- id: S17
  type: agency-report
  title: "Workplace Charging for Electric Vehicles (Alternative Fuels Data Center)"
  publisher: U.S. Department of Energy, Alternative Fuels Data Center
  date: undated
  url: https://afdc.energy.gov/fuels/electricity-charging-workplace
  accessed: 2026-11-25
provenance:
  method: ai-assisted
  editor: Idea-Shelf-Labs
  approved: 2026-11-26
post_url: https://ideashelflabs.com/posts/phev/
license: CC-BY-4.0
---

## Problem

Most private cars spend hours parked at work, overnight, at apartments, on streets and in driveways, often beside an outlet they cannot reach. Speed helps a car passing through; reliable access helps a parked one. Charging plans built around a few powerful posts buy speed that a parked car often cannot use, and sometimes cannot accept: a current plug-in hybrid's onboard charger needs about four hours on Level 2 for a full pack and about 11 hours at 120 V [F9, S2].

The vehicles have a matching imbalance. In 2025, U.S. battery-electric cars averaged about 90 kWh of battery and plug-in hybrids less than 20 kWh [F27, F28, S8]. A large pack serves the rare long day and sits partly unused on ordinary ones. A plug-in hybrid's plug and battery pay off only if owners charge. European fleet records show real-world fuel use far above test values [F16], and company cars, where someone else usually pays for fuel, reach only a small electric share [F22]. A North American manufacturer sample is more favourable [F20]. These studies judge the extra plug, not the hybrid underneath it.

The broader problem is allocation: battery capacity, outlets, feeder capacity and public money are limited, while time already spent parked goes unused. The framing here is distributed electrification: many cars with modest packs sized for regular days, refilled slowly during stays they already make, with hybrid drivetrains keeping long-distance capability, managed charging limiting electrical upgrades, and liquid fuel remaining a second energy pathway. This is not a claim that plug-in hybrids should replace battery-electric cars. Complete cost, actual energy prices, range needs and driver preference still decide the fit.

## Mechanism

The idea stacks three layers; only the first is established.

**The hybrid base.** Regenerative braking recovers some slowing energy; motor assistance, engine load management and stop/start reduce combustion fuel use without any external charge [S12, S13]. An Atkinson-cycle engine trades some peak output for efficiency, and the motor covers the lost acceleration torque [S12]. Gains depend on design and duty cycle. A plug-in hybrid keeps all of this in charge-sustaining operation, so an unplugged one has not lost the hybrid; what may fail to earn its cost is the added plug and battery.

**A modest pack sized for ordinary days.** The test starts from a band of 35 to 50 electric miles, with 40 as the test choice [F1]. Survey averages give context [F2], but no checked current distribution of vehicle-day distances says what share of days it covers [F3]. As a worked example, at 0.30 kWh per mile of battery output, 40 miles uses about 12 kWh of usable energy [F4]; with 86–92% wall-to-battery efficiency that is about 13–14 kWh at the wall [F5]. Gross pack capacity is a third, larger quantity. Refilling it takes about 9–10 hours at 1.4 kW [F6], or about four at 3.3 kW. An eight-hour stay at a steady 1.4 kW supplies roughly 80–86% of it [F7]: a partial refill, which is the design point, since the engine covers any shortfall.

**Spread access and share power.** Every space can have a standard Level 2 outlet; what limits a lot is its connection. A load-management controller measures site load and sets each car's rate so the total stays inside it [S16]. In an illustrative ten-space lot sharing one 33 kW connection, each car still gets 3.3 kW if all charge at once, more than twice the worked example's 1.4 kW, and more when fewer charge [F8]. NREL calls matching charging speed to parking time "right-speeding" [S3, pp. ix and 8]. Larger sites scale the same way [F15], but many slow ports lower peak demand only if managed. The installed cost per connection is unknown [F13], and no universal optimum share of wired stalls exists [F14].

The headline metric that ties the layers together is electric miles captured per kWh of installed battery capacity [F31]. A smaller pack that is fully used on ordinary days can be more productive than a larger pack that rarely depletes. Two illustrations show the logic without proving it. Sixty kWh split into four 15 kWh packs equips four plug-in hybrids instead of one battery-electric car; if each of the four travels the same distance as the battery-electric car (car for car, not equal total travel), the four deliver more electric miles per kWh of installed battery only if their average engine-off share exceeds 25% [F29]. At fleet scale, one million 20 kWh plug-in hybrids install about 73% less pack capacity than one million 75 kWh battery-electric cars [F30]. Both are pack capacity only, not equal electric miles, fuel use or life-cycle performance.

The trade-off is access: a smaller pack needs charging more often and depends more on finding a working outlet, while a larger one gives irregular drivers more slack. Under comparable chemistry and engineering, a smaller pack has less mass, material and cost than a larger one; that does not make the complete vehicle lighter or cheaper, because the engine, fuel system and transmission must be counted. Capacity ratios are not mineral ratios either; a smaller pack of one chemistry does not automatically save every constrained material against a larger pack of another [F33, S8].

## Proposal

### Vehicle and powertrain

Treat the moderate range band as a starting test, not the only legitimate size, and choose an efficient charge-sustaining hybrid architecture. Atkinson or Miller operation, power-split or eCVT drives and competing two-motor designs are candidates, not mandatory specifications; the card names the result it wants, an efficient charge-sustaining mode, and claims no efficiency percentage from naming an architecture [S12, S13]. Label electric range, wall energy and charge-sustaining fuel economy separately so buyers can see weak plug-in designs. There is no mandated fuel-economy floor, vendor or compulsory charging habit, and no measured effect shows that labels alone change purchasing or charging enough.

Licensing is one route, not a complete product. In April 2019 Toyota offered royalty-free licences to about 23,740 electrification patents [F34] through the end of 2030, on negotiated terms, with technical support charged separately [S9]. That does not establish current uptake, a production contract or a guaranteed efficiency gain.

Saving charge for later stop-and-go driving on a known mixed route may save fuel; that working assumption is compared with charge-first operation on matched journeys, counting engine starts for heating, safety and battery protection.

### Market choice and cost per mile

Drivers are free to choose the cheaper energy source; the test measures whether they do. Fuel cost per mile in charge-sustaining mode is the fuel price over actual charge-sustaining miles per gallon; electric cost per mile is wall kWh per mile times the price actually paid per kWh. Battery-output energy must first be divided by charging efficiency, without adding losses twice to wall-metered use. For blended travel, add actual fuel and electricity bills, including session and parking charges, before dividing by miles.

Expensive tariffs, short dwell or an employer paying for fuel can change the decision. These are marginal energy comparisons; ownership cost is a separate account (purchase minus resale, plus financing, maintenance, insurance and charging equipment over the same period and mileage, never counting both purchase price and depreciation). Price response is intended, to be measured rather than assumed.

### Parking lots

Provide working, reachable outlets with clear prices, billing and repairs; use Level 1 where dwell suits the energy needed, and shared or managed Level 2 where it does not; home charging remains an option where practical [S17]. Wiring alone is not evidence of changed behaviour. Compare only infrastructure the enrolled cars can use: an AC-only plug-in hybrid cannot test a DC arm, so DC belongs in a separate, compatible population. Shared power is still limited by circuits, phases and onboard chargers, so report completion times and coincident demand.

### Energy independence, preparedness and optional fuel capability

Useful grid-electric miles can cut ordinary petroleum demand and exposure to oil supply while keeping efficient fuel travel for longer journeys, without waiting for a perfect all-electric grid. That is diversification, not complete independence from fuel, imported resources or electricity supply [S14].

For disaster preparedness, stored fuel and battery energy are separate paths. Liquid range can still move people and critical loads when the grid is down or charging is scarce; battery energy can support electric trips when fuel access is constrained. The dual drivetrain is a resilience feature in its own right, not only a transition step. The limits are real: starting energy is not access to replenishment, shared outages can disable both chargers and fuel pumps, which themselves depend on electricity [S15], roads can fail, and a charged battery-electric car also stores energy. Dual capability does not guarantee mobility or household backup power.

For national security, less ordinary petroleum use and more than one energy route reduce exposure to fuel disruption, grid events and contested supply chains. Optional compatibility with domestically producible liquid fuels, such as flex-fuel capability, is a further layer only where compatible fuel, pumps and stockpiles exist. Capability is not supply, assured low-carbon fuel or guaranteed resilience; feedstock, land, water, seasonal blends and distribution need their own assessment. It is still a capability that cannot be added in a hurry once supply tightens. Vehicle-to-home power needs model-specific equipment and verified ratings.

### Public support

Public support should make room for efficient modest-battery plug-in hybrids and useful charging access, alongside other ways to meet the same needs. Lower cost per vehicle lets a fixed budget reach more households, but a smaller pack does not by itself set the payment or prove more fuel displaced per public dollar. Compare packages on additional electric travel and petroleum displaced per public dollar, charging access and complete-vehicle cost, against efficient hybrids and right-sized battery-electric cars. A first-40-electric-mile cap and a continuous logarithmic battery credit are different, unselected designs; payment basis, rate and eligibility remain open, and the support proposal does not make 40 miles an optimum.

## Why this, not the rival

**Against the efficient hybrid.** The non-plug-in hybrid offers the hybrid gains with no plug premium. A dated product pair shows the trade: the 2026 Prius plug-in SE has a 13.6 kWh battery [F24] and is rated up to 52 mpg in hybrid operation against 57 for the hybrid LE [F25], with a base-price gap of about $5,225 at June 2025 launch [F26, S2, S10]. That gap compares launch base prices, not matched transaction prices. An owner who rarely charges pays the premium for little. One who charges on most driving days, as in a North American manufacturer sample [F20, S5, S6], or reaches the 45–49% electric share of European private cars [F21], displaces fuel the hybrid cannot. Where charging is absent or the plug does not pay, the hybrid wins.

**Against the right-sized battery-electric car.** A battery-electric car uses the same outlets and drops the engine. An EU life-cycle model for medium cars sold in 2025 puts plug-in hybrids at 163 g CO2e/km against 63 for battery-electric and 188 for hybrids [F23, S11], using a projected EU electricity mix. That strongly favours the battery-electric car per vehicle; this package is not claimed to be inherently cleaner or cheaper. The case is allocation under constraint: per installed kWh, packs that are used daily may deliver more electric miles [F29, F30], and the pilot enrols compatible battery-electric cars to test whether the outlet pattern works for them independently.

**Against a few fast posts at the same site.** NREL's model inputs put commercial Level 2 at $4,400–10,600 per port and 150 kW DC at $112,200–196,200, equipment plus installation [F10, F11, S3]. Across those bands DC costs about 11 to 45 times as much per port [F12]. These historical inputs exclude utility upgrades, energy and demand charges and maintenance, and are not a site productivity ratio; they show why outlets per dollar can favour slow charging at long dwell, not that it does. Fast charging stays the right tool en route.

## Who gains, who loses

Drivers who park for hours gain cheaper ordinary-day miles where electricity costs less, with fuel range for long trips and no charging quota. Site owners can wire many spaces within one shared connection [F8, F15, S16], and utilities gain slow, managed load, but only if management caps coincident demand. Hybrid suppliers gain a market that rewards labelled charge-sustaining efficiency, and holders of hybrid patents can license them, as Toyota has offered [S9]; public budgets gain lower petroleum exposure if support is judged per dollar of additional electric travel.

Fast-charging providers lose some long-dwell demand but keep their en-route role. Fuel retailers see ordinary-day volumes fall gradually while long-trip demand remains. Drivers who cannot park for hours, or need long electric range, gain little and keep their battery-electric options. Taxpayers lose if support pays for purchases that would have happened anyway, so the support design is tested against a counterfactual.

Why not already? Plug-in hybrids have often gone unplugged, especially where someone else pays for fuel [F16, F22]. Site owners carry the wiring, billing and repair costs, with no defensible all-in cost per low-power connection [F13], and the party paying for the outlet is often not the one saving on fuel (this card's reasoning, not a measured finding). Price-led charging is intended rather than shown, and no chosen support design pays for additional electric travel rather than battery size.

## How we'd know

Score three comparisons separately: hybrid versus a comparable non-hybrid; plug-in hybrid versus hybrid for the extra plug and battery; and complete plug-in hybrid versus battery-electric ownership. A good charging-lot result proves none of the vehicle comparisons by itself.

- **Vehicle use:** actual fuel and wall energy, engine-off distance over total distance, CD distance reported separately, charging events per driving day and charge-sustaining fuel economy, split by private and company use, home access, route, weather and vehicle. Charging frequency is not electric-mile share, and CD distance is not engine-off distance: European fleet data show fuel burned in CD mode [F17] and a gap between CD share and engine-off share [F18, F19, S4].
- **Access and power:** working outlets, faults, conflicts, dwell, refill completion including partial refills, and actual coincident site demand. A blocked or broken port is not access.
- **Cost:** dated bids and invoices, including utility work, software, maintenance and demand charges, giving incremental electric travel per all-in dollar over a common horizon.
- **Allocation (headline):** electric miles per installed battery kWh [F31], compared across pack sizes rather than assuming a larger pack is better, plus fuel displaced per public dollar and, with a bill of materials, kilograms of each named material.

Record who pays, the actual price gap, what the driver chose and whether access blocked the cheaper choice; fuel use when electricity costs more can be rational.

The first test is a logged pilot [F35] comparing fewer, higher-power AC outlets (arm A) with more lower-power or managed AC outlets (arm B) at a comparable all-in budget, with compatible battery-electric cars and efficient hybrids enrolled for comparison and route-aware control tested separately. The card is rejected for this site class if arm A delivers equal or more useful electric travel per all-in dollar, if the plug and battery do not earn their cost against matched hybrids, or if battery-electric cars meet the same need at lower complete cost. A short pilot shows feasibility and local effects only; seasonal follow-up comes before national conclusions.

## Why it might fail

The strongest objections: the plug and battery do not earn enough service, or cheap electricity fails to attract charging; heating and control strategy burn fuel during depletion; wiring, billing and repairs make access costly or unreliable; shared power, short dwell or cold prevent the intended refill, or simultaneous demand erases the peak advantage; an efficient hybrid or right-sized battery-electric car meets the need at lower complete cost or impact; the second energy route lacks supply, or one disruption blocks both; and support pays for purchases that would have happened anyway.

Stress-testing the common shortcuts:

- *Forty miles covers ordinary life.* It is a design target, not a measured percentile or annual-coverage promise; household, driver, vehicle-day and annual denominators cannot be swapped [F1, F2, F3].
- *No charging means no hybrid benefit.* Hybrid mechanisms need no external charge; only the extra grid-electric service depends on charging [S13].
- *Drivers always choose the cheaper source.* Price response is intended, not universal; route costs, who pays, access and convenience belong in the test.
- *Battery depletion means engine-off driving.* CD operation can include fuel use; engine-off distance, CD distance, energy share and weighting definitions stay distinct, and the European figures are not divided across weightings [F17, F18, F19].
- *A small pack makes the whole car lighter and cheaper.* Only the pack saving holds; an allocation illustration is not a demonstrated national oil saving.
- *Many slow always wins.* Compare only where dwell and vehicle acceptance suit the service; reject the lot hypothesis if compatible higher-power charging wins on useful electric travel per all-in dollar.
- *A budget cap settles the support case.* A smaller pack sets neither the award nor additional travel.

What survives is distributed electrification on an efficient hybrid base: a modest pack, plentiful long-dwell access and market-led choice of energy source. Hybrid mechanisms are established; electric miles per installed kWh, pack size, price response and the value of plug, access and support remain to be scored; the claim's "best used by" is a proposal, not a proven winner.

## Open questions

- Which current vehicle-day distribution and seasonal routes justify the starting band [F3]?
- Which pack size, among about 10, 15, 20 or 30 kWh, maximizes electric miles per installed kWh for a given daily-driving distribution, charging access and vehicle efficiency [F32]? No optimum is claimed.
- What are all-in installed and operating costs per accessible low-power connection versus fewer higher-power ports at the same site [F13]?
- Who plugs in when prices and access favour it, and how do private and fleet users differ?
- Does route-aware charge allocation beat charge-first operation on matched journeys?
- Does the allocation case survive chemistry-specific material accounting, extra engines and equal-budget comparisons [F33]?
- Do labels alone produce a useful change in purchasing or charging?
- Which disruption scenarios benefit from dual energy stores once pumps, roads and starting charge or fuel are counted?
- Which support design, payment amount and eligibility best serve additional useful travel and petroleum displacement?
