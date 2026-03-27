---
title: "Fire Risk Analysis"
---

EPRI publishes a failure rate normalized by deployed capacity: [0.2–0.3 failures per GW per year](https://www.energy-storage.news/battery-storage-failure-incident-rate-dropped-97-between-2018-and-2023/) as of 2023–2024. For a 130 MW facility, that's a 3.9% annual rate. The industry prefers a different number. [EPRI's Stephanie Shaw](https://science.feedback.org/are-grid-battery-storage-systems-fire-prone/) said 0.3% of projects had a fire with potential safety concerns in 2024, but that treats a 2 MW system and a 300 MW system as the same thing.

Both come from EPRI's [BESS Failure Incident Database](https://storagewiki.epri.com/index.php/BESS_Failure_Incident_Database). They measure different things: Shaw's number is specifically "fires with potential safety concerns," while the per-GW metric covers all failures. Neither is reassuring for a 130 MW facility next to thousands of homes.

## "97% failure rate drop"

Jupiter Power's open house presentation claimed a "97% drop" in global grid-scale BESS failure rates between 2018 and 2023, citing EPRI data. This is the per-GWh rate: failures divided by total deployed capacity. It drops because deployment is growing exponentially (the denominator gets huge). Their own chart tells a different story. The absolute number of failure incidents is not declining. EPRI's database shows 8 incidents in 2024, which is among the highest annual counts on the chart. More batteries with a lower rate per GWh still means more fires.

The 97% number is also backward-looking. It's dominated by older, smaller systems. The fleet is getting younger and larger. A 130 MW facility built in 2028 will have more cells, more potential failure points, and no long-term operating history to draw on.

## The math

Probability of at least one incident over N years at annual rate r:

**P = 1 - (1 - r)<sup>N</sup>**

### Using the per-project rate (0.3%/yr)

The industry's preferred number. Doesn't account for facility size.

| Years | Cumulative Probability | Odds |
|---|---|---|
| 5 | 1.5% | 1 in 67 |
| 10 | 3.0% | 1 in 33 |
| 15 | 4.4% | 1 in 23 |
| 20 | 5.8% | 1 in 17 |

### Using the per-GW rate for a 130 MW facility

0.3 failures/GW/yr × 0.13 GW = **3.9% annual rate.**

| Years | Cumulative Probability | Odds |
|---|---|---|
| 5 | 18.1% | 1 in 6 |
| 10 | 32.9% | 1 in 3 |
| 15 | 45.0% | 1 in 2 |
| 20 | 54.7% | better than even |

### Side by side

| Years | Per-project (0.3%/yr) | Per-GW for 130 MW (3.9%/yr) |
|---|---|---|
| 5 | 1.5% | 18.1% |
| 10 | 3.0% | 32.9% |
| 15 | 4.4% | 45.0% |
| 20 | 5.8% | 54.7% |

Using the industry's own fire-specific rate, the cumulative probability of at least one fire over a 20-year facility life is approximately 6%. The per-project rate undercounts risk for large facilities. The per-GW rate includes all failures, not just fires. The actual risk for a specific facility is somewhere in this range.

## Why the real number is probably higher

Almost no utility-scale lithium-ion BESS has been running 10 years. Nobody knows what failure rates look like for aged systems.

Lithium-ion cells degrade: internal resistance goes up, dendrites form, thermal stability drops. These are well-understood mechanisms. The failure rate for a 15-year-old facility will not be the same as for a new one.

EPRI's database has about 81 reported incidents with root cause data for roughly a quarter of them. Thermal events that didn't make the news are probably underrepresented. EPRI itself notes it "cannot guarantee that the database captures every relevant BESS failure incident."

Thermal runaway doesn't always stay in one container. It can cascade. Neither metric distinguishes a contained single-container event from a Moss Landing-scale fire that destroyed 55–80% of the facility and evacuated the surrounding community.

## For this site

This facility would be adjacent to thousands of homes, next to salmon-bearing streams, in a ridge-bounded valley where inversions trap smoke, with two ways out of the neighborhood.

| Chemistry | Thermal Runaway? | 15-year risk range |
|---|---|---|
| Lithium-ion (NMC/LFP) | Yes | 4.4%–45.0% |
| Sodium-ion (Peak Energy NFPP) | None in abuse testing | ~0% from this cause |

Sodium-ion batteries have significantly higher thermal stability than lithium-ion. Peak Energy's NFPP chemistry, which Jupiter Power has contracted for other projects, has shown no thermal runaway in nail penetration, crush, overcharge, and saw testing. [Peer-reviewed research](https://www.mdpi.com/2313-0105/10/10/370) confirms that sodium-ion as a class has higher thermal runaway onset temperatures and lower pressure buildup than lithium-ion, though the degree of improvement varies by chemistry.

## Safety standards

Three overlapping standards govern BESS fire safety. None of them sets a national siting standard for where utility-scale facilities can be built relative to homes.

### NFPA 855

The National Fire Protection Association's [Standard for the Installation of Stationary Energy Storage Systems](https://www.nfpa.org/codes-and-standards/nfpa-855-standard-development/855). Covers design, installation, commissioning, operation, and decommissioning. The 2023 edition mandates fire suppression for nearly all ESS installations and requires battery management systems monitoring temperature, voltage, and state of charge. Referenced by the International Fire Code and many local jurisdictions.

### UL 9540A

Underwriters Laboratories' [test method for evaluating thermal runaway fire propagation](https://www.ul.com/services/ul-9540a-test-method) in BESS. The only consensus standard in the U.S. and Canada explicitly cited in NFPA 855 for large-scale fire testing. Tests progress from individual cell through module, unit, and full installation levels. Jupiter Power says their batteries are "fire safety tested according to strict Underwriters Laboratory protocols" — this likely refers to UL 9540A.

### IFC 1207

The [International Fire Code Section 1207](https://codes.iccsafe.org/s/IFC2024P1/chapter-12-energy-systems/IFC2024P1-Pt03-Ch12-Sec1207), adopted via Washington State Building Code Council. For remote outdoor installations, it requires a minimum **100-foot setback** from other buildings, lot lines, public ways, and exposure hazards. It requires evaluation of thermal runaway, mechanical failures, management system failures, and failures of external protection systems.

### Detection and suppression

Current detection options include VESDA (Very Early Smoke Detection Apparatus, laser-based air sampling), gas sensors for off-gases that precede thermal runaway (CO, H2, VOCs), and thermal imaging. Suppression options include water-based systems (effective at cooling but don't stop the electrochemical reaction), water mist, aerosol systems, and hybrid approaches.

All of these have limitations. The Moss Landing fire began after its fire suppression system failed. Water application can cause electrical shorts and [temporarily increases the peak HF production rate by 35%](https://www.nature.com/articles/s41598-017-09784-z), though total HF produced is unchanged. Aerosol systems work best before ignition in tight enclosures. No suppression technology has been proven to reliably stop cascade propagation once thermal runaway is deeply established at scale.

### How much HF?

[Larsson et al. (2017)](https://www.nature.com/articles/s41598-017-09784-z), published in *Scientific Reports* (Nature portfolio), measured HF emissions from lithium-ion battery fires across 7 cell types and 39 fire tests using two independent measurement methods. They found **20 to 200 mg of HF per Wh** of battery capacity. The paper extrapolates: a 1,000 kWh system could produce 20-200 kg of HF. The proposed Cascadia Ridge facility is approximately 520,000 kWh, 520 times larger than that example. Scaling the paper's findings: a full-facility fire could produce 10 to 104 metric tons of HF. Even a fire involving just 1% of the facility's capacity could produce over a metric ton. HF is immediately dangerous to life and health (IDLH) at just 30 ppm. It is colorless, has a pungent odor at higher concentrations but may not be detectable by smell at levels that still pose health risks, and symptoms of skin and lung exposure can be delayed by hours.

No atmospheric dispersion modeling has been done for this site. Nobody has studied what HF concentrations would look like at Cascade View Elementary (approximately half a mile away), along school bus routes on Snoqualmie Parkway (0.1 miles away), or in the surrounding neighborhoods during a lithium-ion battery fire. The Snoqualmie Valley's topography traps airborne emissions close to the ground during temperature inversions rather than dispersing them. These quantities are large enough that dispersion modeling should be required before this project is approved.

### Regulatory gaps

- **No federal siting standards.** BESS siting is governed by local land use and building codes, which vary enormously. Some jurisdictions have no BESS-specific ordinances.
- **Inconsistent setbacks.** Ranges from 10 feet (IFC egress minimum) to 150 feet (some county ordinances) with no national consensus for utility-scale facilities near residential areas.
- **No standard air monitoring requirement.** At Moss Landing, EPA deployed monitoring stations reactively after the fire started. No BESS facility is required to have permanent fenceline air quality monitoring.
- **Post-incident cleanup is reactive.** EPA had to order cleanups at both Gateway and Moss Landing. Whether operators carry adequate financial assurance for worst-case cleanup is unclear.

## Earthquake risk

The Snoqualmie Valley sits at the intersection of three fault systems:

- **[Southern Whidbey Island Fault (SWIF)](https://washingtondnr.wpcomstaging.com/2009/09/11/southern-whidbey-island-fault-zone-mapped-through-snoqualmie-valley/)**, mapped directly through the valley, capable of M6.5–7.4 shallow earthquakes
- **Seattle Fault**, M7.0–7.5, very shallow (<25 km), highest shaking intensity
- **Cascadia Subduction Zone**, M9.0+, minutes of sustained shaking

King County's BESS ordinance requires [IEEE 693](https://standards.ieee.org/ieee/693/4996/) seismic qualification for structural and nonstructural components, which keeps equipment on its mounts during an earthquake. But it doesn't address what happens inside the cells.

Lab testing shows lithium-ion cells can develop internal short circuits, the initiating event for thermal runaway, from [small mechanical deformations](https://www.sciencedirect.com/science/article/abs/pii/S0378775314007708). The faults threatening this valley are capable of M6.5–7.5 shallow earthquakes that produce significant ground acceleration. No study has tested this chain at utility scale, and nobody has tested whether utility-scale BESS enclosures protect cells the way crash-tested EV packs do.

Beyond cell damage, there's no requirement to model the full chain for this site: earthquake shaking damages cells → thermal runaway → fire → contaminated runoff into Fisher Creek, less than 10 vertical feet below the development area. The SWIF runs through this valley, but the BESS ordinance doesn't cross-reference [KCC 21A.24.290](https://aqua.kingcounty.gov/council/clerk/code/24-30_Title_21A.pdf)'s seismic hazard area provisions. And in a major earthquake, fire department access, water supply, and evacuation routes may all be compromised, exactly when a BESS fire would be most dangerous.

No utility-scale BESS has been hit by a major earthquake. That's because the fleet is young and mostly deployed in low-seismicity areas, not because these systems are proven earthquake-safe.

Peak Energy's sodium-ion cells have been [nail-penetrated, crushed, and sawed](/battery-technology#abuse-testing) without ignition: 0% ignition rate vs. 23% for lithium-ion. For chemistries that don't exhibit thermal runaway, the earthquake-to-fire chain does not apply.

## Evacuation

Snoqualmie Ridge has two primary egress routes: Snoqualmie Parkway and SR-18. Moss Landing evacuated 1,200 to 1,500 people from a smaller community with more ways out. Snoqualmie Ridge is bigger.

The City of Snoqualmie's own [Comprehensive Emergency Management Plan (ESF #16, November 2017)](https://www.snoqualmiewa.gov/DocumentCenter/View/17031/ESF-16---Evacuation-PDF) identifies several constraints:

- The **police department has very limited on-duty personnel** for a large-scale evacuation, and may need to rely on statewide mutual aid from areas not affected by the event.
- The city is **heavily dependent on roads, bridges, and assets it doesn't own or operate**, including King County and WSDOT infrastructure.
- In a major earthquake, "**such severe damage to critical infrastructure** that elements of evacuation pre-planning is impractical to determine prior to an actual evacuation."
- The plan **assumes the city will have enough accurate and adequate notice** to implement an evacuation. "There may be times were there is too little or too late of notice to successfully evacuate all or certain parts of the population."
- Private ambulance services **would not be available** to Snoqualmie due to commitments to higher-population areas like Seattle.
- School buses and Metro buses are in the city but **may not have staffing to operate them** during an evacuation.

The plan lists trigger events: earthquakes, mudslides, floods, volcanic activity, fires, dam failure, terrorism. It does not contemplate an **industrial toxic release** from a battery storage facility. The plan predates Ordinance 19824 by seven years. No BESS-specific evacuation scenario has been studied for this community.

The population numbers in the plan (11,000+ residents, 3,200 students, plus thousands of casino and hotel visitors) are from 2017. Snoqualmie Ridge has grown since then.
