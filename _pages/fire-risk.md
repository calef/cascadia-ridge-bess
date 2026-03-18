---
title: "Fire Risk Analysis"
---

EPRI publishes a failure rate normalized by deployed capacity: [0.2–0.3 failures per GW per year](https://www.energy-storage.news/battery-storage-failure-incident-rate-dropped-97-between-2018-and-2023/) as of 2023–2024. For a 130 MW facility, that's a 3.9% annual rate. The industry prefers a different number — [EPRI's Stephanie Shaw](https://science.feedback.org/are-grid-battery-storage-systems-fire-prone/) said 0.3% of projects had a fire with potential safety concerns in 2024 — but that treats a 2 MW system and a 300 MW system as the same thing.

Both come from EPRI's [BESS Failure Incident Database](https://storagewiki.epri.com/index.php/BESS_Failure_Incident_Database). They measure different things: Shaw's number is specifically "fires with potential safety concerns," while the per-GW metric covers all failures. Neither is reassuring for a 130 MW facility next to thousands of homes.

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

The per-project rate undercounts risk for large facilities. The per-GW rate includes all failures, not just fires. The actual risk for a specific facility is somewhere in this range.

## Why the real number is probably higher

Almost no utility-scale lithium-ion BESS has been running 10 years. Nobody knows what failure rates look like for aged systems.

Lithium-ion cells degrade — internal resistance goes up, dendrites form, thermal stability drops. These are well-understood mechanisms. The failure rate for a 15-year-old facility will not be the same as for a new one.

EPRI's database has about 81 reported incidents with root cause data for roughly a quarter of them. Thermal events that didn't make the news are probably underrepresented. EPRI itself notes it "cannot guarantee that the database captures every relevant BESS failure incident."

Thermal runaway doesn't always stay in one container. It can cascade. Neither metric distinguishes a contained single-container event from a Moss Landing-scale fire that destroyed 55–80% of the facility and evacuated the surrounding community.

## For this site

This facility would be adjacent to thousands of homes, next to salmon-bearing streams, in a ridge-bounded valley where inversions trap smoke, with two ways out of the neighborhood.

| Chemistry | Thermal Runaway? | 15-year risk range |
|---|---|---|
| Lithium-ion (NMC/LFP) | Yes | 4.4%–45.0% |
| Sodium-ion | None in testing | ~0% from this cause |

Sodium-ion does not have thermal runaway.

## Earthquake risk

The Snoqualmie Valley sits at the intersection of three fault systems:

- **[Southern Whidbey Island Fault (SWIF)](https://washingtondnr.wpcomstaging.com/2009/09/11/southern-whidbey-island-fault-zone-mapped-through-snoqualmie-valley/)** — mapped directly through the valley, capable of M6.5–7.4 shallow earthquakes
- **Seattle Fault** — M7.0–7.5, very shallow (<25 km), highest shaking intensity
- **Cascadia Subduction Zone** — M9.0+, minutes of sustained shaking

King County's BESS ordinance requires [IEEE 693](https://standards.ieee.org/ieee/693/4996/) seismic qualification for structural and nonstructural components — that keeps equipment on its mounts during an earthquake. But it doesn't address what happens inside the cells.

Lab testing shows lithium-ion cells can develop internal short circuits — the initiating event for thermal runaway — from [small mechanical deformations](https://www.sciencedirect.com/science/article/abs/pii/S0378775314007708). The faults threatening this valley are capable of M6.5–7.5 shallow earthquakes that produce significant ground acceleration. No study has tested this chain at utility scale, and nobody has tested whether utility-scale BESS enclosures protect cells the way crash-tested EV packs do.

Beyond cell damage, there's no requirement to model the full chain for this site: earthquake shaking damages cells → thermal runaway → fire → contaminated runoff into Fisher Creek, less than 10 vertical feet below the development area. The SWIF runs through this valley, but the BESS ordinance doesn't cross-reference [KCC 21A.24.290](https://aqua.kingcounty.gov/council/clerk/code/24-30_Title_21A.pdf)'s seismic hazard area provisions. And in a major earthquake, fire department access, water supply, and evacuation routes may all be compromised — exactly when a BESS fire would be most dangerous.

No utility-scale BESS has been hit by a major earthquake. That's because the fleet is young and mostly deployed in low-seismicity areas, not because these systems are proven earthquake-safe.

Sodium-ion cells have been [nail-penetrated, crushed, and sawed](/battery-technology#abuse-testing) without ignition — 0% ignition rate vs. 23% for lithium-ion. Without thermal runaway, the earthquake-to-fire chain does not apply.
