---
idea_id: phev-first
title: PHEV-first
status: ready
tags: [tech, product]
---

# PHEV-first

**Claim:** At long-dwell parking, many slow chargers should produce more electric miles per dollar than a few fast posts, best used by moderate-battery PHEVs that cover ordinary days on electricity and occasional long trips on fuel.

**Status:** ready · test specified · lab card · unfinished experiment

**Terms (once):** **PHEV** = plug-in hybrid electric vehicle (grid charge plus liquid-fuel range). **BEV** = battery-electric only. **L1 / L2 / DCFC** = Level-1 AC (about 1.4–1.9 kW; **established**), Level-2 AC (range 2.9–19.2 kW, typical about 6.6–7.2 kW; **established**), DC fast charge (about 50–350 kW). **Long-dwell** = parking where the car sits for hours (work, overnight, apartment lot, street, driveway). **UF** = utility factor (share of miles expected on electricity given a charge pattern). **NHTS** = National Household Travel Survey. **Stall coverage** = chargers relative to parking spaces, so parked cars can plug without hunting scarce posts. **PEF** = petroleum equivalency factor (CAFE credit math for dual-fueled vehicles) — incentive detail lives off this card.

Working figures and unknowns (labeled):

- **Ordinary-day band:** about **40 electric miles** as a sizing choice above the average day, not a measured mean and not a claim that it covers a whole year (**working assumption**). 2022 NHTS average daily vehicle-miles are about **39.7** per household (all of its vehicles; margin of error 2.6), about **21.8** per driver, and about **21.7** per vehicle-day (derived from published totals); 2017 was about **48.8** per household and about **25.8** per driver (**established**); AAA 2022 about **30.1** miles per driver-day; FHWA passenger-car annual about **10,881** miles → about **29.8** miles per calendar day. SAE J2841 utility-factor tables rest on **2001** NHTS; 2017 is the last solid distribution vintage. **Not found:** a published 2022 vehicle-day distribution under 30 / 40 / 50 miles. Average trip length (about **11.5** miles; work trips about **13.4**) is not the same as a day. An older GM line that “40 covers 78% of commuters” meant **one-way commute**, not daily driving. Early Chevy Volt fleets (INL, 2011–12, n=923) showed mean about **40.7** miles between charges, median **31.6**, and 81% at or under 40 — early adopters, not today’s fleet. Travel is right-skewed: in 2017, trips of 50 miles or more were about **2.5%** of trips but about **43%** of person-miles.
- **Pack / wall energy for about 40 miles:** assume about **300 Wh/mi** mid-range (about 240–400 band) → about **12 kWh** usable pack / about **13–14 kWh** from the wall.
- **Refill hours for that band:** L1 at 1.4 kW ≈ **9–10 hours**; L2 at 3.3–3.8 kW ≈ **3.5–4.5 hours**; at 6.6–7.2 kW ≈ **1.8–2.2 hours**; at 11.5 kW ≈ **1.2 hours**. DOE federal workplace guidance: L1 ≈ **5 miles of range per hour** (so about 40 in an 8-hour workday); L2 ≈ **25 miles per hour**. NREL session data (about 150,000 sessions) averaged about **15 kWh** delivered.
- **Installed cost bands (published figures, excluding utility upgrades and demand charges):** L1 about **$200–600** (**not found** in a source checked); commercial L2 about **$4,400–10,600** per port, hardware plus install (NREL 2023; ICCT 2019 shows about **$3,880** workplace and **$5,440** public in 2019 dollars); DC fast 150 kW about **$112,200–196,200** per port and 350 kW and up about **$180,100–285,300** (NREL 2023; ICCT 2019 averages about **$81,818** per DC fast charger) (**established**). DC fast is about **9–45×** an L2 port depending on size; this is derived from ICCT 2019 and NREL 2023, no source states a ratio, and cost varies by site (**working assumption**). Managed sharing is about two vehicles per port in DOE guidance; more than two is practitioner assumption, not measured (**working assumption**). Demand charges are a large share of DCFC operating cost (directional, not a fixed formula here).
- **What “enough” stalls means:** there is **no clean published scientific share** of parking spaces that counts as enough. Building-code floors (for example CALGreen-style: roughly 40% L2-ready / 10% with L2 equipment — versions move), practitioner ratios (about 1 L2 per 3–4 plug-in vehicles, or 1 per 8–12 employees), and DOE federal workplace guidance (L1 ≈ 1 per employee; L2 ≈ 1–2) are practice, not a measured optimum. A national stock ratio from NREL (about 40 L2 plugs per 1,000 plug-in vehicles) describes the fleet stock, not how to design one lot. Enough is not one charger per stall.
- **Credits / PEF:** do **not** lock this card’s working math to vacated tax tables. Federal new-vehicle credits under 30D / 25E ended for vehicles acquired after **30 Sep 2025** (**established**; acquired means a binding contract plus a payment by that date). The separate charger credit under 30C ended for property placed in service after **30 Jun 2026** (**established**). PEF is **in flux**: the Eighth Circuit vacated the 2024 phase-down on 5 Sep 2025; DOE restored 82,049 Wh/gal on 8 Jan 2026; a DOE interim rule on 19 Feb 2026 removed the fuel content factor, so PEF is 12,307 Wh/gal (11,706 with a petroleum accessory), and DOE has said a further rule will follow (**established**). How EPA applies PEF to plug-in hybrid electric miles is **not found**. Incentive and PEF detail stays off this lab card.

