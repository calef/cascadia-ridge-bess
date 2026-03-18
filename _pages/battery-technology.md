---
title: "Battery Technology"
---

## Lithium-ion risks

Thermal runaway is an uncontrolled temperature rise inside a battery cell that feeds itself. Once one cell goes, it can cascade through an entire container. The process generates large volumes of flammable and toxic gas.

### Incidents

| Date | Facility | Capacity | What happened |
|---|---|---|---|
| 2017–2019 | [South Korea (23+ sites)](https://www.pv-magazine.com/2023/07/04/whats-behind-south-koreas-battery-fire-accidents/) | Various | 23+ fires, $32M+ losses, 522 ESS units shut down nationwide. Root causes: insufficient battery protection, poor installation, BMS integration gaps |
| Apr 2019 | [McMicken, AZ](https://www.utilitydive.com/news/aps-says-runaway-thermal-event-caused-2019-battery-explosion-outlines-4-st/582475/) | 2 MW | Explosion injured 4 firefighters seriously, 8+ first responders total |
| May 2024 | [Gateway, San Diego](https://www.epa.gov/newsreleases/epa-orders-cleanup-following-battery-fire-gateway-energy-storage-facility-san-diego) | 250 MW | Burned 11 days, EPA-ordered cleanup |
| Jan 2025 | [Moss Landing, CA](https://www.epa.gov/ca/moss-landing-vistra-battery-fire) | 300 MW | 1,200–1,500 evacuated, largest EPA lithium-ion cleanup in history |

### What comes out of a lithium-ion battery fire

- **Hydrogen fluoride (HF):** 20–200 mg per Wh of capacity. Causes deep tissue burns and pulmonary edema.
- **Heavy metals:** Researchers at Moss Landing found nickel, manganese, and cobalt deposited in surrounding marsh soil at hundreds to over a thousand times pre-fire concentrations at some sampling locations.
- **PFAS:** A 2025 study found per- and polyfluoroalkyl substances in lithium-ion battery fire soot.
- Carbon monoxide, hydrogen cyanide, sulfur dioxide, and various volatile organic compounds.

### Reignition

These fires come back. Undamaged cells in a partially burned facility still hold energy, and that energy can reignite days or weeks later. Gateway reignited repeatedly over 11 days.

### Why this site is different

The Snoqualmie Valley is ridge-bounded. Temperature inversions in western Washington valleys can trap smoke and gas close to the ground, nothing like a coastal site such as Moss Landing where wind disperses emissions.

Fisher Creek runs through the parcel with an unmapped floodplain less than 10 vertical feet from the development area. Contaminated firefighting runoff would reach the creek.

Snoqualmie Ridge has limited ways out: Snoqualmie Parkway and SR-18. Moss Landing evacuated 1,200–1,500 people. Snoqualmie Ridge is bigger.

## Sodium-ion

Sodium-ion is a class of battery chemistries, not a single technology. Safety characteristics vary by formulation. [Peer-reviewed research](https://www.mdpi.com/2313-0105/10/10/370) shows sodium-ion as a class has higher thermal runaway onset temperatures and lower pressure buildup than lithium-ion, but some sodium-ion chemistries can still experience thermal runaway under extreme conditions. The degree of improvement depends on the specific cathode, electrolyte, and cell design.

The comparison below reflects Peak Energy's NFPP chemistry, which is what Jupiter Power has contracted for other projects.

| Technology | Fire Risk | Toxic Emissions | Noise | Grid-Scale Ready? |
|---|---|---|---|---|
| Lithium-ion (NMC) | High | High (HF, heavy metals) | High (active cooling 24/7) | Yes |
| Lithium-ion (LFP) | Moderate | Moderate (HF still produced) | High (active cooling 24/7) | Yes |
| **Sodium-ion (NFPP)** | **Very low** | **Low (no heavy metals, much less HF)** | **Low (passive cooling)** | **2026–2027** |

### Abuse testing {#abuse-testing}

Peak Energy's sodium-ion cells have been tested under the same mechanical abuse conditions that cause lithium-ion cells to catch fire, and they don't ignite:

- **Nail penetration and mechanical abuse:** CATL publicly demonstrated nail penetration, drill, and metal saw tests on sodium-ion packs without ignition. Cells also remain stable under crush testing. In comparative testing (CATARC), sodium-ion showed a 0% ignition rate vs. 23% for lithium-ion, where 85% of cells exceeded 200°C.
- **UL 9540A:** [Natron Energy](https://natron.energy/files/resources/natron-ul-9540a-module-report-revised-july-8-2020-final.pdf) was the first sodium-ion company to publish full UL 9540A results. Cells passed without needing additional safety controls.

### Peak Energy

Peak Energy's sodium-ion cells use an NFPP cathode (sodium iron phosphate pyrophosphate) with a non-flammable electrolyte. They've passed nail penetration, overcharge, and crush testing without thermal runaway. No cobalt, nickel, or manganese. Passive cooling only: no fans, no HVAC, no 24/7 noise. They're targeting cost parity with LFP and commercial-scale production in 2026–2027.

Jupiter Power signed a [$500M / 4.75 GWh deal with Peak Energy](https://www.prnewswire.com/news-releases/peak-energy-signs-4-75-gwh-contract-with-jupiter-power-for-industry-leading-sodium-ion-battery-storage-systems-302612467.html) for this technology. Their CTO called it a "potential game changer."

Cascadia Ridge isn't scheduled to come online until late 2028, after sodium-ion hits commercial scale. So why isn't Jupiter Power using it here?

## Why did lithium-ion get commercialized first? {#why-lithium-first}

Lithium-ion and sodium-ion were both researched starting in the 1970s. Lithium-ion won the race to commercialization because of energy density. Lithium is the lightest metal on the periodic table and has the highest electrochemical potential, which means more energy in a smaller, lighter package. When Sony commercialized the first lithium-ion battery in 1991, the market was portable electronics: laptops, camcorders, eventually phones. For those applications, energy density is everything. Sodium-ion couldn't compete on that metric and the research funding followed lithium-ion. The EV market in the 2010s reinforced the same dynamic: range anxiety means weight and size matter.

Sodium-ion got left behind because there was no market where its advantages mattered. It's heavier and lower energy density, which is disqualifying for anything you carry or drive.

What changed is stationary grid storage. A BESS sits on the ground. Nobody cares what it weighs. The metrics that matter are cost, safety, cycle life, and supply chain stability. Sodium-ion is competitive or better on all four. Sodium is the sixth most abundant element on earth, with no cobalt, nickel, or lithium supply chain risk. The market for utility-scale stationary storage at this scale basically didn't exist until renewable mandates like CETA created demand for it. That's why sodium-ion is reaching commercial scale now.

## Is sodium-ion unproven? {#sodium-ion-proven}

Sodium-ion doesn't have a long operational track record at grid scale. That's true. But the safety case for sodium-ion is fundamentally different from lithium-ion's.

Lithium-ion's risk comes from thermal runaway, and you can only learn how often that happens by running facilities for years and counting incidents. That's why the failure rate data matters and why the lack of data on aged systems is concerning.

Sodium-ion's safety case comes from the fact that the cells don't thermally run away in the first place. That's testable in a lab, and it's been tested. Peak Energy's NFPP cells have been through the same abuse testing protocols used for lithium-ion (nail penetration, crush, overcharge, saw) with a 0% ignition rate vs. 23% for lithium-ion. [Natron Energy](https://natron.energy/files/resources/natron-ul-9540a-module-report-revised-july-8-2020-final.pdf) published full UL 9540A results for sodium-ion before any commercial deployment, which is more pre-deployment safety data than lithium-ion BESS had when the industry started deploying it at scale.

The operational unknowns for sodium-ion are real: cycle degradation at scale, long-term maintenance costs, supply chain reliability. Those are commercial risks, not safety risks. A sodium-ion cell that degrades loses capacity. A lithium-ion cell that degrades can catch fire.

## Further reading {#further-reading}

- [Safety of sodium-ion batteries: prospective analysis from first generation towards more advanced systems](https://www.mdpi.com/2313-0105/10/10/370) (MDPI Batteries, 2024). Finds sodium-ion has higher thermal stability than lithium-ion but notes that safety varies by chemistry and that some sodium-ion formulations can still thermally runaway.
- [Thermal runaway hazards comparison between sodium-ion and lithium-ion batteries using accelerating rate calorimetry](https://www.sciencedirect.com/science/article/abs/pii/S095758202400716X) (Process Safety and Environmental Protection, 2024). Compared NTM sodium-ion, LFP lithium-ion, and NCM lithium-ion. Found sodium-ion thermal runaway characteristics closer to the safer LFP profile than to NCM.
- [Natron Energy UL 9540A module test report](https://natron.energy/files/resources/natron-ul-9540a-module-report-revised-july-8-2020-final.pdf) (PDF). First sodium-ion company to publish full UL 9540A results. Cells passed without additional safety controls.