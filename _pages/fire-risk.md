---
title: "Fire Risk Analysis"
---

The battery storage industry points to a low annual failure rate as evidence of safety. The number they cite — 0.3% of utility-scale BESS experienced a fire with safety concerns in a given year — comes from EPRI's BESS Failure Incident Database.

But these facilities run for 15–20 years. When you compound the annual rate over the actual operating life, the picture looks different.

## The math

Probability of at least one fire over N years at a constant annual rate r:

**P = 1 - (1 - r)<sup>N</sup>**

### At the industry's own 0.3% annual rate

| Years | Cumulative Probability | Odds |
|---|---|---|
| 1 | 0.3% | 1 in 333 |
| 5 | 1.5% | 1 in 67 |
| 10 | 3.0% | 1 in 33 |
| 15 | 4.4% | 1 in 23 |
| 20 | 5.8% | 1 in 17 |

Over 15 years: roughly **1 in 23.**

### At higher annual rates

| Years | 0.3%/yr | 0.5%/yr | 1.0%/yr |
|---|---|---|---|
| 5 | 1.5% | 2.5% | 4.9% |
| 10 | 3.0% | 4.9% | 9.6% |
| 15 | 4.4% | 7.2% | 14.0% |
| 20 | 5.8% | 9.5% | 18.2% |

## Why 0.3% is probably too low

**The fleet is young.** Almost no utility-scale lithium-ion BESS has been running 10+ years. The 0.3% figure reflects mostly new equipment. We don't know what happens as these systems age.

**Batteries degrade.** Internal resistance increases, dendrites form, thermal stability drops. Older cells are more failure-prone. The 0.3% rate doesn't capture this because the fleet hasn't gotten there yet.

**Smaller events get missed.** EPRI's database has about 81 incidents but root cause data for only 26 or so. Thermal events that didn't make the news probably aren't counted.

**Bigger facilities have more failure points.** A 130 MW / 520 MWh system has far more cells, modules, and control systems than a typical installation.

**Single fires can cascade.** Thermal runaway can jump from container to container. The 0.3% rate doesn't distinguish between a single-container event and a facility-wide fire like Moss Landing.

## What this means here

A homeowner buying a house across the parkway from a lithium-ion BESS is looking at a 1-in-23 chance of a fire with safety concerns over 15 years — using the industry's own number. At more realistic rates, it's closer to 1-in-14.

That's across the street from thousands of homes, next to salmon-bearing streams, in a valley where inversions trap smoke, with limited evacuation routes.

| Chemistry | Thermal Runaway? | 15-year fire probability |
|---|---|---|
| Lithium-ion (NMC/LFP) | Yes | 4.4%–14.0% |
| Sodium-ion (NFPP) | None in testing | ~0% from this cause |

Sodium-ion takes thermal runaway off the table. That's not a marginal improvement — it removes the risk category entirely.