## 1. The problem

Most cars travel relatively short distances on ordinary days and sit parked for hours — at work, overnight, apartment lots, street, or driveway. They still need long range sometimes. Right-skew travel makes the year different from the ordinary day: a thin tail of long trips carries a large share of person-miles.

Charging money often buys a few high-power stalls. Speed helps when the car is passing through. Most of the week the car is sitting. Those long-dwell sites need enough ordinary outlets that plugging in is ordinary, not a hunt for scarce premium posts. Work, apartment, street, driveway: same rule. An apartment lot is the office-lot problem with a different landlord. This is not a story about people who cannot charge at all.

## 2. The insight

When cars are parked for hours, access matters more than charging speed. Household vehicles are parked about 95% of the day (**established**), roughly six to ten hours at work and longer overnight (**working assumption**). That sit is an L1 / L2 finish problem for a moderate daily band, not a DC-fast problem. That lot rule may be useful even apart from the PHEV package: for battery-electric cars it is mostly about dwell coverage; for plug-in hybrids it is also about whether the cord gets used.

Engines are efficient at steady highway speed and wasteful in stop-and-go. Right-size the battery for the stop-and-go day (streets, errands, the crawl), not to cover a freeway commute on electricity. The engine can take the highway. The scarce-battery question underneath: what pack size buys the most electrically driven *inefficient* miles per unit of battery material?

**Serious rival:** cheap long-range battery-electric cars with dense home and fast charging, which drop the engine entirely. This card differs by sizing a smaller pack for the stop-and-go day and leaving the long trip to fuel, aiming for the most electric stop-and-go miles per unit of battery.

## 3. The proposal

### Vehicle

- **Pack:** a moderate battery for ordinary local and stop-and-go travel — starting band about **35–50 electric miles** (about **40** as a sizing choice above the average day (**working assumption**), not a settled answer; raise as packs get cheaper). Do not size the pack as a freeway-commute battery.
- **Electric where the pack beats the engine:** on a mixed trip, the car runs the engine for steady freeway cruising and saves the battery for stop-and-go, which the pack handles better than the engine. Saving charge needs a known route, from navigation or a learned commute; with no route known, the car uses charge first. It still must not drive on gas through town with a charged battery. That would make an unplugged plug-in hybrid a heavy gas car. Saving the battery this way lets a moderate pack cover longer mixed days, because those days usually include freeway miles. More fuel saved per unit of battery also means fewer imported cells and critical minerals per car, which serves energy independence and national security. The battery saving is a **working assumption** until real trip data scores it.
- **Utility factor as the vehicle metric:** SAE J2841 assumes a full charge at the start of each day (**established**). Real-world utility factor may fall short of the label: the ICCT U.S. report (Dec 2022) says real-world electric drive share *may be* **26–56%** lower than the EPA label assumes (**published-contested**; California BAR data gives 41–56% and Fuelly data 26–39% for model year 2022 plug-in hybrids rated 8–42 miles). SAE paper 2024-01-2155, by Toyota authors, disputes the Fuelly gap and says the BAR data is biased and unrepresentative; only its abstract was read. In Europe (ICCT, June 2022), private cars show **45–49%** electric driving against **70–85%** assumed, and company cars **11–15%** (**established**). Habitual non-chargers dominate the gap. **Whether people actually plug in is the kill switch** for the PHEV-shaped version of this idea.

### Parking lots

