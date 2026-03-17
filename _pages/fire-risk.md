---
title: "Fire Risk Analysis"
---

There are two ways to measure how often lithium-ion BESS facilities have fires. Both come from EPRI. They tell different stories — and neither one is reassuring for a 130 MW facility next to thousands of homes.

## Two metrics

**Metric 1: Per-project rate.** [EPRI's Stephanie Shaw](https://science.feedback.org/are-grid-battery-storage-systems-fire-prone/) said 0.3% of projects experienced a failure leading to a fire with potential safety concerns in 2024, drawing on their [BESS Failure Incident Database](https://storagewiki.epri.com/index.php/BESS_Failure_Incident_Database). This treats every project the same regardless of size — a 2 MW system and a 300 MW system each count as one project.

**Metric 2: Per-GW rate.** EPRI's [published failure data](https://www.energy-storage.news/battery-storage-failure-incident-rate-dropped-97-between-2018-and-2023/) shows 0.2–0.3 failures per GW of deployed capacity per year as of 2023–2024. This scales with facility size — larger facilities, with more cells and more potential failure points, contribute more to the denominator and carry proportionally more risk.

The per-project rate is a single-year observation from a fleet of roughly 431 projects. The per-GW rate is EPRI's published, normalizable metric. They measure different things: Shaw's number is specifically "fires with potential safety concerns," while the per-GW metric covers all failures.

## The math

Probability of at least one incident over N years at annual rate r:

**P = 1 - (1 - r)<sup>N</sup>**

### Using the per-project rate (0.3%/yr)

This is the industry's preferred number. It doesn't account for facility size.

| Years | Cumulative Probability | Odds |
|---|---|---|
| 5 | 1.5% | 1 in 67 |
| 10 | 3.0% | 1 in 33 |
| 15 | 4.4% | 1 in 23 |
| 20 | 5.8% | 1 in 17 |

### Using the per-GW rate for a 130 MW facility

0.3 failures/GW/yr × 0.13 GW = **3.9% annual rate.** This accounts for the fact that a 130 MW facility is roughly twice the fleet average (~63 MW).

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

The truth is somewhere in between. The per-project rate undercounts risk for large facilities. The per-GW rate includes all failures, not just fires with safety concerns. But even the low end — a 1-in-23 chance over 15 years — is not a number most people would accept next to their homes.

## Why the real number is probably higher than either

The fleet is mostly new. Almost no utility-scale lithium-ion BESS has been running 10 years, let alone 20. We don't actually know what failure rates look like for aged systems.

Lithium-ion cells degrade over time — internal resistance goes up, dendrites form, thermal stability drops. These are well-understood mechanisms in battery science. The failure rate for a 15-year-old facility is not going to be the same as for a new one.

EPRI's database has about 120 reported incidents total. Thermal events that didn't result in a major fire or make the news are probably underrepresented. EPRI itself notes it "cannot guarantee that the database captures every relevant BESS failure incident."

And thermal runaway doesn't always stay in one container. It can cascade. Neither metric distinguishes a contained single-container event from a Moss Landing-scale fire that destroyed 55–80% of the facility and evacuated the surrounding community.

## For this site

By either measure, the risk over a 15–20 year operating life is not small. At the low end, it's 1-in-23. Accounting for facility size, it could be far higher.

Those numbers land a certain way when the facility is adjacent to thousands of homes, next to salmon-bearing streams, in a ridge-bounded valley where inversions can trap smoke, with two ways out of the neighborhood.

| Chemistry | Thermal Runaway? | 15-year risk range |
|---|---|---|
| Lithium-ion (NMC/LFP) | Yes | 4.4%–45.0% |
| Sodium-ion (NFPP) | None in testing | ~0% from this cause |

Sodium-ion doesn't have thermal runaway. That's not an incremental safety improvement — it's a different category of risk.

## Earthquake risk

The Snoqualmie Valley sits at the intersection of three fault systems:

- **[Southern Whidbey Island Fault (SWIF)](https://washingtondnr.wpcomstaging.com/2009/09/11/southern-whidbey-island-fault-zone-mapped-through-snoqualmie-valley/)** — mapped directly through the Snoqualmie Valley, capable of M6.5–7.4 shallow earthquakes
- **Seattle Fault** — M7.0–7.5, very shallow (<25 km), highest shaking intensity
- **Cascadia Subduction Zone** — M9.0+, minutes of sustained shaking

King County's BESS ordinance requires [IEEE 693](https://standards.ieee.org/ieee/693/4996/) seismic qualification for structural and nonstructural components. That standard ensures equipment stays on its mounts during an earthquake. What it doesn't address:

- **Internal cell damage.** Research shows lithium-ion cells can develop internal short circuits from [as little as 4mm of axial compression](https://www.sciencedirect.com/science/article/abs/pii/S0378775314007708). An internal short circuit is the initiating event for thermal runaway. IEEE 693 prevents racks from toppling — it doesn't prevent the vibration and shock that damages cells internally.
- **Compound hazard analysis.** No requirement to model the earthquake → thermal runaway → fire → toxic runoff chain for this specific site. Fisher Creek is less than 10 vertical feet below the development area.
- **Site-specific seismic assessment.** The SWIF runs through this valley. [KCC 21A.24.290](https://aqua.kingcounty.gov/council/clerk/code/24-30_Title_21A.pdf) addresses development in seismic hazard areas, but the BESS ordinance doesn't explicitly cross-reference those provisions.
- **Post-earthquake response.** In a major earthquake, fire department access may be compromised, water supply disrupted, and evacuation routes damaged — exactly when a BESS fire would be most dangerous.

No utility-scale BESS has been hit by a major earthquake yet. That's because the fleet is young and mostly deployed in low-seismicity areas — not because these systems are proven earthquake-safe.

Again: sodium-ion eliminates the coupling. No thermal runaway means an earthquake can't trigger a chemical fire.
