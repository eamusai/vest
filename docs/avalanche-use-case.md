# Avalanche use case: breathing space, activation, and rescue

[Home](../README.md) · [Decisions](decisions.md) · [Next steps](next-steps.md)

Research brief, version 0.1 — source review November 8, 2026. Added at the user's request. No avalanche equipment has been selected, purchased, modified, or tested for Vest. This is a research concept, not a rescue procedure or a promise of survival.

## Scenario and user intent

An adult skier or snowboarder is caught in an avalanche and may become buried, unable to move their arms, reach a trigger, use a phone, or help themselves. The desired outcome is to improve the opportunity for rescue without requiring action from an incapacitated wearer.

The user proposed three related ideas: inflate to make space around the person; deflate enough to leave breathing room; and potentially detect the avalanche automatically and use the inflated chamber's air to support breathing until help arrives. Preserve each as a question. Neither successful detection nor sufficient breathable air until rescue is established.

Working context: recreational avalanche terrain with companions. This assumption needs confirmation; it is not a solution for solo burial, all snow conditions, children, or every winter activity. Prevention, terrain decisions, local forecasts, training, and practiced companion rescue remain essential. [SLF prevention guidance](https://www.slf.ch/en/avalanches/avalanche-science-and-prevention/)

## Distinguish the jobs

| Job | Existing approach | Boundary for Vest |
| --- | --- | --- |
| Reduce burial during a moving slide | Avalanche airbags increase a person's effective volume to exploit segregation in flowing snow. | This mechanism does not establish that inflation will lift a person out of settled debris. |
| Leave space near the airway | Some airbags actively deflate after deployment, potentially leaving an air pocket. | The space must reach the mouth/nose and remain open; a cavity elsewhere is not sufficient. |
| Maintain breathable air after burial | Air-diversion or airflow devices address oxygen supply and exhaled carbon dioxide. | A space alone is not a sustained breathing system. |
| Locate and recover the person | Avalanche transceiver, probe, shovel, and trained companions. | A satellite distress alert does not replace local burial search and excavation. |

Sources: [airbag mechanism research](https://www.slf.ch/fileadmin/user_upload/WSL/Mitarbeitende/zweifelb/2012_ISSW_airbags.pdf), [WMS 2024 guidance](https://journals.sagepub.com/doi/full/10.1016/j.wem.2023.05.014), and [Avalanche Canada equipment guidance](https://avalanche.ca/gear). A transmitting avalanche transceiver already supports being located without a button press after the accident; it requires correct preparation and equipped rescuers.

## What already exists, and what the evidence says

**Inflated avalanche airbags:** Haegeli and colleagues' 2014 retrospective accident study reported lower adjusted mortality with inflated airbags. Non-inflation was an important limitation. Historical observational data are not a current failure rate for every model and do not validate automatic activation or our design. [Study abstract](https://pubmed.ncbi.nlm.nih.gov/24909367/)

**Inflate, then deflate:** PIEPS describes JetForce BT automatic deflation three minutes after deployment to create air space. This is existing product behavior, not a timing prescription for Vest. [Manufacturer description](https://www.pieps.com/en/product/jetforce-bt-35/)

A 2020 study examined 12 volunteers in controlled snow burial: the airbag deployed before burial was completed and later deflated. Eleven completed the 60-minute observation. The setup included respiratory measurement apparatus and medical monitoring; comparisons used historical controls. It supports investigation of post-deflation space, not a guaranteed survival duration, inflation against already-compacted snow, or a self-contained breathing reservoir. The WMS guideline rates the evidence for deflation-created pockets as low quality. [Original study](https://utahavalanchecenter.org/sites/default/files/attached_files/Avalanche%20airbag%20post-burial%20active%20deflation.pdf), [WMS guidance](https://journals.sagepub.com/doi/full/10.1016/j.wem.2023.05.014)

**Active airflow:** Safeback SBX uses a fan to move air from surrounding snow toward the breathing area without a mouthpiece. The manufacturer describes handle activation and integration into specified compatible carriers, including the Db Snow Pro Vest 8L. This establishes a relevant existing vest comparator, not a selection or recommendation. It also means the handle may remain a limitation for someone incapacitated before activation. [SBX description](https://www.safeback.no/sbx), [vest integration](https://www.safeback.no/products/db-snow-pro-vest-8l)

The 2025 randomized SBX trial analyzed 24 participants from 36 randomized and found delayed critical hypoxemia and hypercapnia in simulated burial. Outcomes were physiological surrogates, not real-avalanche mortality. Healthy volunteers, controlled posture/depth, possible inlet/outlet obstruction, and untested chest restriction limit generalization. Safeback supplied devices and batteries. This does not establish a guaranteed wait for rescue or validate our proposed reservoir. [Original JAMA paper hosted by SLF](https://www.slf.ch/fileadmin/user_upload/WSL/Mitarbeitende/schweizj/Eisendle_etal_Respiratory_gas_shifts_avalanche_burial_jama_2025.pdf)

## Developing the proposed concept

### Automatic detection and activation

The hypothesis is that detecting involvement early could help when a wearer cannot pull a handle. It is not an implemented or validated feature. A later requirements study should distinguish skiing, ordinary falls, jumps, transport, and lift use from avalanche involvement. Measure missed events, false activations, and activation delay; motionlessness alone cannot establish burial. Retain independent manual activation as a candidate requirement, subject to manufacturer review.

Detection during movement and detection after burial are different tasks. A detector that identifies burial only after snow has settled may be too late for the airbag's burial-reduction mechanism. No sensor combination, threshold, automatic deflation rule, or deployment timing is selected here. Bench replay cannot establish real-avalanche reliability.

### Inflate to create space, then partially deflate

Separate deployment before/during the slide from attempted expansion after burial. For the latter, the unknown is whether a chamber can displace snow without transferring dangerous loads to the chest, neck, or face. For either, investigate cavity location, collapse after deflation, posture, snow properties, and the tradeoff between retained volume and breathing space. A timer by itself does not prove the avalanche has stopped or exclude a second slide.

These are proposed engineering questions, not demonstrated mechanisms or dimensions for a build. Existing equipment should not be modified to try them on a person.

### Breathe from the inflated chamber

Inflator contents are not automatically breathing air. Mammut documents nitrogen in a carbon cartridge; Alpride documents CO2/argon cartridges for specified systems. BCA documents compressed-air inflation in its Float systems. These distinctions do not establish that any complete airbag's contents, materials, or gas path are suitable for respiration. [Mammut data sheet](https://static.mammut.com/file/Data_Sheet_-_Carbon_Cartridge_Non-Refillable_300_Bar.pdf), [Alpride cartridge specification](https://www.alpride.com/product-page/alpride-cartridge-set-co2-argon), [BCA explanation](https://backcountryaccess.com/en-us/support/faqs-float-avalanche-airbags)

Do not route an existing inflation cylinder or bladder to a person's airway. A breathing reservoir would need separate validation of gas composition and cleanliness, delivery pressure and resistance, exhaled-CO2 handling, usable capacity, leakage, and failure behavior. Drawing air from the chamber also reduces the volume doing the airbag's other job. Chamber volume alone cannot justify a rescue-time claim.

Ambient airflow support, a stored breathing-air reserve, and mechanically assisting ventilation are different architectures. None automatically opens a blocked airway or overcomes restricted chest movement. An incapacitated person may also be unable to acquire or retain a mouthpiece. Those limitations make respiratory and mountain-rescue expertise necessary before selecting any breathing architecture. [WMS physiology and device guidance](https://journals.sagepub.com/doi/full/10.1016/j.wem.2023.05.014)

## Requirements to investigate

The following are proposed evaluation questions, not passed requirements:

| Area | Evidence needed before advancing |
| --- | --- |
| Wearability and retention | Fit over winter layers; unobstructed skiing/snowboarding motions; retention and access with gloves under the exact carrier instructions. |
| Breathing space | Mannequin measurements of cavity location and persistence, plus body loads across postures and representative snow conditions. |
| Air supply | Specialist bench measurements of gas quality, flow/resistance, CO2 clearance, blockage, icing, and depletion behavior. No human breathing trial. |
| Activation | An independently reviewed event dataset, explicit missed/false-event definitions, and timing results before any deployment claim. |
| Rescue compatibility | Preserve transceiver operation and probe/shovel access; evaluate electronics, magnets, heaters, and fans as interference sources. |
| Readiness | Traceable manufacturer checks, cold-condition power limits, service/recall status, and unambiguous failure indicators. |

[UIAA interference guidance](https://theuiaa.org/documents/safety/UIAA-Avalanche-Beacons-Recommendation.pdf) identifies possible interference from electronics and some electric airbags. Adding electronics near a transceiver therefore requires compatibility evaluation in both transmit and search modes. A successful power-on check is not proof of compatibility.

## First research step and boundaries

Start with a tabletop comparison of existing deflating airbags, airflow systems, and carriers against the three user ideas. Review exact manuals and product combinations before choosing reference equipment. The [SBX manual landing page](https://www.safeback.no/sbx-user-manual) is located, but its manual and all candidate carrier/airbag instructions have not been fully reviewed. No compatibility between JetForce and SBX is asserted.

Then propose a separate dry usability session: identify matching instructions, interpret staged readiness examples, locate controls on inert mock-ups while wearing gloves, and assess movement and rescue-tool access. Record omissions, confusion, help needed, access time, and discomfort. Use the water study's documentation principles, but do not reuse its participants, sample allocation, or answer key without a new protocol. There is no current avalanche pilot authorization or completed test.

Only after a justified unmet need is identified should specialists develop a mannequin/bench protocol for cavity mechanics, airflow, or detection. No live-avalanche exposure, human burial, breath restriction, pressure loading of people, modified safety gear worn in the field, or casual emergency broadcasts belong in this initial work. Bench success would still not establish a survival benefit.

Open decisions: intended setting and companion availability; which failure of existing equipment matters most; whether the user chiefly wants burial prevention, breathing space, or assistance after incapacitation; and which specialists and manufacturers can evaluate it. A single water-and-snow vest is not assumed. Water buoyancy, marine alerting, avalanche air pockets, and burial search remain separate requirements.

All cited URLs returned source material or a source landing page at review. Retrieval is not full manual verification. Licensing remains undecided; the repository stays private and no manufacturer manuals or drawings are copied here.