At long-dwell sites, treat charging as stall coverage and power-per-stall matched to how long cars sit — not as a small set of premium posts:

1. **Power per stall** — L1 (about 1.4–1.9 kW) or shared L2 (typically 6.6–7.2 kW) (**established** charger ranges) sized so the ordinary-day band finishes inside the sit (workday or overnight). At about 6–10 hours of dwell at work, and longer overnight, L1 / L2 finishes the about-40-mile band (**working assumption**); DC fast buys unused speed plus a demand spike.
2. **Stall coverage** — enough outlets that plugging is ordinary. Exact “enough” share of spaces is **unknown**; use pilots and practitioner bands, not a fake density claim. Where ports are shared, DOE guidance is about two vehicles per port; more than two is practitioner assumption, not measured (**working assumption**).
3. **Site demand** — prefer many slow ports over few fast ports so peak building load stays lower for the same electric-mile delivery at long dwell. Cost bands above: DC fast is about 9–45× an L2 port (**working assumption**, derived; cost varies by site).
4. **Home overnight** — when a plug exists at home, it is still the first refill. The lot thesis does not replace home charging; it covers the long sits away from home, and apartments that are office lots by another name.

Must not change when the lot pattern is chosen: the claim that electric miles per infrastructure dollar rise with coverage at long dwell. If the site installs a handful of DC-fast posts and calls coverage done, the proposal has been abandoned.

### Resilience

Keep liquid-fuel capability for long trips, emergencies, and gaps in charging. Road trips still work. Nobody waits on a perfect all-electric future to keep moving.

### Optional U.S. fuel-capability layer

Flex-fuel (E85) or other domestically producible liquids on these cars — even when the market value is low today — is an optional resilience add-on, not the center of the claim. The vehicle stays in the fleet a decade or more; you cannot retrofit a weekend if foreign oil gets tight. Pumps and stockpiles are a separate job. Corn is not the thesis. Capability is not the same as supply. Tradeoffs (land, water, food vs fuel, lifecycle, seasonal blend, availability in a disruption) stay open. Other countries may use different liquid backups.

### Money and credits

Incentive design, PEF / CAFE ladders, and credit windows live off this lab card’s working math. Vehicle credits 30D / 25E are dead after 30 Sep 2025 acquisitions; PEF tables are in flux after the 2024 phase-down was vacated. Do not treat a logarithmic pack credit or a vacated PEF ladder as settled inputs here.

## 4. Why this

Some drivers are excellent battery-electric candidates. Others travel long distances often, or park where a handful of fast posts will not cover the stalls. A transition can use different pack sizes and drivetrains for different use cases.

The package is three pieces, not one slogan: (1) many slow chargers at long dwell, (2) a moderate pack for stop-and-go ordinary days, and (3) liquid range for the thin long-trip tail. Make-or-break for the PHEV-shaped version is **plug-in frequency and realized utility factor**, not hardware on the lot alone. The lot pattern can still be right for battery-electric cars even if plug-in hybrids fail to plug in — score them separately. The pack size, charger ranges, and cost ratios here are working assumptions or published-contested figures; the thing to measure is plug-in frequency.

## 5. How you'd know

**Vehicle**

- Share of days plugged in
- Electric miles / total miles (realized utility factor)
- Gasoline gallons per 100 miles
- Gas burned while usable charge (and a cord) remained
- Battery utilization

**Lots**

- Chargers per parking space (stall coverage)
- Sessions per charger; share of parked cars that can charge without competing for a few posts
- Average charging power and peak site demand
- Installation cost per parking space served (stay inside the published cost bands above; do not invent a dollars-per-stall number)

**System**

Electric miles delivered per dollar of infrastructure and vehicle support — and, where possible, per kilogram of battery and per unit of peak grid capacity.

Units sold are a weaker number if they do not tell you whether the battery got used.

## 6. First test

One office lot or city fleet. People who can charge at home still do. Log charging and fuel for **90 days**.

Compare two treatments on similar sites or split lots:

- **A:** few higher-power chargers
- **B:** many low-power chargers (L1 / shared L2 matched to dwell)

Compare electric miles, access, install cost (using the bands above), peak demand, conflicts, utilization, and realized utility factor.

**Win:** a high share of ordinary-day miles on electricity; most stalls can plug in; little competition for scarce posts; far fewer fuel stops — and a clear read on which charger pattern buys more electric miles per dollar.

**Alongside (not blocking):** keep the national ordinary-day band honest against the latest NHTS means; do not invent a 2022 day-length distribution that was not published.

