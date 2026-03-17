---
title: "Fire Risk Analysis"
---

The battery industry's safety argument comes down to one number: 0.3% of utility-scale BESS had a fire with safety concerns in a given year, per EPRI's failure database.

That's for a single year. These facilities operate for 15–20 years. The compound probability over an actual operating life tells a different story.

## The math

Probability of at least one fire over N years at annual rate r:

**P = 1 - (1 - r)<sup>N</sup>**

### Using the industry's 0.3% annual rate

| Years | Cumulative Probability | Odds |
|---|---|---|
| 1 | 0.3% | 1 in 333 |
| 5 | 1.5% | 1 in 67 |
| 10 | 3.0% | 1 in 33 |
| 15 | 4.4% | 1 in 23 |
| 20 | 5.8% | 1 in 17 |

Over 15 years at the industry's own rate: about **1 in 23.**

### At higher rates

| Years | 0.3%/yr | 0.5%/yr | 1.0%/yr |
|---|---|---|---|
| 5 | 1.5% | 2.5% | 4.9% |
| 10 | 3.0% | 4.9% | 9.6% |
| 15 | 4.4% | 7.2% | 14.0% |
| 20 | 5.8% | 9.5% | 18.2% |

## Why the real number is probably higher

The 0.3% figure comes from a fleet that's mostly new. Almost no utility-scale lithium-ion BESS has been running 10 years, let alone 20. We don't actually know what failure rates look like for aged systems.

Lithium-ion cells degrade over time — internal resistance goes up, dendrites form, thermal stability drops. These are well-understood mechanisms in battery science. The failure rate for a 15-year-old facility is not going to be the same as for a new one.

EPRI's database has about 81 reported incidents with root cause information for roughly 26 of them. Thermal events that didn't result in a major fire or make the news are probably underrepresented.

A 130 MW / 520 MWh facility is also a lot bigger than most of what's in the fleet data. More cells, more modules, more battery management systems, more points where something can go wrong.

And thermal runaway doesn't always stay in one container. It can cascade. The 0.3% figure treats all fires the same — it doesn't distinguish a contained single-container event from a Moss Landing-scale fire that destroyed 55–80% of the facility and evacuated the surrounding community.

## For this site

Someone buying a house across the parkway from a lithium-ion BESS is looking at a 1-in-23 chance of fire over 15 years, at minimum. Probably closer to 1-in-14.

Those numbers land a certain way when the facility is next to thousands of homes, next to salmon-bearing streams, in a valley where inversions trap smoke, with two ways out of the neighborhood.

| Chemistry | Thermal Runaway? | 15-year fire probability |
|---|---|---|
| Lithium-ion (NMC/LFP) | Yes | 4.4%–14.0% |
| Sodium-ion (NFPP) | None in testing | ~0% from this cause |

Sodium-ion doesn't have thermal runaway. That's not an incremental safety improvement — it's a different category of risk.
