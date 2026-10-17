---
idea_id: spare-tire-microgrids
title: Spare-tire microgrids
status: ready
tags: [tech]
---

# Spare-tire microgrids

**Claim:** A standard skid of battery, controls, and an engine generator with stored fuel, fed by an on-site solar array, should keep water and flood pumps running through grid outages better than a standby generator alone.

**Status:** ready · lab memo · unfinished experiment

**Terms (once):** **Microgrid** = a set of loads and local power sources that can run tied to the grid or cut loose ("island") and run alone. **Skid** = a factory-built steel frame carrying the battery, inverter, controls, and engine generator, shipped and set as one unit. **Site array** = the solar panels on the same site but off the skid: parking or yard canopies, roofs, or ground mounts. **CHP** = combined heat and power, a generator whose waste heat is put to use. **Ride-through** = keeping power steady in the seconds between grid loss and the engine taking load. **VFD / soft starter** = a variable-frequency drive or an electronic soft starter, either of which brings a motor up to speed gradually and limits its starting surge. **State of charge** = how full the battery is. **Behind the meter** = equipment on the customer's side of the utility meter.

Working figures and unknowns (labeled):

- **Water energy:** drinking water and wastewater systems use about **2%** of U.S. energy (EPA, Energy Efficiency for Water Utilities web page); an older EPA page puts treating and moving wastewater alone at **3–4%** of U.S. electricity (EPA, Spend Less Energy Managing Water), and a 2018 study of over 160 utilities (Chini and Stillwell, Water Resources Research) put it at about **1%** of U.S. electricity (**published-contested**: estimates differ by method and by energy versus electricity). Pumping is **90–99%** of a water system's energy use; groundwater systems use about **1,800 kWh** per million gallons and surface-water systems about **1,500** (EPA 816-F-13-004, 2013) (**established**).
- **Engine start time:** stationary natural gas or diesel generators start within about **7–10 seconds** of an outage (EPA, Power Resilience Guide for Water and Wastewater Utilities, 2023) (**established**). NFPA 110 "Type 10" means power back within **10 seconds**; whether a given pump station must meet the strictest level is set by the local code and code official, not by NFPA 110 itself (NFPA, An Overview of NFPA 110, 2023) (**established**).
- **Standby engines run little by design and by rule:** emergency standby generators are typically rated for no more than about **200 hours a year** (EPA 2023 guide) (**established**). Under federal engine rules, an emergency engine may run without limit in a real emergency but only **100 hours a year** for maintenance and testing, of which up to **50** may be non-emergency use, and not for peak shaving or selling power (40 CFR 63.6640(f)) (**established**). State air rules may be stricter (**not checked**).
- **Engine heat is only worth something if it is used:** CHP reaches about **65–80%** total efficiency against about **50–55%** for grid power plus an on-site boiler (EPA CHP Partnership) (**established**). That figure assumes an engine that runs many hours with a heat user beside it. A standby engine that runs tens of hours a year has almost nothing to recover (**working assumption**, following from the run-hour rules above).
- **Single generators struggle with long outages:** NREL's analysis of two large generator data sets found that even a well-maintained single emergency diesel generator is only about **80%** likely to carry power through a two-week grid outage, and that reliability varies by more than tenfold with maintenance level (Marqusee and Jenket, Applied Energy, 2020) (**established**; abstract read).
- **Fuel:** the U.S. Army Corps of Engineers rule of thumb for diesel use is **0.07 gallons per hour per kW** of generator size (cited in the EPA 2023 guide) (**established** rule of thumb). One utility manager quoted in the same guide stores five days of fuel at 70% load (**practitioner practice, not a standard**). Standard engine service comes about every **240 running hours**, or ten days of continuous running (EPA 2023) (**established**). How many days of fuel a skid should carry: **not found**; it depends on each site's storm and resupply risk.
- **Gas pipelines can fail with the grid:** in the February 2021 freeze, Lower-48 natural gas production fell **28%** between 8 and 17 February; **21.5%** of the production decline came from power loss at wellheads, gathering, and processing; and **87%** of fuel-related generator outages were natural gas supply (FERC and NERC final report, 2021) (**established**). The EPA water guide notes that earthquakes can break gas lines and that bi-fuel generators can switch to diesel when gas is cut (**established**).
- **Flood pumping already leans on engines:** the Corps' pump-station manual says diesel drives are used at a number of New Orleans stations because no grid power is expected during a hurricane, and that large diesel drives need a great deal of maintenance (USACE EM 1110-2-3105, 2020) (**established**). The same manual names lack of operation and long downtime as the primary cause of equipment deterioration, and asks for generators to auto-test at least monthly and pumps to run at least twice a year (**established**).
- **When the backup is neglected:** in the 5 August 2017 New Orleans flood, the city's water board could self-generate **under 10%** of its designed 25-hertz pump power, and pumping in the hardest-hit basins was **45–70%** of design; the root-cause report blamed maintenance and funding (ABS Group for the City of New Orleans, 2018) (**established**).
- **Solar and batteries at water plants already exist:** the University Area Joint Authority in State College, Pennsylvania runs a **5 MW** solar array covering about **80%** of its wastewater plant's yearly energy, with a **500 kVA** battery and a microgrid for long outages; Inland Empire Utilities Agency in California manages **5 MW** of solar, **1 MW** of wind, and **4 MW** of batteries (EPA 2023 guide case studies) (**published**; case-study figures not independently checked).
- **Fuel cells:** a Bloom Energy Server 6.5 is **325 kW**, weighs about **13 tonnes** with its skid, runs on pipeline gas at **12–18 psig**, is built to run around the clock, and is listed at **65% falling to 53%** electrical efficiency over its life (vendor datasheet, February 2026) (**published**, vendor figures). Solid oxide fuel cell systems have usually run as steady base load; their load following is limited mainly by fuel-flow delays that can starve the cell during a sudden load step, which careful controls can manage (Mueller, Jabbari, and Brouwer, Journal of Power Sources, 2009) (**established**; no pump-station test found). Pairing a fuel cell with a battery for motor starts is a **working assumption** that follows from this.
- **Biogas CHP at wastewater plants:** **104** U.S. wastewater plants used digester biogas as their main CHP fuel, about **190 MW** in total, as of June 2011 (EPA CHP Partnership, 2011) (**established**, 2011 vintage; a current count was **not found**).
- **One-off systems die on parts:** the Drake Landing borehole heat store in Alberta met over **90%** of 52 homes' space heating for years, then shut down in 2024 when parts and repair expertise ran out (OkotoksOnline, June 2024, citing the operator's information packet) (**established**).
- **Pump loads, single-site examples** (1 hp = 0.746 kW at the shaft): a Stockton, California reclamation district planned adding two **75 hp** drainage pumps, about **112 kW** together (Reclamation District 1614 newsletter, May 2018) (**established** for that site). Fountain Valley, California Well No. 9 runs a **500 hp** pump, about **373 kW**, at 3,500 gpm and 400 ft of head on a VFD (AKM project page) (**established** for that site). Stockton's 14-Mile Slough wastewater pump station beside a levee has six **300 hp** pumps on VFDs, about **1,340 kW** together, backed by a **2,000 kW** diesel standby generator (West Yost project page) (**established** for that site). The State College wastewater plant above uses about **9.8 million kWh** a year, about **1,100 kW** on average, derived from its first-year solar output of 7,845,429 kWh being about 80% of plant demand (EPA 2023 case study) (**working assumption**, derived). New Orleans' West Closure Complex drainage station runs 11 pumps, each on a **5,000 or 5,400 hp** diesel engine (ENR, 2012, gives both figures), about **41–44 MW** in total (**published-contested** on the exact rating). A typical range across U.S. wells, plants, and flood stations: **not found**.
- **Solar on the skid versus a site array:** a skid-sized footprint, taking a Tesla Megapack at 347 by 65 inches (about **14.5 m²**; Tesla Megapack order page, vendor-published), at a canopy density of **12–16 W per square foot** (SurgePV solar-carport glossary; **published**, thin source: an industry software vendor's glossary, not independently checked) holds only about **2–2.5 kW** of panels (**working assumption**, derived). Parking canopies hold about **1.0–2.5 kW per covered space** (same SurgePV glossary; **published**, thin source). Parking-lot canopy systems range from about **300 kW to over 6 MW**, and developers generally want at least 300 kW to cover fixed costs such as interconnection (International Journal of Energy Management, 2025) (**published**). One New York train-station canopy holds **4.18 MWp** over about **10 acres** and **1,100** spaces (same article), about **0.42 MWp per acre** (derived). Fixed-tilt ground arrays reach a median **0.35 MWdc per acre**, and single-axis tracking **0.24**, for plants built in 2019 (LBNL, 2022, from 736 U.S. plants) (**established**). Matching the 500 hp well's draw at full sun would take about **150–370** canopy spaces or about **1.1 acres** of fixed ground array (**working assumption**, derived; peak power only, not daily energy). Building inside a federal levee's easement requires Corps permission under Section 408 (USACE Section 408 program page) (**established**).
- **Utility battery module, such as Tesla Megapack** (a product example, not an endorsement or partner claim): the 2-hour version is **1,927 kW / 3,854 kWh** at **92.0%** round-trip efficiency; the 4-hour version is **979 kW / 3,916 kWh** at **93.7%**; 480 V three-phase; up to **84,000 lb** (Tesla Megapack order page, read 17 Oct 2026) (**published**, vendor). A surge or overload rating: **not found** on Tesla's page.
- **How long one module carries a pump load** (hours = stored kWh ÷ load kW, before discharge losses, motor losses, or any reserve held back; **working assumption** arithmetic on the figures above): the 112 kW drainage pair, about **34 hours** on either version; the 373 kW well, about **10 hours**; the 1,100 kW treatment plant, about **3.5 hours** on the 2-hour version, and not at all on the 4-hour version, whose 979 kW limit is below the load; the 1,340 kW lift station, about **2.9 hours** on the 2-hour version and not at all on the 4-hour version; the 41–44 MW flood station, not at all, since one module's power is under 5% of the load, and about **22–23** modules matched to its power would empty in about **2 hours**.
- **Motor starting:** a motor started at full voltage typically draws about **six times** its full-load current until it nears speed; soft starters cut that with an adjustable current limit; VFDs are not a starting problem but a harmonic-distortion one that the source must be sized for (Kohler Power Systems white paper, Sizing Generators for Motor Starting) (**established**). So a 500 hp well started at full voltage would ask for a surge several times its roughly 373 kW running draw, beyond one 2-hour module's 1,927 kW rating (**working assumption**, derived). Pumps on a battery need VFDs or soft starters and one-at-a-time starts.
- **Grid market access:** FERC Order 841 (2018) requires each regional market operator to let storage provide every capacity, energy, and ancillary service it can technically provide, and to set a minimum size no larger than **100 kW** (FERC Order 841) (**established**). FERC Order 2222 (2020) lets aggregations of distributed resources, including behind-the-meter batteries, take part in those markets, also with a minimum no larger than **100 kW**, and requires coordination with the local distribution utility (FERC Order 2222 fact sheet) (**established**). When each market operator put Order 2222 into effect: **not checked**. Behind-the-meter value outside wholesale markets comes from retail tariffs and utility programs, set state by state (**not checked** per state).
- **Water utilities doing grid work:** the Massachusetts Water Resources Authority contracted **1 MWh** of behind-the-meter storage at a water pumping station and an administration building for demand-charge management and demand response, announced in January 2021 (Stem, Inc. press release, January 2021) (**published**, thin source: vendor press release; no results reported). Irvine Ranch Water District put batteries at six sites, about **6.5 MW** and **35–36 MWh** (the report gives both), for demand-charge management and a utility demand-response program; every site cut load during events, but only **three of six** saw bill savings and three saw bills rise, and the report found that demand-response baselines penalize stacking the two uses (California Energy Commission report CEC-500-2024-048, 2024) (**established**). Santa Margarita Water District expects a battery at its Chiquita reclamation plant to save about **112,000 dollars a year** by charging off-peak and discharging at peak (Santa Margarita Water District news release, July 2025) (**published**, thin source: the district's own forward estimate, not a measured result). Revenue per kW for frequency regulation, arbitrage, or demand response at a water site: **not found** in a source opened here.
- **Forecast-driven charging already exists in products:** Tesla's Powerwall Storm Watch charges a home battery to full when a qualifying watch or warning is issued for the home's area, including flood, flash flood, and coastal flood warnings and hurricane or tropical storm watches, then returns to normal after the event (Tesla support page, Storm Watch) (**published**, thin source: vendor support page, home scale). A module charges from empty in about its rated duration at full power, about 2 or 4 hours, if the grid or array can supply that power (**working assumption**, derived from vendor ratings).
- **Not found:** installed cost of a standard skid; a battery-sizing rule for a given pump station; how often grid outages coincide with pumping need at levee stations; the share of U.S. flood and water pump stations with on-site backup; storage duration of compressed natural gas (CNG) per skid; the daily electric load of an idle levee station; a typical pump-power range across U.S. sites; a surge rating for the battery module; grid-service revenue per kW at a water site; how many hours before forecast rain the battery should be full.

## 1. The problem

Water and flood systems run on pumps, and pumps run on electricity. Wells, treatment plants, lift stations, and drainage stations behind levees all stop when the power stops. Storms are when the grid is most likely to fail and when the pumps are most needed.

Most sites answer this with a standby generator that sits idle for months, gets tested now and then, and is expected to start and run for days the moment the grid drops. Idle machines deteriorate, and a single generator is less certain over a long outage than it looks: even well maintained, it has about four chances in five of lasting two weeks. The New Orleans flood of August 2017 shows the failure in practice. The pumps were there; most of the self-generated power to run them was not.

Each district also tends to build its own one-off backup, which brings one-off parts, one-off know-how, and one-off failures.

## 2. The insight

A backup is more dependable when most of it does useful work every day. A site solar array and a battery can carry controls, gates, remote monitoring (SCADA), lighting, and smaller pumps daily, which keeps the electrical side of the site running, monitored, and exercised. The battery also covers the 7–10 seconds before an engine takes load and helps start big motors, so gates and controls never see a dead gap. The engine is then a true reserve: fueled on site, tested under load on a schedule, and asked to carry the big pumps only when the grid is down for long.

Engine rules point away from CHP for most of these sites. CHP pays when an engine runs thousands of hours and something next door uses the heat. A standby engine runs tens of hours a year, is limited to 100 hours of non-emergency use, and usually sits at a levee or well field with nothing nearby that needs heat. So the engine here is a generator. Heat recovery belongs only at wastewater plants, whose digesters need heat.

At a rarely run station, the battery and array sit mostly idle between storms. On dry days they can earn money doing grid work, then fill up and hold before forecast rain.

## 3. The proposal

### The skid and the site array

A factory-built skid in a few standard sizes, so a district buys a product instead of designing a plant. The skid carries the battery, inverter, controls, and engine generator. The solar is a separate site array, because a skid's own footprint holds only a few kilowatts of panels against pump loads of roughly 100 kW to over 1 MW.

- **Site array** on parking or yard canopies, building roofs, or ground mounts on the site, sized to make a real dent in the site's daily energy. Matching a 500 hp well at full sun takes on the order of 150–370 canopy spaces or about an acre of fixed ground array. Arrays inside a federal levee's easement need Corps Section 408 permission.
- **Battery** as a utility battery module such as Tesla Megapack (a product example, not an endorsement). One module carries a small drainage station or a 500 hp well for hours, a treatment plant for a few hours, and a large flood station not at all. It is sized for ride-through, motor starting, daily load, and grid work, not for running main pumps through a multi-day storm.
- **Inverter and starters** rated for motor starting: pumps on VFDs or soft starters, started one at a time, because a full-voltage start draws about six times running current.
- **Engine generator** with fuel stored on site: diesel, propane, or CNG, or a bi-fuel engine that uses pipeline gas while it flows and stored fuel when it does not. Pipeline gas alone does not count as the reserve, because gas supply can fail along with the grid.
- **Controls** that island the site automatically, shed non-critical loads, start pumps in sequence to limit the starting surge, and log every start, run hour, and fault.
- **Two smaller engines instead of one large one** where loads are large, so one failure still leaves part of the station running (EPA guidance for loads above about 500 kW).

### Where it goes first

Different sites use the two halves differently:

1. **Wells and treatment plants** run every day, so solar and battery displace grid power every day, and the engine covers outages.
2. **Levee and drainage stations** run rarely but must not fail when they do. Here the daily half mainly keeps controls, gates, and communications up and the equipment exercised, while the engine, or an existing diesel drive, carries the main pumps. Where a station already has engine-driven pumps, the skid adds ride-through, controls, and monitoring rather than replacing them.
3. **Wastewater plants with digesters** are the one place where engine heat recovery clearly belongs, because the digesters need heat and the biogas is already there.

### Operating rules

- Test the engine under load at least monthly and run every pump at least twice a year, as the Corps manual asks.
- Keep a written storm-week runbook: fuel on hand, resupply contracts, load-shed order, and who is on site.
- Report uptime, start success, and fuel use after every outage.

### Grid work between storms

When no rain is forecast, the array and battery earn money:

- **Demand-charge cuts and arbitrage** behind the meter, under the site's utility tariff: trimming the peak draw that sets part of the bill, and charging when power is cheap to use it when it is dear.
- **Demand response**, cutting site draw when the utility calls an event.
- **Frequency regulation, energy, and capacity** in regional wholesale markets (regulation means fast up-and-down power adjustments that keep the grid steady), where the site is large enough on its own or joins an aggregation.

Before a forecast storm, the controls stop grid work, charge to full, and hold until the storm passes. The trigger is a forecast or a watch rather than a warning, so the battery has time to fill; a module needs about its rated duration at full power to charge from empty. How many hours ahead it must be full is a working assumption for the first test to set. Grid contracts must let the site stop delivering when a storm is forecast, and pumping takes priority over every grid contract.

## 4. Why this

The pieces are proven one at a time: solar and batteries at water plants, diesel drives at hurricane pump stations, generators with automatic transfer. What is missing is a standard package and the habit of running most of it every day.

Standardizing helps in three ways. Parts and know-how stay available; the Drake Landing heat store failed on parts and repair skills, not on physics. Districts can buy without designing. And outage results from many sites can be compared. Running the electrical side daily goes after the main known failure, which is equipment that sat idle until the storm.

## 5. How you'd know

- Start success and time to carry load, at every test and every outage
- Hours the site held critical load during grid outages, against hours needed
- Pump capacity available during storms, as a share of design
- Fuel on hand at the start of an outage and fuel burned per outage hour
- Grid energy displaced by solar per year, by site type
- Battery state of charge when each storm's rain starts
- Net grid-service income and bill change per year, after charging costs and penalties
- Faults found during daily operation that would have stayed hidden on an idle standby set
- Cost per site against a standby-generator-only baseline (no number assumed here)

## 6. First test

One levee or drainage pump station and one well field or treatment plant in the same district. Install the skid at both, keep the existing backup in place, and log through one full storm season. Add one planned islanding test: cut the grid on purpose for 72 hours (a test design choice, not a sourced figure) under the storm-week runbook, with real pumping load. Between storms, enroll the battery in one grid program and log its state of charge at the start of every forecast storm.

**Win:** the skid starts and carries load every time; the site holds critical pumping through the test with no dead gap at gates and controls; fuel use matches the plan; the battery is full when each storm's rain starts; the well field shows measured grid savings; grid work earns more than it costs.

**Fail:** missed starts, gaps at transfer, fuel running short, a storm arriving with the battery low, grid work that raises the bill, or a daily half that delivers nothing useful at the levee station.

## 7. Open questions

- Which levee or pump station can host the first skid with a storm-week runbook and measured uptime?
- What skid sizes cover most sites: by pump horsepower, by run pattern, or both?
- How many days of on-site fuel is enough, and which fuel keeps best for a rarely run engine at each site?
- Does the daily half earn its cost at a rarely run levee station, or only at wells and plants?
- How do state air permits treat a skid whose engine runs only in emergencies and tests?
- Who owns and maintains the skid: the district, the utility, or a service contract?
- How many hours before forecast rain should the battery be full, and which forecast product triggers the hold?
- Which grid programs let a water site stop delivering when a storm is forecast, and what do they pay?
- Where can the site array go: parking, roofs, yards, or levee right-of-way with Corps permission?

## 8. Why it might not work

- **The engine is still the weak point.** If the engine is neglected, the skid fails the same way an old standby set does, with a battery that only buys minutes.
- **Fuel runs out or never arrives.** Roads close, tanks run dry, and pipeline gas can drop in the same storm.
- **The daily half does not pay at levee stations.** A station that pumps a few weeks a year has little daily load, so its solar may sit mostly unused unless it can export to the grid or earn grid-service income.
- **Big pumps outsize the skid.** Multi-megawatt drainage pumps need large engines or direct diesel drives that no standard skid covers.
- **Flooding reaches the skid.** Batteries, controls, and fuel must sit above the design flood level, which not every site allows.
- **Permits and interconnection** turn a product back into a custom project, site by site.
- **Standard sizes do not fit** local pump mixes, and districts return to one-off designs.
- **Cost.** If a well-maintained standby generator with a fuel contract gives the same outage uptime for less, the skid loses.
- **A forecast miss leaves the battery low.** A storm that arrives early, or was not forecast, finds the battery drained by grid work, and the station starts on the engine alone.
- **Grid work costs more than it earns.** In one California pilot at six water sites, every site cut load during utility events, but three of the six saw their bills rise.
- **Grid duties pull the other way.** A program may call for discharge on the same day the pumps need the battery.

What would make this wrong: skid sites logging no better outage uptime or start success than well-maintained standby sites, at higher cost.

## 9. Stress-test

**"The engine is CHP."** At a levee or well field there is no heat user, and the engine is limited to tens of non-emergency hours a year, so there is little heat worth recovering. Calling it CHP oversells it. Keep heat recovery to wastewater plants with digesters, and score it only there.

**"Solar plus battery can run the pumps."** Not the main drainage pumps through a multi-day storm under cloud. One module's roughly 1.9 MW is under 5% of a large flood station's 41–44 MW of engines, and about 22 modules matched to that power would empty in about two hours. The battery is for ride-through, motor starts, and small loads. A design that relies on the battery to carry the main pumps through a storm is wrong.

**"Natural gas is the reserve."** In February 2021, gas production fell 28% across the Lower 48, and about a fifth of the drop came from lost electricity. Pipeline gas is a daily fuel, not an independent reserve. The reserve needs fuel stored on site.

**"A fuel cell is a better reserve."** A fuel cell built to run all day on pipeline gas is a daily source with the same gas risk and slow ramps for motor starts. It may fit a campus that wants daily power. It is not this reserve.

**"Daily use makes the backup reliable."** It makes the electrical side reliable. The engine still sits mostly idle and still needs monthly loaded tests. If skid engines fail to start as often as plain standby sets, this part of the case fails.

**"Grid services pay for the battery."** Only if the site's tariff and programs pay and the grid duties do not cut into storm readiness. Water-site results so far are mixed, and no sourced revenue per kW for a water site was found. If logged grid income does not beat charging costs and penalties, the battery is a resilience cost, not an earner.

**"The battery will be full when the storm arrives."** Only if the hold rule fires early enough. If the first season logs any storm whose rain starts with the battery well short of full, the trigger or the lead time is wrong and must change before grid work continues.

**"Standard skids fit everyone."** If the first sites need custom engineering anyway, the product case shrinks to controls and runbooks.

Wrong in one line: skid sites lose pumping during outages as often as standby-only sites, or the daily half saves nothing at the stations that matter most.

## Sources

- [EPA, Energy Efficiency for Water Utilities](https://www.epa.gov/sustainable-water-infrastructure/energy-efficiency-water-utilities)
- [EPA, Spend Less Energy Managing Water](https://www.epa.gov/green-infrastructure/spend-less-energy-managing-water)
- [Chini and Stillwell, The State of U.S. Urban Water: Data and the Energy-Water Nexus, Water Resources Research, 2018](https://data.openei.org/files/6461/2017WR022265.pdf)
- [EPA 816-F-13-004, Strategies for Saving Energy at Public Water Systems, 2013](https://www.epa.gov/sites/default/files/2015-04/documents/epa816f13004.pdf)
- [EPA, Power Resilience Guide for Water and Wastewater Utilities, 2023](https://www.epa.gov/system/files/documents/2023-05/PowerResilienceGuide_2023_508c.pdf)
- [NFPA, An Overview of NFPA 110, 2023](https://www.nfpa.org/news-blogs-and-articles/blogs/2023/01/23/an-overview-of-nfpa-110)
- [40 CFR 63.6640](https://www.ecfr.gov/current/title-40/chapter-I/subchapter-C/part-63/subpart-ZZZZ/subject-group-ECFR24cf3a3de5678d3/section-63.6640)
- [EPA CHP Partnership, CHP Benefits](https://www.epa.gov/chp/chp-benefits)
- [Marqusee and Jenket, Applied Energy, 2020 (abstract)](https://www.osti.gov/biblio/1659849)
- [FERC and NERC, The February 2021 Cold Weather Outages in Texas and the South Central United States, 2021](https://www.ferc.gov/sites/default/files/2021-12/Cold%20Weather%20Report_%202021_120821.pdf)
- [USACE EM 1110-2-3105, Mechanical and Electrical Design of Pump Stations, 2020](https://www.publications.usace.army.mil/Portals/76/Users/182/86/2486/EM1110-2%20-3105.pdf)
- [ABS Group, New Orleans flooding root cause analysis, 2018](https://webwstprodstussc1.blob.core.windows.net/www-documents/Projects/Planning/ABS-Group-NOLA-Flooding-RCA-Report-August-2018_Final-NP.pdf)
- [Bloom Energy Server 6.5 datasheet, February 2026](https://www.bloomenergy.com/wp-content/uploads/bloom-energy-server-datasheet-feb-2026.pdf)
- [Mueller, Jabbari, and Brouwer, On the intrinsic transient capability and limitations of solid oxide fuel cell systems, Journal of Power Sources, 2009](https://www.sciencedirect.com/science/article/abs/pii/S0378775308021575)
- [EPA CHP Partnership, Opportunities for Combined Heat and Power at Wastewater Treatment Facilities, 2011](https://www.epa.gov/sites/default/files/2016-07/documents/opportunities_for_combined_heat_and_power_at_wastewater_treatment_facilities_market_analysis_and_lessons_from_the_field.pdf)
- [OkotoksOnline, Drake Landing shutdown, June 2024](https://okotoksonline.com/articles/sun-goes-down-on-drake-landing-solar-community)
- [Reclamation District 1614 newsletter, May 2018](https://rd1614.com/wp-content/uploads/2019/02/May-2018-Newsletter.pdf)
- [AKM, Fountain Valley Well No. 9](https://www.akmce.com/project/fountain-valley-well-9/)
- [West Yost, 14-Mile Slough Pump Station](https://www.westyost.com/awards/14-mile-slough-pump-station/)
- [ENR, West Closure Complex project of the year, December 2012](https://www.enr.com/articles/12844-enr-texas-louisiana-project-of-the-year-pump-station-creates-a-powerful-defense)
- [Tesla Megapack order page, read 17 Oct 2026](https://www.tesla.com/megapack/design)
- [SurgePV, Solar Carport glossary](https://www.surgepv.com/glossary/solar-carport)
- [Audin, Solar Canopies Can Turn Parking Lots into Power Plants, International Journal of Energy Management, 2025](https://www.aeecenter.org/wp-content/uploads/2025/05/IJEM-Vol7-Iss2-Solar-Canopies-Can-Turn-Parking-Lots-Into-Power-Plants.pdf)
- [LBNL, Land Requirements for Utility-Scale PV, 2022 (summary)](https://emp.lbl.gov/sites/default/files/emp-files/land_requirements_for_utility-scale_pv.pdf)
- [USACE, Section 408 program](https://www.usace.army.mil/Missions/Civil-Works/Section408/)
- [Kohler Power Systems, Sizing Generators for Motor Starting](https://resources.kohler.com/power/kohler/industrial/pdf/Sizing_Generators_for_Motor_Starting_WP.pdf)
- [FERC Order No. 841, 2018](https://www.ferc.gov/sites/default/files/2020-06/Order-841.pdf)
- [FERC Order No. 2222 fact sheet, 2020](https://www.ferc.gov/media/ferc-order-no-2222-fact-sheet)
- [Stem, Inc. press release on MWRA storage, January 2021](https://www.globenewswire.com/news-release/2021/01/13/2157733/0/en/Stem-Inc-Awarded-Project-to-Deliver-Smart-Energy-Storage-to-Massachusetts-Water-Resource-Authority.html)
- [California Energy Commission, CEC-500-2024-048, Irvine Ranch Water District pilot, 2024](https://www.energy.ca.gov/sites/default/files/2024-05/CEC-500-2024-048.pdf)
- [Santa Margarita Water District, How SMWD is Rethinking Energy Management, July 2025](https://www.smwd.com/m/newsflash/Home/Detail/219)
- [Tesla Support, Storm Watch](https://www.tesla.com/support/energy/powerwall/mobile-app/storm-watch)
