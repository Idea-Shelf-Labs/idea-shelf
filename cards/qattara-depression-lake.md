---
schema: idea-shelf/card@2
id: qattara-depression-lake
title: Qattara depression lake
version: 2.0.0
updated: 2026-11-26
status:
  editorial: published
  evidence: test-specified
claim: >-
  Run as one coupled system, nuclear-heated MED, surplus-power RO, a solar-clad pipeline over the ridge, and hydro on the descent are designed to cut the net energy cost of filling a below-sea-level basin with freshwater.
summary: >-
  Egypt's Qattara Depression lies below sea level about 56 km from the Mediterranean. Instead of
  the rejected seawater schemes, this card proposes making fresh water on the coast with a nuclear
  plant's waste heat and surplus power, pumping it over the plateau, and recovering energy as it
  falls into a held freshwater lake. Gravity can roughly repay its own pumping but not
  desalination. The open questions are salt, seepage, brine, cost and whether a lake is worth it.
domains: [water, energy, agriculture, climate]
patterns: [converge-on-proven, stabilize-across-systems, growth-with-less-harm]
readiness: concept
geography: [EG]
why_not_yet: >-
  Past schemes for the depression admitted seawater for hydropower and were rejected; Egypt's
  2026 review also judged a desalinate-at-the-rim pipeline not feasible and favoured not using
  the depression as a reservoir at all [F6]. No one has modelled a coupled freshwater corridor
  (waste heat, surplus power, lift and drop) hour by hour, and the costs, the floor's salt and
  seepage, and who holds the corridor rights are all unknown [F70, F76, F82].
coalition:
  - actor: Egypt's water, electricity and planning ministries
    gains: A scored option for using coastal reactor heat and surplus power to make and store fresh water inland, tested against the risks their own 2026 review named.
  - actor: The coastal nuclear plant's owner and operator
    gains: A use for condenser heat that is otherwise discharged, on the operator's terms; no steam is taken, and any cooling-water temperature rise is theirs to allow [F14, F15].
  - actor: Farmers and settlements near the lake edge and along the corridor
    gains: Irrigation water held at about 1,000 mg/L for salt-tolerant crops, and a buffer against plant outages and dry spells [F71, F80].
  - actor: Grid operator
    gains: A flexible load (RO, heat pumps) that soaks up midday solar surplus, and a small pumped-storage pair for an evening shift [F48, F51].
boundary: >-
  Public support, if any, pays for the decisive coupled corridor model and the first field cores of
  the lake floor, not for construction. Building waits for a closed energy and salt balance, a
  brine and intake permit path, and clearance of the oil, gas and Siwa risks the 2026 review named.
resilience: >-
  Coastal water supply that depends on continuous plant output: the upper lake and the water bank
  hold months of output as a reserve for a plant outage or a dry spell [F31, F33].
losers:
  - who: Oil and gas operators on the plateau and in the review's 35 development and 8 exploration areas
    mitigation: Map the route and lake footprint against fields and pipelines first; the test fails if the footprint cannot avoid them or be cleared [F7, F8].
  - who: Siwa Oasis and the desert habitats, springs and wells near the depression
    mitigation: Seepage and salt monitoring is a pass/fail test; any rise in nearby well or groundwater salinity rejects the lake [F70].
  - who: Qara, the only permanent settlement in the depression, and Bedouin land and well users along the corridor
    mitigation: Their consent and water rights are mapped before any route is chosen; they can refuse the corridor.
  - who: Coastal marine life near the intake and brine outfall
    mitigation: Brine disposal and intake design are scored, costed and permitted before any build; the brine volume is still unknown [F27].
  - who: Taxpayers and electricity customers, if the lake costs more than piping water straight to users
    mitigation: The rival (coastal desal piped direct) sets the bar; the lake must show a value that beats it per cubic metre delivered [F82, F98].
rival:
  name: Coastal desalination piped directly to farms and towns, with no lift over the plateau and no lake
  why_not: >-
    It delivers the same fresh water with no lift, no ridge, no evaporation loss and no salt
    balance to manage. The lake version wins only if a held inland freshwater lake is worth the
    extra pipe, the evaporation make-up [F58, F98] and the risk, and if the drop repays the lift after friction [F46].
first_test:
  design: >-
    A coupled corridor model for one route, hourly over a full year: MED output from the reactor's
    usable waste heat, RO on surplus electricity only, the dispatch rule, pipe friction, pump and
    turbine efficiency, heat-pump COP checked against measured units at this lift, solar annual yield, and a water and salt balance for the lake at a stated
    size and purpose, with sensitivity runs on every range in this card. In parallel, field cores
    of the lake floor for salt-crust thickness and pore brine.
  cost_band: $100k-1M
  duration: 12 months
  success: >-
    The three energy ledgers close on the same water; the plant buys little or no outside
    electricity beyond the surplus the design assumes; the drop repays most of the lift after
    friction; and the cores support a salt balance that holds the lake near 1,000 mg/L without
    raising salinity in nearby wells or groundwater.
  kill: >-
    The corridor cannot show a lift-to-drop, a brine plan and a salt balance that support a held
    freshwater lake: hydro does not pay back most of the pumping once friction is counted, or
    purchased electricity exceeds the surplus the design assumes, or modelled seepage raises
    salinity in nearby wells or groundwater.
  kill_terms: [lift-to-drop, brine plan, salt balance, held freshwater lake]