If treatment B wins on electric miles per dollar at long dwell but PHEV drivers still do not plug in, the **lot rule** can survive as a battery-electric / dwell finding while the **PHEV-shaped package** fails. Score that split explicitly.

## 7. Open questions

- Exact working electric-mile band from current U.S. travel data (means versus a still-missing day-length distribution) — and how fast it should rise?
- What stall coverage counts as “enough” when science has no clean percentage?
- Power-per-stall schedule to refill about 40 electric miles in ordinary sits across work, overnight, and street parking?
- What actually raises plug-in rates (habit, software, deposit, fleet rules, a stall you can count on)?
- Who runs the first logged A/B lot?
- Optional fuel layer: put flex capability on the cars, grow supply, both, or defer?
- Off-card: which credit windows remain open, and what PEF rewrite DOE issues in 2026 — verify before any policy memo treats them as live.

## 8. Why it might not work

- **The rules score the wrong thing** — today’s utility-factor rules count only electric miles, so a car that saves charge on purpose for stop-and-go can look worse on paper even if it burns less fuel. The fix is to score fuel burned per mile, not electric miles alone.
- **People don’t plug in** — real utility factor stays far below the label; gas use stays high; the PHEV-shaped version dies even if the lot is wired.
- **Lots aren’t free power** — panels, landlords, and billing turn “enough for everyone” into a mega-project.
- **Coverage gets watered down** — a handful of chargers labeled as done; scarce posts bring back the hunt.
- **DC fast is sold as the long-dwell answer** — unused speed plus demand charges wipe the dollars-per-electric-mile case.
- **Car makers refuse dual hardware** — betting on battery-electric only; the PHEV premium never shrinks.
- **The pack gets judged as a freeway battery** — stop-and-go sizing looks “too small” against commute myths (including one-way commute stats misread as daily driving).
- **Cold weather or long suburb days** make an about-40-mile ordinary-day band feel tight without a higher pack or more reliable plugs.
- **Politics:** some critics call plug-in hybrids a delay on full electrification; others fight the fuel-blend rules; capability is not supply for any flex layer.
- **The pattern arrives too late** — cheap long-range battery-electric cars and dense home charging show up first.

What would make this wrong: unplugged cars, thin coverage, electric miles barely moving, or scarce high-power posts that leave most stalls dark.

## 9. Stress-test

**“About 40 covers ordinary life / the year.”** 2022 NHTS means do not show 40 per vehicle (about 22 per vehicle-day); 40 is a sizing choice above the mean (**working assumption**), and they do not publish a vehicle-day distribution under 30 / 40 / 50, and right-skew long trips carry a large share of person-miles. Utility-factor tables on 2001 NHTS and early-adopter Volt logs are not a modern fleet year-cover proof. Keep “ordinary day”; drop “covers the year” until a day-length distribution exists.

**“Many slow always beats few fast.”** Only at long dwell with a band that finishes inside the sit. Pass-through and en-route sites are a different product. If the A/B lot shows DC fast delivering more electric miles per dollar at about 6–10 hour dwell inside the cost bands above, the lot half of the claim fails.

**“Enough stalls.”** No clean scientific enough-percentage was found. Building-code floors and practitioner ratios are policy and practice, not a measured optimum. Claiming a percentage here would be invention. Pilots must report coverage and access conflicts, not assert a magic density.

**“PHEV-first rides on the lot.”** The lot rule can be right for battery-electric dwell and still fail for plug-in hybrids if habitual non-charging kills utility factor. Plug-in reality is the kill switch for the vehicle half. Score lot electric-miles per dollar and PHEV realized utility factor as separate pass / fail.

**“Credits / PEF make the math.”** Vehicle credits 30D / 25E are dead for acquisitions after 30 Sep 2025; the 2024 PEF phase-down was vacated; DOE is rewriting. Any card that treats a stale PEF ladder or a dead vehicle credit as a live working figure is wrong on dates. Keep incentive math off this card and mark it in flux.

**“Flex-fuel is required.”** It is an optional U.S. resilience layer. The claim stands or falls on long-dwell many-slow plus moderate-pack ordinary-day electrification. Capability without pumps is theater.

Wrong in one line: the first logged lot still concentrates spend in a few fast posts, most stalls stay dark, and plug-in hybrids burn gas with charge left — or the card invents a travel distribution, stall percentage, or PEF ladder that the sources do not support.
