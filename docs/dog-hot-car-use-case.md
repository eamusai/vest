# Dog left in a hot car: detection and emergency alerts

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Child hot-car case](child-hot-car-use-case.md) · [Next steps](next-steps.md)

Research brief, version 0.1 — source review November 8, 2026. No canine device, heat-exposure study, emergency integration, or protective benefit has been demonstrated. This is a separate animal-welfare research case; child water-approach warning remains the highest priority.

## Intended outcome and evidence boundary

A dog wears a device that recognizes possible unattended presence in a vehicle and concerning heat conditions, alerts a responsible person, and escalates to appropriate emergency responders through an established service. The intended outcome is timely physical assistance, not merely a recorded alarm.

CDC advises never leaving pets in parked cars and explains that an open window is not adequate protection. This concept does not make leaving a dog in a vehicle acceptable or establish a safe waiting period. [CDC heat and pets guidance](https://www.cdc.gov/heat-health/risk-factors/heat-and-pets.html)

The pediatric case provides useful questions about communications and occupancy, but **not canine physiological thresholds, fit, or validation**. A veterinarian must help define intended dogs and exclusions, including how conformation, coat, age, health, acclimatization, and activity might affect measurements and risk. No wearable measurement is currently validated here as a heatstroke diagnosis.

## Candidate observations

| Observation to investigate | What it might contribute | What must not be assumed |
| --- | --- | --- |
| Device worn/contact and independent occupancy information | Distinguish a dog present from an empty vehicle or abandoned device | A wearable alone covers an untagged dog or one that removes it. |
| Paired vehicle/trip information | Support an inside-vehicle context | Proximity to a parked car establishes confinement. |
| Caregiver separation and supervision handoff | Identify possible unattended occupancy before heat illness | A nearby phone means the dog is supervised. |
| Environmental temperature, trend, and sensor quality | Describe local conditions and measurement uncertainty | Under-coat, surface, cabin, and core temperatures are interchangeable. |
| Motion or other veterinary-supported signals | Add context if independently validated | Panting, stillness, or a single physiological change gives a reliable diagnosis. |

Compare a wearable with vehicle occupancy sensing and a combined approach. Consider transport crates and multiple dogs explicitly. Monitoring cannot depend on the dog reacting to an alarm, pressing a control, or escaping the vehicle.

## Proposed response plan

Recognize possible unattended occupancy early; do not wait for clinical collapse or a guessed heat threshold. Attempt caregiver and backup alerts, and investigate local alerts where they would be useful without causing additional distress. The dog's welfare must be considered when selecting any sound or vibration.

The intended automatic emergency escalation needs a defined local destination. Depending on jurisdiction and circumstance, the response plan may involve an emergency communications center, animal-control service, police, or a staffed monitoring service that can reach the appropriate responders. Emergency veterinary care is a related pathway, but contacting a clinic does not itself arrange access to a locked vehicle. No destination or agreement is selected here; local acceptance and responsibilities must be confirmed before a product claim.

Use the same distinction between **event detected → message sent → recipient accepts → any dispatch confirmed → physical resolution** as in the child case. For an actual emergency call, the National 911 Program asks callers to provide location, callback information, and details of the emergency. For this proposed integration, also identify the vehicle and dog, observation age, uncertainty, and available responsible contact. Its guidance does not establish automated acceptance or a universal response for animal incidents. [Calling 911](https://www.911.gov/calling-911/)

Acknowledgment alone must not cancel an unresolved warning. An unreachable owner must not indefinitely block escalation. Conversely, lack of feedback from a responder must never be displayed as confirmed rescue. Cancellation rules, repeated-message handling, escalation timing, and fallback coverage require joint operational and veterinary review. The initial study uses simulated recipients only, not real emergency calls.

## Proposed requirements and failure cases

| Requirement to investigate | Representative failure scenario |
| --- | --- |
| Detect unavailable or removed wearables where feasible, and state coverage gaps. | Chewed strap, slipping garment, depleted battery, or device left in a crate without the dog. |
| Preserve unresolved alerts when connectivity changes. | Phone left in car; application closed; cellular dead zone; backend outage. |
| Separate each animal and its responsible person. | Two dogs share a vehicle; tags are swapped; a sitter has not accepted handoff. |
| Expose location age and uncertainty. | Underground garage, incorrect vehicle pairing, or stale position. |
| Distinguish environmental trends from sensor faults. | Sensor against the coat, direct sun, water exposure, calibration drift, or delayed readings. |
| Assess fit and heat burden across the intended population. | Rubbing, restricted movement, added insulation, entanglement with crate/restraint, or chewing exposed components. |
| Treat power, communications, or cooling-system failure as uncertainty. | An operating air conditioner or engine is incorrectly treated as a permanent guarantee of safety. |
| Protect location and owner information. | Unnecessary tracking retention, unauthorized pairing, or disclosure to the wrong recipient. |

No automatic inflation, sedation, vehicle unlocking, or escape mechanism is included in this initial concept. Garment design must not create more risk than the sensing function might reduce.

## Evidence needed before further work

First specify the target dogs, transport settings, comparator systems, and responder jurisdiction with veterinary and emergency-operations expertise. Set separate canine acceptance criteria for detection, missed events, nuisance alerts, latency, freshness, power availability, and escalation failure. Do not reuse pediatric limits or publish a “safe temperature” from a speculative sensor model.

Begin with fictional incident walkthroughs and simulated streams. A later, separately reviewed bench study could use inert dog-shaped fixtures, independent environmental references, and communications fault injection. No dog or other living subject is to be left in a vehicle or heated for testing. Animal wearability studies, if justified later, need veterinary and welfare review, owner consent, ordinary comfortable conditions, and stop rules.

The next deliverable is a bounded feasibility and response specification. No evidence yet shows that this proposal can detect every incident, bring responders in time, or prevent injury.