figures:
  # Basin geography
  - id: F1
    what: Area of the Qattara Depression below sea level
    value: 19500
    unit: km2
    label: established
    sources: [S1]
    note: Ball 1933 p.290. The live post and v1 said 19,605 (source not found). S2 gives 12,500 km2 (a different outline); a 1976 NASA/ASRT Landsat report's 95,000 km2 at -60 m looks like an error and is not used.
  - id: F2
    what: Average floor depth below sea level
    value: -60
    unit: m
    label: established
    sources: [S1]
    note: Ball 1933 p.290.
  - id: F3
    what: Lowest point of the depression
    value: -134
    unit: m
    label: established
    sources: [S1, S51]
    note: Ball 1933 and Ball 1927 both give 134 m below sea level (v1 said 133). The illustrative lake's deepest DEM cell is about -136 m (F40).
  - id: F4
    what: Shortest distance from the depression to the Mediterranean
    value: 56
    unit: km
    label: established
    sources: [S1, S2]
    note: Ball 1933 p.290 and contour table p.293; S2 says about 55 km.
  # Egypt's 2026 review
  - id: F5
    what: Date the Cabinet Media Center published the ministerial committee's Qattara findings
    value: "2026-05-12"
    unit: date
    label: established
    sources: [S3, S4, S5, S6]
    note: Published 12 May 2026. Committee formed under decree 3433 of 2016; reported by four Arabic outlets.
  - id: F6
    what: Development scenarios the committee assessed (four judged not feasible; scenario 4, not using the depression as a reservoir, favoured)
    value: 5
    unit: scenarios
    label: established
    sources: [S3, S4, S5, S6]
    note: Scenario 5, closest to this card, desalinates at the rim and pipes water straight to users. Why it was judged not feasible is not published.
  - id: F7
    what: Oil production development areas the review said overlap the depression
    value: 35
    unit: areas
    label: established
    sources: [S3, S4]
  - id: F8
    what: Oil exploration areas the review said overlap the depression
    value: 8
    unit: areas
    label: established
    sources: [S3, S4]
  # Thermal ledger
  - id: F9
    what: Low-temperature MED top brine temperature
    value: 70
    unit: °C
    low: 60
    high: 70
    label: published-contested
    sources: [S7, S8]
    note: Makers give about 60-70 °C; the card designs for 65-70 °C.
  - id: F10
    what: Condenser cooling-water outlet temperature at a nuclear plant
    value: 35
    unit: °C
    low: 30
    high: 40
    label: published-contested
    sources: [S9]
    note: Typical range; condensing steam sits about 10-15 °C above the cooling water.
  - id: F11
    what: Electrical output lost per °C of warmer cooling water (PWR studies)
    value: 0.42
    unit: percent per °C
    low: 0.39
    high: 0.45
    label: published-contested
    sources: [S10, S11]
  - id: F12
    what: Cooling-water temperature rise the operator might allow
    value: null
    unit: °C
    low: 2
    high: 5
    label: not-found
    sources: []
    note: The card uses 2-5 °C for arithmetic only; the operator's limit is unknown.
  - id: F13
    what: Lift from cooling-water temperature to MED temperature
    value: 32.5
    unit: K
    low: 25
    high: 40
    label: working-assumption
    sources: []
    note: 65-70 °C (F9) minus 30-40 °C (F10).
  - id: F14
    what: Generation lost by running cooling water 2-5 °C warmer
    value: 1.5
    unit: percent of electrical output
    low: 1
    high: 2
    label: working-assumption
    sources: []
    note: 2-5 °C × 0.39-0.45 %/°C (F11) = 0.8-2.3 %, rounded to about 1-2 %.
  - id: F15
    what: No steam is taken from the plant; MED takes only condenser cooling-water heat
    value: design choice
    unit: n/a
    label: working-assumption
    sources: []
    note: Design choice so the plant's safety basis is unchanged. Taking the heat still has a cost - equipment, the operator's consent and lost generation (F14).
  - id: F16
    what: Average COP of commercial industrial heat pumps at a 61 K lift
    value: 3.3
    unit: COP
    label: established
    sources: [S13]
  - id: F17
    what: Heat-pump COP used for the 25-40 K top-up
    value: 4
    unit: COP
    low: 3
    high: 5
    label: working-assumption
    sources: [S13, S14]
    note: S14's fit of COP against lift gives about 4-5 at 25-35 K and less at 40 K; the card uses 3-5 to allow for real plants and the larger lift.
  - id: F18
    what: MED electricity use (pumps and auxiliaries)
    value: 2
    unit: kWh/m3
    low: 1.5
    high: 2
    label: published-contested
    sources: [S15]
    note: S15 text gives 1.5-2 kWh/m3, its table 2 kWh/m3. v1's 1-2.5 was not found in an opened source.
  - id: F19
    what: MED heat use
    value: 73
    unit: kWh/m3 (thermal)
    low: 50
    high: 73
    label: published-contested
    sources: [S8, S15]
    note: S15 table 1 gives 263 MJ/m3 (÷ 3.6 = 73 kWh/m3); S8 gives about 50-70 kWh(th)/m3; S15's text also quotes 4-7 kWh/m3 (an electrical equivalent). v1's 64-108 kWh/m3 was not found in an opened source.
  - id: F20
    what: Heat-pump electricity to raise all MED heat from cooling-water temperature (the design's own draw, unless other outside heat is used)
    value: 17
    unit: kWh/m3
    low: 10
    high: 24
    label: working-assumption
    sources: []
    note: 50-73 kWh heat (F19) ÷ COP 3-5 (F17). The cooling water supplies the rest of the heat (about 67-80 %). About 2-8 times RO's 3-4.5 kWh/m3 (F23), so MED makes sense only on surplus power RO can't absorb (RO makes 2-8 times more water per kWh); the MED/RO split is not modelled. v1 and the live post said 13-36.
  - id: F21
    what: A published nuclear MED+RO design to scale from (v1 cited an IAEA example, 600 MWth HTGR, about 52,000 m3/day)
    value: null
    unit: m3/day
    label: not-found
    sources: []
    note: The IAEA publication could not be opened; the example is not used.
  - id: F22
    what: Usable heat, temperature and rating of a reactor for this corridor
    value: null
    unit: MWth
    label: not-found
    sources: []
  # Electrical ledger
  - id: F23
    what: Seawater RO specific energy
    value: 3.7
    unit: kWh/m3
    low: 3
    high: 4.5
    label: published-contested
    sources: [S15]
    note: S15 table gives 3.7-4.5 kWh/m3; its text says under 3-4 kWh/m3 in recent plants. v1 and the live post said 3-5.5 (upper end not found).
  - id: F24
    what: Average electricity for 1 million m3/day of RO
    value: 155
    unit: MW
    low: 125
    high: 190
    label: working-assumption
    sources: []
    note: 1,000,000 m3 × 3-4.5 kWh/m3 (F23) ÷ 24 h.
  - id: F25
    what: Share of hours RO runs on surplus power, and the installed oversizing that implies
    value: null
    unit: percent of hours
    label: not-found
    sources: []
  - id: F26
    what: Nameplate of an illustrative solar-clad pipeline strip (70 km × 10 m at 200 W/m2)
    value: 140
    unit: MWp
    label: working-assumption
    sources: []
    note: 0.7 km2 × 200 W/m2. Nameplate, not annual yield; annual yield on a real corridor is not found.
  - id: F27
    what: MED/RO split, brine volume and outfall design
    value: null
    unit: m3/day
    label: not-found
    sources: []
  # Hydraulic ledger (illustrative route, derived from the Copernicus DEM)
  - id: F28
    what: Pipe length from the coast near El Dabaa to the upper lake
    value: 85
    unit: km
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30 along one illustrative route; one dip of about 15 m near km 78. Intake point about 31.057N 28.501E.
  - id: F29
    what: Upper lake level, site ground to full
    value: 190
    unit: m
    low: 180
    high: 190
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30 (a surface model with a few metres of error).
  - id: F30
    what: Upper-lake dam length (bed about 171.7 m, crest about 191.7 m)
    value: 3.1
    unit: km
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30; dam about 20 m high.
  - id: F31
    what: Upper lake volume when full
    value: 147
    unit: million m3
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30; area about 14.3 km2. About 98-147 days of one plant pair's output (F56), or about 54 days at 2.7 million m3/day (F58), when not cycled for storage.
  - id: F32
    what: Upper lake area when full
    value: 14.3
    unit: km2
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30.
  - id: F33
    what: Natural closed basin 9.5 km NNE of the upper lake (water bank), volume at its 155 m spill level
    value: 0.7
    unit: billion m3
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30; area about 43.6 km2; about 25-35 m below the upper lake's level (155 m against 180-190 m), so weak as a storage pair.
  - id: F34
    what: Ridge crest on the descent, about 4.1 km south of the upper lake
    value: 212
    unit: m
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30; higher than the full upper lake (190 m). For comparison, the lowest crest of the shortest coast-to-depression gap, about 55 km on the east side, is about 148 m (GLO-30); a route there is not scored.
  - id: F35
    what: Depth of the cut through the ridge
    value: 27
    unit: m
    low: 22
    high: 32
    label: working-assumption
    sources: []
    note: 212 m crest (F34) minus a full (190 m) or low (180 m) upper lake (F29). The live post and two images said 20-35 m; a 20 m cut would leave its floor above the full lake. The energy figures F44-F46 assume the cut. Not costed.
  - id: F36
    what: Net energy cost of a booster pump over the ridge instead of a cut
    value: 0.015
    unit: kWh/m3
    low: 0.01
    high: 0.02
    label: working-assumption
    sources: []
    note: The extra 22-32 m (F35) is pumped at 1/η and recovered through the same turbines at η, so only the round-trip loss is spent - 22-32 m × 0.002725 (F41) × (1/η - η), η = 0.894-0.922 (F43). Corrects v1, the live post and two images, which gave 0.09-0.10 kWh/m3 (the whole extra lift, with nothing recovered) and said it wipes out the best case. The cut is a trade between a one-time dig and about 6-15 % of the before-friction gain (F44), forever. Booster friction not included.
  - id: F37
    what: Cliff-foot level after the escarpment
    value: -71
    unit: m
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30; the fall from the upper lake is about 251-261 m (F47).
  - id: F38
    what: Run along the depression floor from the cliff foot to the lake
    value: 150
    unit: km
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30 along the illustrative route, cliff foot (F37) to the lake (F39).
  - id: F39
    what: Lake area at about -97.6 m in the southwest pocket centred near 29.35N 26.84E (the Tahoe-size goal)
    value: 490
    unit: km2
    label: working-assumption
    sources: [S17, S18]
    note: Derived from GLO-30. Lake volume about 7.2-7.3 km3 (GLO-90). Smaller stages - 180 km2 at about -116 m, 270 km2 at about -108 m (F57).
  - id: F40
    what: Deepest DEM point of the lake pocket
    value: -136
    unit: m
    label: working-assumption
    sources: [S17]
    note: Lowest DEM cell in the southwest pocket, about -135.8 m (GLO-30 averaged to about 90 m); a flat deep floor below about -125 m covers about 100 km2. A surface model with a few metres of error.
  - id: F41
    what: Energy per metre of head for one cubic metre of fresh water
    value: 0.002725
    unit: kWh/m3 per m
    label: working-assumption
    sources: []
    note: Physics, not a sourced figure. E = ρgh with ρ = 1,000 kg/m3, g = 9.81 m/s2; 9,810 J ÷ 3.6e6 J/kWh.
  - id: F42
    what: Ideal net energy from lifting to about 180 m and dropping to -97.6 m
    value: 0.266
    unit: kWh/m3
    label: working-assumption
    sources: []
    note: 97.6 m (the depth below sea level) × 0.002725 (F41); set by the lake depth alone.
  - id: F43
    what: Pump-plus-turbine round-trip efficiency, split evenly between pump and turbine
    value: 82.5
    unit: percent
    low: 80
    high: 85
    label: working-assumption
    sources: [S19]
    note: Each machine about 89.4-92.2 %. S19 gives about 80 % for new pumped-storage plants.
  - id: F44
    what: Net energy before pipe friction
    value: 0.146
    unit: kWh/m3
    low: 0.127
    high: 0.165
    label: working-assumption
    sources: []
    note: 277.6 m × 0.002725 × η minus 180 m × 0.002725 ÷ η, η = 0.894-0.922 (F43).
  - id: F45
    what: Pipe friction head loss
    value: 0.25
    unit: m per km
    low: 0.1
    high: 0.4
    label: working-assumption
    sources: []
    note: Over a route of about 250 km (F28 + descent + F38); a wide, smooth pipe sits at the low end.
  - id: F46
    what: Net energy after pipe friction
    value: -0.02
    unit: kWh/m3
    low: -0.138
    high: 0.099
    label: working-assumption
    sources: []
    note: 25-100 m of friction head (F45) taken off F44, split between the pumped and turbine legs. At best about 2-3 % of RO's energy (F23); at worst a net cost. Value is the midpoint; the range crosses zero.
  # Storage
  - id: F47
    what: Head between the upper lake and the cliff foot
    value: 256
    unit: m
    low: 251
    high: 261
    label: working-assumption
    sources: [S17]
    note: 180-190 m (F29) down to -71 m (F37).
  - id: F48
    what: Electricity delivered per million m3 released through the turbines
    value: 0.635
    unit: GWh per million m3
    low: 0.61
    high: 0.66
    label: working-assumption
    sources: []
    note: 251-261 m × 0.002725 = 685-710 MWh per million m3 before losses, × turbine 0.894-0.922 (F43).
  - id: F49
    what: Daily storage throughput assumed
    value: 1.25
    unit: million m3/day
    low: 1
    high: 1.5
    label: working-assumption
    sources: []
    note: Sized to one plant pair's daily output (F56).
  - id: F50
    what: Electricity pumped in per day for the storage cycle
    value: 0.95
    unit: GWh/day
    low: 0.75
    high: 1.2
    label: working-assumption
    sources: []
    note: 685-710 MWh per million m3 ÷ pump 0.894-0.922 × 1-1.5 million m3/day (F49).
  - id: F51
    what: Electricity back out per day from the storage cycle
    value: 0.8
    unit: GWh/day
    low: 0.6
    high: 1.0
    label: working-assumption
    sources: []
    note: F48 × F49.
  - id: F52
    what: Round-trip efficiency of new pumped-storage plants (US DOE)
    value: 80
    unit: percent
    label: established
    sources: [S19]
  - id: F53
    what: Electricity from draining the whole upper lake once
    value: 93
    unit: GWh
    low: 90
    high: 97
    label: working-assumption
    sources: []
    note: 147 million m3 (F31) × 0.61-0.66 GWh per million m3 (F48). Takes months at the daily flow; not a daily figure.
  # Lake sizing and evaporation
  - id: F54
    what: Lake Tahoe surface area (comparison for the lake goal)
    value: 490
    unit: km2
    label: established
    sources: [S18]
  - id: F55
    what: Freshwater evaporation rate used for the lake
    value: 5.5
    unit: mm/day
    low: 4.0
    high: 5.5
    label: published-contested
    sources: [S1]
    note: Ball 1933 pp.295-296 - fresh water 5.5 mm/day, saturated brine 2.8; averages over a lake's first 100 years 4.0-4.6 mm/day (for a seawater lake turning saline). The card uses 5.5 for a lake held fresh. A rate measured for this basin is not found.
  - id: F56
    what: Average delivered output of one large MED+RO plant pair
    value: 1.25
    unit: million m3/day
    low: 1.0
    high: 1.5
    label: working-assumption
    sources: [S22, S23, S24]
    note: From reference plants - Taweelah RO about 909,000 m3/day (S22), Sorek 2 RO about 670,000 m3/day (S23), Jubail MED about 800,000 m3/day and Ras Al Khair hybrid about 1,036,000 m3/day (S24). Installed size would be larger (F25).
  - id: F57
    what: Lake area one plant pair can hold against evaporation alone (first step)
    value: 225
    unit: km2
    low: 180
    high: 270
    label: working-assumption
    sources: []
    note: 1.0-1.5 million m3/day (F56) ÷ 5,500 m3/day per km2 (F55), with no seepage and nothing drawn off. Levels about -116 m and -108 m (GLO-30).
  - id: F58
    what: Make-up water to hold the 490 km2 lake against evaporation
    value: 2.7
    unit: million m3/day
    label: working-assumption
    sources: []
    note: 490 km2 (F39) × 5,500 m3/day per km2 (F55); about 1 km3 a year. More if the bed seeps or water is drawn off.
  - id: F98
    what: Share of the lake's desalinated inflow lost to evaporation, and the farmland the same water could irrigate if piped direct
    value: 98
    unit: percent of inflow
    low: 97
    high: 99
    label: working-assumption
    sources: []
    note: 1 minus the 1-3 % bleed (F68). The bleed waters about 1,250-6,000 feddan (10-30 million m3 a year at 5,000-8,000 m3 per feddan); the same 1 km3 a year piped direct would water about 125,000-200,000 feddan; at the same water duty that is 33-100 times the bleed's area (1 ÷ 1-3 %). This is the rival's strongest number.
  - id: F59
    what: Large plant pairs needed for the 490 km2 goal
    value: 2.5
    unit: plant pairs
    low: 2
    high: 3
    label: working-assumption
    sources: []
    note: 2.7 million (F58) ÷ 1.0-1.5 million m3/day (F56). The early-years bleed (F80), about 0.93 million m3/day, is extra and not counted here.
  - id: F60
    what: Site area of Sorek 2, a large RO plant
    value: 9.4
    unit: ha
    label: established
    sources: [S25]
  # Retention and salt
  - id: F61
    what: Freshwater upper limit (USGS) and the lake's salinity target
    value: 1000
    unit: mg/L
    label: established
    sources: [S26]
    note: USGS classes fresh water as under 1,000 ppm and slightly saline as 1,000-3,000 ppm. Holding the lake at the limit is a working assumption.
  - id: F62
    what: Full-yield irrigation-water limit, tolerant crops (barley, cotton, sorghum, sugar beet, wheat)
    value: 3000
    unit: mg/L
    low: 2560
    high: 3390
    label: established
    sources: [S27]
    note: FAO Paper 29 Table 4, ECw at 100 % yield × 640 - barley 5.3 dS/m (3,390), cotton 5.1 (3,260), sugar beet 4.7 (3,010), sorghum 4.5 (2,880), wheat 4.0 (2,560).
  - id: F63
    what: Full-yield irrigation-water limit, date palm and tomato
    value: 1410
    unit: mg/L
    low: 1090
    high: 1730
    label: established
    sources: [S27]
    note: Date palm about 1,730; tomato about 1,090 (FAO ECw × 640).
  - id: F64
    what: Full-yield limit, crops losing up to about a tenth of yield at 1,000 mg/L (maize, orange, grapefruit, alfalfa, potato, grape)
    value: 700
    unit: mg/L
    low: 640
    high: 830
    label: established
    sources: [S27]
    note: FAO Table 4, ECw × 640 - maize 1.1 dS/m (700), orange 1.1 (700), grapefruit 1.2 (770), alfalfa 1.3 (830), potato 1.1, grape 1.0 (640). At 1,000 mg/L (about 1.6 dS/m) each is below its 90 %-yield limit.
  - id: F65
    what: Full-yield limit, sensitive crops (beans, carrots, onions)
    value: 480
    unit: mg/L
    low: 450
    high: 510
    label: established
    sources: [S27]
    note: FAO ECw 0.7-0.8 dS/m × 640.
  - id: F66
    what: Salinity of the lake feed (MED distillate or two-pass RO permeate)
    value: 20
    unit: mg/L
    low: 5
    high: 30
    label: published-contested
    sources: [S28, S29]
    note: Distillate about 20-30 (S28); second-pass RO about 5-13 (S28, S29).
  - id: F67
    what: Extra desalinated water needed with single-pass RO permeate (200-400 mg/L) to hold the same lake
    value: 40
    unit: percent
    label: working-assumption
    sources: []
    note: Salt balance at 1,000 mg/L; costs more energy than a second pass at about 0.1-0.3 kWh/m3 (working assumption).
  - id: F68
    what: Bleed needed to hold the lake at 1,000 mg/L, desalinated feed only
    value: 2
    unit: percent of inflow
    low: 1
    high: 3
    label: working-assumption
    sources: []
    note: Steady-state salt balance; about 10-30 million m3 a year at 2.7 million m3/day of evaporation.
  - id: F69
    what: Bleed with the Nile option (about 0.45 km3 a year of Nile water)
    value: 11.5
    unit: percent of inflow
    low: 11
    high: 12
    label: working-assumption
    sources: []
    note: Up to about 135 million m3 a year.
  - id: F70
    what: Measured evaporation, leakage and salt dissolution for a freshwater lake on this floor
    value: null
    unit: m3/day
    label: not-found
    sources: [S1, S30]
    note: Ball 1933 p.291 describes a floor of Miocene sands, gravels, clays and limestones, with about 5,800 km2 of sabkha. The Moghra aquifer (Lower Miocene sand and sandstone with shale) is pumped for reclamation (about 445 wells) and discharges naturally into the depression (S30), so a lake on the floor sits on the aquifer's outlet. Ball 1933 places Siwa's principal village within about 80 km of the depression's western end.
  - id: F71
    what: Salt-tolerant edge-farm zone watered by the bleed
    value: 110
    unit: km2
    label: working-assumption
    sources: []
    note: About 26,000 feddan. At steady state the desalinated-only bleed (F68) waters about 1,250-6,000 feddan at 5,000-8,000 m3 per feddan a year; with the Nile option's bleed (F69) up to about 27,000, which fills the zone.
  - id: F72
    what: Farm drainage sent to the salt cell (leaching fraction)
    value: 20
    unit: percent of water applied
    low: 15
    high: 25
    label: working-assumption
    sources: []
    note: Typical leaching fraction; the salt cell receives about 4-7 times less water than a direct bleed.
  - id: F73
    what: Salt cell (natural low salt flat at the lake's northeast end)
    value: 50
    unit: km2
    low: 47
    high: 54
    label: working-assumption
    sources: [S17]
    note: Derived from GLO-30. Cell floor about -99 to -98 m. Closed by a dike about 1 km long and 2 m high (DEM gives about 0.8 km, at most about 2.1 m) with a gravity gate; the outlet draws off the bottom of the deep sump.
  - id: F74
    what: Reserve pit south of the lake
    value: 127
    unit: million m3
    label: working-assumption
    sources: [S17]
    note: About 19-22 km2, floor about -109 m, behind a natural ridge about 14 m high. Bermed evaporation pans of up to about 368 km2 for the high-Nile case.
  - id: F75
    what: Salt in each centimetre of floor crust under 490 km2
    value: 10.6
    unit: million t per cm
    label: working-assumption
    sources: []
    note: 490 km2 × 0.01 m × 2,160 kg/m3 (solid halite). About 1,450 mg/L if mixed into the 7.2-7.3 km3 lake.
  - id: F76
    what: Thickness of the salt crust under the lake
    value: null
    unit: cm
    label: not-found
    sources: []
  - id: F77
    what: Time to flush a crust of up to about 10 cm
    value: 4.5
    unit: months
    low: 3
    high: 6
    label: working-assumption
    sources: []
    note: 2-4 cycles of about 45 days at 85 % brine recovery (both working assumptions), collecting brine in the stage below about -120 m (about 159 km2, about 0.9 km3 of room). v1 and the live post said 3-8 months.
  - id: F78
    what: Flush water needed
    value: 0.495
    unit: km3
    low: 0.24
    high: 0.75
    label: working-assumption
    sources: []
    note: About 5 months to 2 years of one plant pair (F56), or about 3-9 months at 2.7 million m3/day (F58); or a Nile-surplus year.
  - id: F79
    what: Energy to pump flush brine to the salt cell, once
    value: 55
    unit: GWh
    low: 18
    high: 91
    label: working-assumption
    sources: []
    note: 0.24-0.75 km3 (F78) × 25-40 m of lift × 0.002725 kWh/m3 per m (F41) ÷ pump efficiency about 0.9. v1 and the live post said 55-190 GWh, which could not be reproduced. 10 cm of crust settles about 1.0-1.4 m thick on the cell.
  - id: F80
    what: Early-years lake salinity while pore brine diffuses out of the floor
    value: 2250
    unit: mg/L
    low: 1500
    high: 3000
    label: working-assumption
    sources: []
    note: Simple diffusion model at an assumed 0.3 million t of salt a year from the floor - about 1,300-3,300 mg/L peaking around years 12-16 with a bleed of about 340 million m3 a year, more than the edge farms can use (excess to the pans). Settling near 1,000 mg/L takes decades, about 30 years in the slow case. Until then the lake is slightly saline by the USGS classes (F61), not fresh. Diffusion rate and brine depth are not found.
  # Money
  - id: F81
    what: A published cost study that transfers to a nuclear-solar MED+RO corridor like this one
    value: null
    unit: USD/m3
    label: not-found
    sources: []
    note: v1 cited Weiner et al. (0.45 vs 0.75 USD/m3) and Hassabou et al. 2013; neither could be opened, so neither is used.
  - id: F82
    what: Capital, operating and water cost of a Qattara corridor; land, right-of-way and interconnection costs
    value: null
    unit: USD
    label: not-found
    sources: []
  # Comparisons (other systems, for scale only)
  - id: F83
    what: Colorado River Aqueduct total lift through five pumping plants (242 miles, in service since 1941)
    value: 1617
    unit: ft
    label: established
    sources: [S33]
    note: About 490 m; about 390 km.
  - id: F84
    what: Energy to deliver Colorado River water by the aqueduct
    value: 2000
    unit: kWh per acre-foot
    label: established
    sources: [S34]
    note: About 1.6 kWh/m3.
  - id: F85
    what: State Water Project single lift at the Tehachapi Mountains
    value: 1926
    unit: ft
    label: established
    sources: [S35]
    note: About 590 m.
  - id: F86
    what: State Water Project energy from the Delta to the end of the East Branch, net of its own hydro
    value: 3236
    unit: kWh per acre-foot
    label: established
    sources: [S35]
    note: About 2.6 kWh/m3.
  # Nile feed: future option, outside the scored design (derived from GLO-30 and GLO-90)
  - id: F87
    what: Nile volume a surplus-year feed might take
    value: 0.3
    unit: km3/yr
    low: 0.1
    high: 0.5
    label: working-assumption
    sources: []
    note: Surplus years only, water Egypt's planners judge spare after existing users. About 3-16 m3/s averaged over a year.
  - id: F88
    what: Nile flow reaching the sea, 1970s falling to the 1990s
    value: 3.95
    unit: km3/yr
    low: 1.7
    high: 6.2
    label: established
    sources: [S36]
    note: About 6.2 km3 a year at first, about 1.7 by the 1990s.
  - id: F89
    what: How often the Nile has a surplus year
    value: null
    unit: years per decade
    label: not-found
    sources: []
  - id: F90
    what: Dissolved salt in the Nile at the Delta head
    value: 200
    unit: mg/L
    low: 173
    high: 240
    label: published-contested
    sources: [S37]
    note: S37 (report dated 2003) tables 2-5 and 2-6 - about 173 mg/L at El-Kanater (EEAA data, 2002) and 240 mg/L at the Delta Barrage (NWRC, February 2001). The live post said "a 2001 survey".
  - id: F91
    what: Saddle every Nile route must cross, northeast of Moghra near 30.49N 29.51E
    value: 110.5
    unit: m
    low: 110.5
    high: 114
    label: working-assumption
    sources: [S17]
    note: GLO-30 gives 110.5 m; GLO-90 about 111-114 m. Direct crossings from Fayoum, Minya or Assiut top out at about 150-200 m.
  - id: F92
    what: Route B (Delta head near Qanater, north of Wadi El Natrun) length
    value: 507
    unit: km
    label: working-assumption
    sources: [S17]
    note: About 221 km on the pumped side; lift about 100-106 m; descent about 208 m through about 5 hydro steps. The Amreya route is about 397 km but takes canal water mixed with farm drainage. Dropping into Wadi El Natrun (floor about -21 m) adds about 126 m of lift. A gravity-only version needs a tunnel or cut of about 125-130 km. Route C (dropping into the wadi and pumping out) is about 510 km; a clean feeder from the Delta head to Amreya would add about 160 km of gravity canal (map in the post).
  - id: F93
    what: Net energy of the Nile feed as an open canal
    value: 0.105
    unit: kWh/m3
    low: 0.05
    high: 0.16
    label: working-assumption
    sources: []
    note: Pumping 0.33-0.39, hydro steps return 0.44-0.49; pump and turbine each 89-92 %, canal friction 0.05-0.10 m per km. As a pressure pipe (0.1-0.4 m per km) -0.36 to +0.09. Amreya - +0.08 to +0.18 (canal), -0.23 to +0.12 (pipe). Canal evaporation about 20-25 million m3 a year (20 m wide, 2-2.5 m/yr).
  - id: F94
    what: Wadi El Natrun branch reach and drip-irrigated area
    value: 16500
    unit: feddan
    low: 8000
    high: 25000
    label: working-assumption
    sources: []
    note: Lined branch of about 18-20 km after the first lift, capped at about 20 % of each year's surplus; no-farm buffer about 2.5 km around the wadi floor; avoids the monasteries (S41). Costs about 0.1 kWh/m3 of branch water (never drops through the hydro steps).
  - id: F95
    what: Wadi El Natrun aquifer over-abstraction
    value: 106
    unit: million m3/yr
    label: established
    sources: [S39]
    note: Water levels down about 5 m in a decade (S40).
  - id: F96
    what: Salt the Nile feed would add to the main lake each year without an outlet
    value: 9
    unit: mg/L per year
    low: 2
    high: 16
    label: working-assumption
    sources: []
    note: 0.1-0.5 km3 at 170-240 mg/L into a 7.2-7.3 km3 lake. Even Lake Nasser water carries roughly 150 mg/L.
  - id: F97
    what: Nile suspended sediment
    value: 50
    unit: ppm
    label: published-contested
    low: 50
    high: 50
    sources: [S42]
    note: Preprint; single value.
sources:
  - {id: S1, type: peer-reviewed, title: "The Qattara Depression of the Libyan Desert and the possibility of its utilization for power-production (Ball), The Geographical Journal 82(4)", publisher: Royal Geographical Society, date: 1933-10, url: "https://archive.org/details/sim_geographical-journal_1933-10_82_4", accessed: 2026-11-26}
  - {id: S2, type: agency-report, title: "Joint Egypt/United States report on Egypt/United States cooperative energy assessment, vol. 4 (OSTI 6164049)", publisher: US Department of Energy, date: 1979-04, url: "https://www.osti.gov/biblio/6164049", accessed: 2026-11-26}
  - {id: S3, type: news, title: "Egypt Cabinet review of the Qattara Depression development scenarios (Cabinet Media Center infographics, 12 May 2026), as reported", publisher: Al-Ahram Gate, date: 2026-05-12, url: "https://gate.ahram.org.eg/News/5643584.aspx"}
  - {id: S4, type: news, title: "Cabinet Media Center findings on the Qattara Depression, as reported", publisher: El Watan, date: 2026-05-12, url: "https://www.elwatannews.com/news/details/8282914"}
  - {id: S5, type: news, title: "Cabinet Media Center findings on the Qattara Depression, as reported", publisher: El Sabah, date: 2026-05-12, url: "https://elsabahnews.com/430954/"}
  - {id: S6, type: news, title: "Cabinet Media Center findings on the Qattara Depression, as reported", publisher: Al-Wafd, date: 2026-05-12, url: "https://www.alwafd.news/5872176"}
  - {id: S7, type: company, title: Multiple Effect Distillation (MED), publisher: Veolia Water Technologies, date: 2026, url: "https://www.veoliawatertechnologies.com/en/technologies/multiple-effect-distillation-med"}
  - {id: S8, type: company, title: Multi Effect Distillation, publisher: AquaSwiss, date: 2026, url: "https://aquaswiss.eu/desalination-solutions/multi-effect-distillation/"}
  - {id: S9, type: peer-reviewed, title: "Condenser cooling-water conditions at Gulf-region nuclear power plants", publisher: Nuclear Engineering and Technology, date: 2015, url: "https://www.sciencedirect.com/science/article/pii/S1738573315300814"}
  - {id: S10, type: peer-reviewed, title: "Influence of cooling water temperature on the efficiency of a pressurized-water reactor nuclear-power plant (Durmayaz & Sogut)", publisher: International Journal of Energy Research, date: 2006, url: "https://onlinelibrary.wiley.com/doi/10.1002/er.1186"}
  - {id: S11, type: peer-reviewed, title: "Effects of cooling water temperature on PWR power plant output (Ibrahim et al.)", publisher: Hindawi, date: 2014, url: "https://doi.org/10.1155/2014/793908"}
  - {id: S13, type: peer-reviewed, title: "High temperature heat pumps - market overview, state of the art, research status, refrigerants, and application potentials (Arpagaus et al.)", publisher: Energy, date: 2018, url: "https://doi.org/10.1016/j.energy.2018.03.166"}
  - {id: S14, type: peer-reviewed, title: High-Temperature Heat Pumps for Industrial Use, publisher: Chemie Ingenieur Technik, date: 2023, url: "https://doi.org/10.1002/cite.202300241"}
  - {id: S15, type: peer-reviewed, title: "Recent progress in renewable energy based-desalination in the Middle East and North Africa MENA region (Sayed et al.), Journal of Advanced Research 48", publisher: Elsevier / PMC, date: 2022-09-13, url: "https://pmc.ncbi.nlm.nih.gov/articles/PMC10248802/", accessed: 2026-11-26}
  - {id: S17, type: dataset, title: "Copernicus DEM - Global and European Digital Elevation Model (GLO-30 and GLO-90)", publisher: Copernicus Data Space Ecosystem, date: 2021, url: "https://dataspace.copernicus.eu/explore-data/data-collections/copernicus-contributing-missions/collections-description/COP-DEM", accessed: 2026-11-26}
  - {id: S18, type: other, title: Tahoe facts and trivia, publisher: UC Davis Tahoe Environmental Research Center, date: 2026, url: "https://tahoe.ucdavis.edu/tahoe-facts-and-trivia"}
  - {id: S19, type: agency-report, title: "Technology Strategy Assessment: Pumped Storage Hydropower", publisher: US Department of Energy, date: 2023, url: "https://www.energy.gov/sites/default/files/2023-07/Technology%20Strategy%20Assessment%20-%20Pumped%20Storage%20Hydropower_0.pdf"}
  - {id: S22, type: company, title: Taweelah RO Desalination IWP, publisher: ACWA Power, date: 2026, url: "https://acwapower.com/en/what-we-do/projects/taweelah-ro-desalination-iwp/"}
  - {id: S23, type: company, title: Sorek II Desalination Plant, publisher: IDE Technologies, date: 2026, url: "https://ide-tech.com/en/project/sorek-b-desalination-plant/"}
  - {id: S24, type: industry-report, title: "Ten of the world's largest desalination plants", publisher: Aquatech, date: 2019, url: "https://www.aquatechtrade.com/water-stories/desalination/worlds-largest-desalination-plants"}
  - {id: S25, type: industry-report, title: "Water Desalination Report, vol. 61 no. 14 (7 April 2025)", publisher: Water Desalination Report, date: 2025, url: "https://ultressa.com/wp-content/uploads/2025/11/wdr2025-14.pdf"}
  - {id: S26, type: agency-report, title: Saline Water and Salinity, publisher: USGS Water Science School, date: 2026, url: "https://www.usgs.gov/special-topics/water-science-school/science/saline-water-and-salinity"}
  - {id: S27, type: agency-report, title: "Water Quality for Agriculture, FAO Irrigation and Drainage Paper 29 Rev. 1 (Ayers & Westcot)", publisher: FAO, date: 1985, url: "https://www.fao.org/4/t0234e/T0234E03.htm", accessed: 2026-11-26}
  - {id: S28, type: other, title: Composition of Desalinated Water, publisher: DESWARE (Encyclopedia of Desalination and Water Resources), date: 2026, url: "https://www.desware.net/sample-chapters/D02/D13-002.pdf"}
  - {id: S29, type: industry-report, title: "World's First Large Full Triple-Pass RO Seawater Desalination Plant, Technical Review vol. 46 no. 1", publisher: Mitsubishi Heavy Industries, date: 2009, url: "https://www.mhi.com/technology/review/sites/g/files/jwhtju2326/files/tr/pdf/e461/e461012.pdf"}
  - {id: S30, type: peer-reviewed, title: "Management of groundwater abstraction and seawater intrusion in the Moghra aquifer, Egypt (Armanuos et al.), Scientific Reports 15:30385", publisher: Springer Nature / PMC, date: 2025-08-19, url: "https://pmc.ncbi.nlm.nih.gov/articles/PMC12365243/", accessed: 2026-11-26}
  - {id: S33, type: agency-report, title: "Fact Sheet: The Colorado River Aqueduct", publisher: Metropolitan Water District of Southern California, date: 2021-07, url: "https://www-admin.mwdh2o.com/media/ja5k5pcu/cra_fact-sheet-2021.pdf", accessed: 2026-11-26}
  - {id: S34, type: other, title: "Wilkinson et al., ACEEE Summer Study on Energy Efficiency in Buildings, panel 12 paper 14", publisher: ACEEE, date: 2006, url: "https://www.aceee.org/wp-content/uploads/proceedings-1980-2020/2006/SS06_Panel12_Paper14.pdf"}
  - {id: S35, type: agency-report, title: "California's Water-Energy Relationship, CEC-700-2005-011-SF", publisher: California Energy Commission, date: 2005, url: "https://cawaterlibrary.net/wp-content/uploads/2017/05/Californias-Water-Energy-Relationship.pdf"}
  - {id: S36, type: other, title: "Use and productivity of Egypt's Nile water (Molden, el Kady and Zhu), USCID 14th Technical Conference, Phoenix", publisher: U.S. Committee on Irrigation and Drainage, date: 1998-06, url: "https://hdl.handle.net/10217/210814"}
  - {id: S37, type: agency-report, title: "Nile River Water Quality Management Study, Report No. 67", publisher: Ministry of Water Resources and Irrigation / USAID Egypt Water Policy Reform, date: 2003-06, url: "https://cpb-eu-w2.wpmucdn.com/sites.aub.edu.lb/dist/e/139/files/2017/03/Nile-RIver-Water-Quality-Management-Study-1.pdf", accessed: 2026-11-26}
  - {id: S39, type: peer-reviewed, title: "Numerical Simulation of Groundwater Flow and Vulnerability in Wadi El-Natrun Depression", publisher: Journal of the Geological Society of India, date: 2018, url: "https://doi.org/10.1007/s12594-018-0986-7"}
  - {id: S40, type: peer-reviewed, title: "Hydrogeochemical characterization and recharge dynamics, Northwestern desert of Egypt", publisher: Environmental Earth Sciences, date: 2026, url: "https://link.springer.com/article/10.1007/s12665-026-12815-6"}
  - {id: S41, type: agency-report, title: "Tentative List 1827: The monasteries of the Arab Desert and Wadi Natrun", publisher: UNESCO World Heritage Centre, date: 2026, url: "https://whc.unesco.org/en/tentativelists/1827/"}
  - {id: S42, type: other, title: Nile sediment (preprint), publisher: Authorea, date: 2022, url: "https://doi.org/10.22541/au.166852645.57451569/v1"}
  - {id: S43, type: peer-reviewed, title: "Toshka lakes (Remote Sensing 11(2):158)", publisher: MDPI, date: 2019, url: "https://doi.org/10.3390/rs11020158"}
  - {id: S44, type: agency-report, title: "Earthshots: The lakes form (Toshka)", publisher: USGS EROS, date: 2026, url: "https://eros.usgs.gov/earthshots/the-lakes-form"}
  - {id: S45, type: peer-reviewed, title: "Dazo et al. 1966, snail hosts of schistosomiasis in Egypt", publisher: Bulletin of the World Health Organization (PMC2476091), date: 1966, url: "https://pmc.ncbi.nlm.nih.gov/articles/PMC2476091/"}
  - {id: S46, type: peer-reviewed, title: "Schistosomiasis snail hosts and water hyacinth in Nile canals (PMID 10605512)", publisher: PubMed, date: 1999, url: "https://pubmed.ncbi.nlm.nih.gov/10605512/"}
  - {id: S47, type: other, title: Wadi El Natrun Important Bird Area factsheet, publisher: BirdLife International DataZone, date: 2026, url: "https://datazone.birdlife.org/site/factsheet/6197-wadi-el-natrun"}
  - {id: S48, type: other, title: Egyptian Upstream Gateway Western Desert flyer, publisher: Egyptian Ministry of Petroleum and Mineral Resources, date: 2026, url: "https://eug.petroleum.gov.eg/dp/jsp/assets/docs/EvG_WD_Phase1_Flyers.pdf"}
  - {id: S49, type: news, title: "Khalda Petroleum achieves 15 oil discoveries in H1 FY2025/26", publisher: Zawya, date: 2026, url: "https://www.zawya.com/en/economy/north-africa/egypt-khalda-petroleum-achieves-15-oil-discoveries-in-h1-fy202526-344511"}
  - {id: S50, type: news, title: "Egypt's president opens New Delta project to grow wheat in desert with artificial river", publisher: The National, date: 2026-05-17, url: "https://www.thenationalnews.com/news/mena/2026/05/17/egypts-president-opens-new-delta-project-to-grow-wheat-in-desert-with-artificial-river/"}
  - {id: S51, type: peer-reviewed, title: "Problems of the Libyan Desert (Ball), The Geographical Journal 70", publisher: Royal Geographical Society, date: 1927-07, url: "https://archive.org/details/sim_geographical-journal_1927-07_70_1", accessed: 2026-11-26}
terms:
  Qattara Depression: The below-sea-level basin in northwestern Egypt (Matruh Governorate), Western Desert; the classic candidate site, not a locked one.
  MED: Multi-effect distillation, thermal desalination driven by low-grade heat.
  RO: Reverse osmosis, membrane desalination driven by electricity.
  Lift-to-drop: How high the water must be pumped compared with how far it can fall into the basin; scored after pump, turbine and friction losses.
  Corridor: One coastal desalination plant, one pipeline route, one receiving basin.
  First build: One reactor-class heat and power source, one corridor, one basin.
  Seawater scheme: Historical proposals (Penck, Ball, Bassler) that admit Mediterranean seawater for hydropower, ending hypersaline or as a salt pan; rejected in 2026. This card is the other path.
  Three ledgers: The thermal (MED heat), electrical (RO, pumps) and hydraulic (lift, drop, friction) energy accounts, kept separate and closed on the same water.
  Bleed: Water deliberately drawn off the lake (to edge farms, then a salt cell) to carry salt out; seepage does not count.
  Pore brine: Salty water held in the sediment below the salt crust.
  Feddan: Egyptian area unit, about 0.42 ha.
related: []
post_url: https://ideashelflabs.com/posts/qattara/
provenance:
  method: ai-assisted
  editor: Idea-Shelf-Labs
  approved: 2026-11-26
license: CC-BY-4.0
---

## Problem

Northwestern Egypt holds a basin that lies below sea level over about 19,500 km² [F1], with an
average floor about 60 m below sea level [F2] and a low point near -134 m [F3], about 56 km from
the Mediterranean [F4]. For a century the proposals for it were seawater schemes: admit the sea,
run turbines on the drop, let evaporation hold a level. They end as a hypersaline lake or a salt
pan. Egypt's 2026 review rejected seawater filling, judged four of five scenarios not feasible,
including a desalinate-at-the-rim pipeline (scenario 5), and favoured not using the depression as
a reservoir at all [F5, F6]. It named seepage into groundwater and wells, saltier soil, harm to
desert ecosystems including Siwa Oasis, overlap with 35 oil development and 8 exploration areas
[F7, F8], mineral sites, pipelines, the cost of a canal from the sea, and hydropower costing more than other
power sources [S3, S4, S5, S6].

Fresh water is the scarce good inland. Making it at the coast costs energy, and moving it over a
plateau costs more. Without recovery on the descent, the lift is a pure loss. Without a scored
brine and intake plan, coastal desalination is an unfinished plant. This card asks whether the
depression's depth can work for a freshwater lake instead of against it, and what it would take
to keep that lake fresh.

## Mechanism

Three separate energy ledgers, closed on the same water.

**Thermal.** A coastal nuclear plant discharges condenser cooling water at about 30-40 °C [F10].
MED needs about 65-70 °C [F9]. The design takes no steam [F15]; MED takes the cooling-water heat,
possibly run 2-5 °C warmer if the operator allows [F12], at a cost of about 1-2 % of output
[F11, F14]. Heat pumps on midday solar surplus lift it the remaining 25-40 K [F13] at a COP of
3-5 [F16, F17]. MED uses about 1.5-2 kWh/m³ of electricity and 50-73 kWh/m³ of heat [F18, F19].
The heat pumps deliver all of MED's heat; the cooling water supplies most of it and electricity the
rest, about 10-24 kWh/m³ of electricity [F20]. That is more than RO's 3-4.5 kWh/m³ [F23], so MED
earns its place only by turning two otherwise wasted inputs into water - rejected cooling heat and midday solar power the grid would curtail and RO can't absorb - and the MED/RO split is a
sizing question [F27]. It is cheap
heat, not free heat [F14, F15]. No opened source gives a nuclear MED+RO design to scale from [F21]; the reactor for this corridor
is not chosen [F22].

**Electrical.** RO runs on surplus electricity when it is abundant, at 3-4.5 kWh/m³ [F23]; every
million m³/day needs about 125-190 MW on average [F24], and more installed because it runs only
part of the day [F25]. A solar-clad pipeline adds nameplate, about 140 MWp for an illustrative
strip [F26]; annual yield is not found.

**Hydraulic.** One metre of head is worth about 0.002725 kWh per m³ [F41]. Lift to about 180 m,
drop to about -97.6 m, and the ideal net gain is about 0.266 kWh/m³ [F42], set by the lake's
depth below sea level. With an 80-85 % pump-turbine round trip [F43] the net is 0.127-0.165
kWh/m³ before friction [F44]; with 0.1-0.4 m per km of friction [F45] over about 250 km it spans
+0.099 to -0.138 kWh/m³ [F46]. Gravity can roughly repay its own pumping. At best it leaves about
2-3 % of RO's energy; it does not pay for desalination. Whole-system energy neutrality is not
claimed. The test target is low purchased power: the plant buys little or no outside electricity
because solar and reactor surplus cover the load.

Systems that pump water uphill and keep it there spend that energy for good: the Colorado River
Aqueduct lifts 1,617 ft [F83] at about 2,000 kWh per acre-foot [F84]; the State Water Project
lifts 1,926 ft in one step [F85] and spends about 3,236 kWh per acre-foot to the end of its East
Branch [F86]. Here the water ends lower than it started, so the lift can be paid back.

## Proposal

### Coast

One hybrid plant near El Dabaa (illustrative site, chosen only to score the idea; no endorsement
by the plant or its owners): MED on condenser heat, RO on surplus power, sharing the plant's
intake and outfall if allowed. An hourly dispatch rule runs the reactor steady, sends midday
solar surplus to heat pumps and RO, and evening power to the grid. Brine and intake ecology are
first-class design [F27]. Large plants need hectares, not square kilometres [F60].

### Route

An illustrative route, derived from the Copernicus DEM and not surveyed [S17]: about 85 km of
pipe inland [F28] to an upper lake at 180-190 m [F29] behind a 3.1 km dam [F30], holding about
147 million m³ over 14.3 km² [F31, F32]. A natural closed basin nearby holds about 0.7 billion m³
as a water bank [F33]. A ridge at about 212 m sits 4.1 km south of the upper lake [F34]: the route
needs a cut 22-32 m deep [F35] or a booster pump. Water boosted over the ridge falls back through the
same turbines, so a booster loses only about 0.01-0.02 kWh/m³ [F36]; the cut is a cost trade, not a
must, and the energy figures assume it. The water drops to about -71 m at the cliff foot [F37] and runs about 150 km
across the floor [F38] to a lake of about 490 km² at about -97.6 m [F39, F40], about Lake Tahoe's
size [F54].

### Storage

The upper lake and a diked cliff-foot pond form a small pumped-storage pair across 251-261 m of
head [F47]. At 1-1.5 million m³/day [F49] it moves about 0.75-1.2 GWh/day in and returns
0.6-1.0 GWh/day [F48, F50, F51], close to the round trip of new pumped-storage plants [F52].
Draining the whole upper lake once gives about 90-97 GWh but takes months [F53]. Storage shifts
energy in time; the net gain comes only from the drop below sea level.

### Lake and staging

At an assumed 5.5 mm/day of evaporation [F55], the 490 km² lake needs about 2.7 million m³/day of
make-up [F58], or two to three large plant pairs [F56, F59]. The first build is one reactor, one
corridor, one basin: one plant pair holding about 180-270 km² [F57].

### Salt

The lake is held at about 1,000 mg/L, the upper limit for fresh water [F61], not at the 5-30 mg/L
of its feed [F66]; skipping the second RO pass would need about 40 % more water [F67]. At that
level the tolerant field crops and date palm keep full yields [F62, F63]; maize, citrus and grapes
lose up to a tenth [F64]; beans, carrots and onions struggle [F65]. A bleed of 1-3 % of inflow
[F68] (11-12 % with Nile water [F69]) irrigates part of a zone of about 110 km² of salt-tolerant
edge farms, which it fills only in the high-Nile case [F71]; the farms' drainage [F72] flows to a natural salt cell of 47-54 km² [F73], with a reserve pit and pans
for surges [F74].

Before the lake is held, the floor's salt crust is flushed: each centimetre holds about 10.6
million tonnes [F75], and its thickness is unknown [F76]. A crust up to 10 cm clears in about
3-6 months [F77] using 0.24-0.75 km³ of water [F78] (5 months to 2 years of one plant pair's
output, or 3-9 months at the full goal) and 18-91 GWh of brine pumping, once [F79].
Pore brine keeps diffusing out for years, so early salinity of 1,500-3,000 mg/L is accepted [F80].
Field cores come first. Where cores show a leaky or salty bed, a liner or engineered barrier under
the lake is the fallback; its cost is not found [F82].

### Nile feed: future option, outside the scored design

In surplus years only, 0.1-0.5 km³ [F87] of Nile water, about 170-240 mg/L [F90], could run by
its own canal from the Delta head over a saddle near Moghra at about 110.5 m [F91] to the lake,
about 507 km [F92], netting about +0.05 to +0.16 kWh/m³ as an open canal [F93] while needing no
desalination. Nile flow to the sea has fallen from about 6.2 to 1.7 km³ a year [F88], and how
often a surplus comes is not found [F89]. A capped branch could let Wadi El Natrun farms pump less
from an aquifer overdrawn by about 106 million m³ a year [F94, F95, S40], with a buffer for the
natron lakes and bird area [S47] and clear of the monasteries [S41]. Without an outlet the feed
would add 2-16 mg/L a year [F96]; sediment is low [F97]. The Toshka lakes, filled by Nile
overflow, have been shrinking since, and reports describe them turning salty [S43, S44]; the feed needs screening for
schistosomiasis snails [S45, S46]; New Delta overlap is unmapped [S50]. Nothing here enters the
card's energy, storage or lake figures.

## Why this, not the rival

The seawater scheme uses the drop but destroys the freshwater use and was rejected [F6]. Coastal
desalination piped straight to users needs no lift, no ridge cut, no evaporation make-up and no
salt balance; it is the bar. About 97-99 % of the lake's desalinated water evaporates [F98]: the
same water piped direct would irrigate about 33 to 100 times more farmland than the bleed does. That measures water productivity, not the total value of the two systems: the lake also provides storage and a reserve.
This card beats the rival only if a held freshwater lake (reserve, edge farming, local humidity) is worth the extra pipe and the 2.7 million m³/day lost to
the sky [F58], and if the drop repays the lift after friction [F46]. No opened cost study transfers to this
corridor [F81], and a corridor cost is not found [F82].

## Who gains, who loses

The coalition is Egypt's water, electricity and planning ministries, the plant operator, edge
farmers and the grid operator. The operator gains a use for discharged heat but keeps control of
any cooling-water change [F12, F14]. Edge farmers gain water at a salinity that suits tolerant
crops [F62]. The grid gains a flexible load and an evening shift [F51].

Losers are the oil and gas interests whose producing fields (Razzak, Alamein, Abu Gharadig among
others) lie in the Western Desert around the depression [S48, S49] and whose areas the review counted [F7, F8]; Siwa, its
springs and wells, if seepage or salt spreads [F70]; coastal marine life at the intake and outfall
[F27]; and taxpayers if the lake costs more than direct supply [F82]. Why not yet: the seawater
history, the 2026 review, and the absence of any coupled model, cost or survey.

## How we'd know

Pump work, pipe losses, desalination energy and turbine recovery measured on the same water, net
energy per m³ published. Lake salinity held inside a stated band. Leakage and evaporation measured,
not assumed [F55, F70]. Brine and intake inside permit limits. Oil, gas, settlement and habitat
constraints answered as explicit accepts or refusals before any fill.

The first test is the coupled corridor model in `first_test`, with field cores of the floor in
parallel. It fails if the corridor cannot show a lift-to-drop, a brine plan and a salt balance
that support a held freshwater lake. After it: compare at least one alternate basin on
lift-to-drop; Qattara wins only if the numbers say so.

## Why it might fail

- Desalination energy dominates and friction turns the small gravity gain into a cost, so the
  plant buys far more outside power than the target allows [F23, F46].
- Fresh water dissolves salt from the floor faster than the bleed removes it, or seeps toward
  wells and Siwa [F70, F76, F80].
- Evaporation make-up costs more than the lake is worth [F58].
- The ridge cut costs too much and the booster's losses, with pipe friction, push the net into a cost [F35, F36, F46].
- Brine or intake fails coastal permitting [F27].
- Oil and gas areas, pipelines or habitat block the only workable route or footprint [F7, F8].
- Nuclear desalination plus a long pressure pipe costs more than direct supply [F82].
- A new freshwater ecosystem in the desert brings unwanted consequences (mosquitoes, invasive species); its ecology is unknown.
- The project drifts back to seawater under a hydropower excuse, the path already rejected.

Stress test: "Egypt already rejected this." Partly. The review rejected seawater filling, judged a
rim-desalination pipeline not feasible for reasons not published, and favoured no reservoir
[F6]. This design differs in what fills the basin and how desalination is powered, but those
differences clear nothing by themselves; it still faces seepage, Siwa, oil and gas, and cost. If
it cannot pass those, the review's conclusion holds here too. "The lake will make it rain" is not
claimed: a lake this size should raise humidity near the shore; more than that is not counted.

## Open questions

- Does a ground survey confirm the route, the ridge, and the lake levels [F29, F34, F39]?
- What usable heat, temperature and hours does a chosen reactor offer, and what cooling-water rise
  would the operator allow [F12, F22]?
- What MED/RO split, brine volume and outfall fit one plant [F27]?
- What share of hours does RO run on surplus, and how much larger must it be [F25]?
- Does one corridor's solar yield plus reactor surplus cover annual pumping and RO [F26]?
- How thick is the crust, and how much brine sits below it [F76, F80]?
- What evaporation and leakage apply to a freshwater lake here [F55, F70]?
- Can the edge-farm soils take 1,000 mg/L water and drain to the salt cell [F71]?
- Why was scenario 5 judged not feasible, and do the reasons apply here [F6]?
- How do the plateau oil and gas fields and pipelines map against the route [S48]?
- Who holds intake, right-of-way and basin-rim rights, and who can stop the project?
- What is the lake for: reserve, habitat, farm supply, storage, or the lake itself?
- How often does the Nile have a surplus, and how would the Natrun branch drain [F89, F94]? Would
  taking surplus flow weaken the Delta's defence against seawater intrusion [F88]?
- How long does the first lake take to fill while it evaporates, and is it worth it for most of a
  decade at 1,500-3,000 mg/L [F57, F80]?
- Does the corridor cross Second World War minefields near El Alamein, and what does clearance cost?
- Would a shallow desert lake breed mosquitoes or the snails that carry schistosomiasis, and how is
  that controlled?
- Would the lower eastern gap (crest about 148 m) give a better lift-to-drop than the illustrative
  route [F34]?
