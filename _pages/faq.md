---
title: "FAQ"
---

## What is a BESS? {#what-is-a-bess}

A Battery Energy Storage System (BESS) is a facility that stores electricity in large banks of batteries and releases it back to the grid when needed. The proposed Cascadia Ridge facility would be 130 MW / 520 MWh, enough to power roughly 100,000 homes for four hours. In practice, it's rows of battery modules in prefabricated enclosures, plus inverters (to convert DC to AC), transformers (to step up voltage), cooling systems, fire suppression equipment, and switchgear connecting to the transmission grid. This project would connect to PSE's existing Mt. Si substation via a 115kV tie-line.

## Why is PSE interested in having a BESS? {#why-pse}

Washington's [Clean Energy Transformation Act (CETA)](/ceta) requires utilities to be greenhouse gas neutral by 2030 and supply 100% clean electricity by 2045. Wind and solar don't generate power on demand. They produce when conditions are right, not necessarily when people need electricity. Storage bridges that gap: charge when renewables are overproducing, discharge during peak demand. Without storage, PSE either overbuilds generation (expensive for ratepayers) or keeps fossil fuel peakers running (which violates CETA). PSE's Mt. Si substation sits adjacent to the proposed site, making it a logical interconnection point.

## Why not build it somewhere away from residential areas? {#why-here}

Storage needs to be near where power is consumed, not where it's generated. You can't put a battery next to a wind farm in Eastern Washington and expect it to help the Eastside during peak demand without expensive new transmission lines. Transmitting stored power long distances means energy losses both ways, and building new long-distance transmission is slow to permit and faces its own opposition.

PSE's Mt. Si substation sits right next to this site. It's an existing grid interconnection point where PSE needs capacity. The electrical interconnection makes sense. But PSE's own [siting study](/project#siting-study) screened out Mt. Si because of what surrounds it: homes, schools, and constrained land use. The study's "Good Neighbor" criteria flagged exactly the conditions that exist here.

That's the core problem. The grid connection is real, but so are the siting constraints. With sodium-ion, many of those constraints (thermal runaway, toxic emissions, cooling noise) go away. With lithium-ion, they don't. Sodium-ion batteries can do the same job at this location without the thermal runaway risk. Lithium-ion was the standard when PSE's RFP was issued, but sodium-ion is now commercially available and Jupiter Power has already signed a [$500M sodium-ion deal with Peak Energy](https://www.prnewswire.com/news-releases/peak-energy-signs-4-75-gwh-contract-with-jupiter-power-for-industry-leading-sodium-ion-battery-storage-systems-302612467.html) for other projects. What doesn't belong next to homes is a chemistry that can produce uncontrollable fires and toxic hydrogen fluoride gas when it fails.

## What are the concerns? {#concerns}

The proposed facility would use **lithium-ion batteries**. Community concerns include:

- **Fire:** Lithium-ion cells can undergo thermal runaway, an uncontrolled, self-sustaining temperature rise that can cascade through an entire facility. EPRI tracks two failure metrics. For a 130 MW facility like Cascadia Ridge, the [15-year compound probability ranges from 4.4% to 45%](/fire-risk) depending on which metric you use. Recent incidents at [Moss Landing, CA](https://www.epa.gov/ca/moss-landing-vistra-battery-fire) and [Gateway, San Diego](https://www.epa.gov/newsreleases/epa-orders-cleanup-following-battery-fire-gateway-energy-storage-facility-san-diego) required evacuations and EPA-ordered cleanups. Existing [safety standards](/fire-risk#safety-standards) (NFPA 855, UL 9540A, IFC 1207) set requirements for detection and suppression, but there are no federal siting standards and no national consensus on setbacks from homes.
- **Toxic emissions:** Lithium-ion battery fires produce hydrogen fluoride, heavy metals, and other hazardous compounds. [Larsson et al. (2017)](/assets/larsson-2017-hf-emissions.pdf) measured 20-200 mg of HF per Wh of capacity; scaled to Cascadia Ridge, even a fire involving 1% of the facility could produce over a metric ton of HF. The site is adjacent to Fisher Creek (salmon habitat) and thousands of homes on Snoqualmie Ridge.
- **Noise:** Lithium-ion systems require active cooling: fans and HVAC running around the clock.
- **Battery chemistry:** Jupiter Power has signed a [$500M sodium-ion deal with Peak Energy](https://www.prnewswire.com/news-releases/peak-energy-signs-4-75-gwh-contract-with-jupiter-power-for-industry-leading-sodium-ion-battery-storage-systems-302612467.html) for other projects. Peak Energy's NFPP chemistry has shown no thermal runaway in abuse testing and uses passive cooling. Sodium-ion grid storage is already commercially available and deployed in the US.
- **Proximity** to neighborhoods, parks, and schools, and potential impacts on property values.
- **Land use:** Snoqualmie's Comprehensive Plan designates this land for business park and mixed use, not industrial battery storage.

## Who will decide whether the proposed BESS project will be approved? {#who-decides}

**King County.** The site is in unincorporated King County, so the City of Snoqualmie has no jurisdiction even though Snoqualmie Ridge residents are the most directly affected. Under the site's UR zoning and [King County Ordinance 19824](/permitting), BESS is a permitted use. No Conditional Use Permit and no public hearing are required. The main avenue for public input is the **21-day SEPA comment period** that opens when Jupiter Power files a new permit application.

Councilmember Sarah Perry (District 3) sponsored the BESS ordinance. The City of Snoqualmie has identified this area as a potential annexation area. If annexed, the city's Comprehensive Plan would apply.

## What happens to a lithium-ion BESS in an earthquake? {#earthquake}

The Snoqualmie Valley is exposed to the [Southern Whidbey Island Fault](https://washingtondnr.wpcomstaging.com/2009/09/11/southern-whidbey-island-fault-zone-mapped-through-snoqualmie-valley/) (mapped through the valley, M6.5–7.4), the Seattle Fault (M7.0–7.5), and the Cascadia Subduction Zone (M9.0+). [USGS Fact Sheet 2025-3050](https://doi.org/10.3133/fs20253050) (September 2025) puts the 50-year probabilities for the Puget Sound region at 85% for a M6.5+ deep earthquake, 17% for a M6.5+ crustal fault earthquake, and 10-15% for an approximately M9 Cascadia Subduction Zone event. Lab testing shows lithium-ion cells can develop internal short circuits, the initiating event for thermal runaway, from small mechanical deformations.

King County's ordinance requires IEEE 693 seismic qualification, which keeps equipment on its mounts. But nobody has tested whether utility-scale BESS enclosures protect cells the way crash-tested EV packs do. And there's no requirement to model the full chain: earthquake damages cells → thermal runaway → fire → contaminated runoff into Fisher Creek, all while evacuation routes may be damaged. No utility-scale BESS has been tested by a major earthquake. See the [earthquake risk section](/fire-risk#earthquake-risk) of our fire risk analysis.

Sodium-ion chemistries like Peak Energy's NFPP have shown no thermal runaway in abuse testing, so the earthquake-to-fire chain would not apply.

## If lithium-ion batteries are sensitive to vibration, why are they safe in cars and planes? {#ev-vibration}

Different kind of stress. Driving and flying produce low-amplitude, high-frequency vibration. EV and aircraft battery packs are purpose-built for that: cells are locked into rigid, crash-tested enclosures with vibration isolation and per-cell monitoring. The cells don't move relative to each other.

Earthquake shaking is the opposite: high-amplitude, low-frequency. It's more like a car crash than road vibration. And lithium-ion EV crashes *do* cause fires. That's well documented.

The packaging matters too. An EV battery is a sealed, crash-engineered unit. A utility-scale BESS is rack-mounted modules in shipping containers, designed for stationary use. IEEE 693 keeps the racks on their mounts, but the cell-level containment inside the modules isn't crash-tested the way an EV pack is. Nobody has tested whether utility-scale BESS enclosures protect cells during seismic shaking the way an EV pack protects them during a crash.

## Getting the facts right {#fact-check}

Our community's opposition is strongest when it's accurate. Some claims circulating in public comment and social media need correction. The real facts are alarming enough.

### McMicken, Arizona (2019): firefighters were injured, not killed

Four firefighters were hospitalized (one critically) when an unvented battery container exploded at the McMicken BESS facility in Surprise, Arizona. None died. The explosion occurred when first responders opened the container door and flammable gas that had accumulated inside ignited. The real lesson is about deflagration venting and gas accumulation, and Jupiter Power has not disclosed their venting design for Cascadia Ridge. That's worth raising. But claiming firefighters died weakens the argument when someone checks.

### Moss Landing evacuation: 1,200-1,500 people, not 15,000

The January 2025 Moss Landing fire evacuated approximately 1,200 to 1,500 people. The larger number may reflect the broader area population, but it wasn't the evacuation count. The accurate comparison is actually worse for us: Moss Landing is a smaller community with more ways out, and the evacuation still took over 25 hours. Snoqualmie Ridge is bigger, has two primary egress routes, and demonstrated gridlock during the December 2025 floods. The real numbers make the case.

### Monitoring: automated systems exist, but the gaps are real

BESS facilities have continuous automated monitoring through battery management systems (BMS) that track temperature, voltage, and state of charge around the clock. Saying "there is no monitoring" is easy to rebut and makes the community look uninformed.

The real gap is different and worth pressing on: there is no requirement for permanent **fenceline air quality monitoring** at BESS facilities. At Moss Landing, EPA deployed monitoring stations reactively, after the fire started. There is also no requirement for soil or water monitoring near adjacent waterways. And "monitoring" through a BMS is not the same as having trained personnel on site. Jupiter Power has indicated the facility would not be permanently staffed. These are the questions that matter, and they don't require exaggeration to be alarming.

### Failure rates: use the range, not just the high number

EPRI data supports two failure rate metrics. The per-project rate (0.3%/year, treating all facilities equally regardless of size) yields a 15-year probability of about 4.4%. The per-GW rate (0.2-0.3 failures/GW/year, adjusted for the 130 MW capacity) yields about 45%. The actual risk is somewhere in that range. Citing only the 45% number without context invites a rebuttal that discredits the entire argument. Presenting both numbers and explaining the difference is more persuasive and harder to dismiss. See [fire risk](/fire-risk) for the full analysis.

## What can I do? {#take-action}

See [Take Action](/take-action) for specific steps: who to contact, what to ask for, and how to make your voice heard.
