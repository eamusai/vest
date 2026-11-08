# Child water-approach warning — highest priority

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Roadmap](decisions.md) · [Next steps](next-steps.md)

Research brief, version 0.1 — November 8, 2026. This is the project's highest-priority use case. No child-worn device, working alert system, field trial, or demonstrated protective benefit exists.

## Purpose

The central aim is to help save a child's life by warning a supervising parent or caregiver **before a young child who cannot yet swim reaches water they should not approach**. The proposed wearable, potentially integrated with a vest, estimates approach to a defined water hazard and sends a timely caregiver alert. The parent wants advance warning, rather than waiting for immersion.

The priority is the child-protection problem, not a particular garment, sensor, or inflation mechanism. The earlier adult boating study remains a secondary track. Adult equipment choices and the adult appearance illustration do not establish suitability for children.

The separate [harmful-water sensing idea](water-quality-use-case.md) would address specified contaminants, not drowning risk. Neither concept currently makes a lake visit safe, and a water-quality reading would not replace approach prevention or supervision.

An alert would be an additional aid. It cannot replace close, constant supervision, barriers that restrict access, or appropriate existing water-safety measures. CDC emphasizes supervision and pool fencing; no evidence reviewed here establishes that this concept prevents drowning. [CDC prevention guidance](https://www.cdc.gov/drowning/prevention/index.html)

## Intended flow

1. A caregiver identifies the hazard and a proposed warning boundary, with a separate confirmation of which child and receiving device are paired.
2. The wearable system estimates the child's position relative to that boundary, including uncertainty and the age of its information.
3. A possible approach or boundary crossing produces a distinguishable alert on a caregiver receiver. A phone is one candidate; a dedicated receiver is another.
4. The alert identifies which paired wearable needs attention. Delivery and acknowledgment are recorded separately; acknowledgment does not prove that the child is safe.
5. Lost position, stale data, a removed wearable, low power, or a failed connection must have explicit unavailable/fault behavior rather than silent reassurance. Whether each fault can be detected is itself a requirement to evaluate.

No warning distance, response-time guarantee, operating range, battery target, or automatic inflation rule has been selected. Absence of an alert must never be presented as proof that a child is away from water. This concept is a warning system, not a physical access barrier.

## What "near water" requires

Distance to a parent is not distance to a water edge. A wetness sensor detects contact after it happens; that does not satisfy the advance-warning aim. A positioning system also needs a trustworthy description of the hazard: a device can estimate location without knowing where water is.

The first research candidate is a **known, fixed hazard boundary**, such as a mapped pool perimeter with any necessary local infrastructure. This is a proposed starting setting, not a selected deployment site or endorsement of a product. Arbitrary lakes, shorelines, canals, temporary water, changing water levels, and unfamiliar locations remain broader ambitions with additional mapping and sensing questions. A map must not imply coverage of unrecorded water hazards.

| Evidence or candidate | What it offers | Limit for this concept |
| --- | --- | --- |
| [GPS.gov accuracy guidance](https://www.gps.gov/gps-accuracy) | Smartphone GPS commonly has errors of several meters even under open sky, with worse conditions around obstructions. | Our inference: ordinary phone-style GPS alone is not an established precise pool-edge warning system. Map error and stale fixes compound the problem; no universal safe geofence radius follows from this source. |
| [Android UWB documentation](https://developer.android.com/develop/connectivity/uwb) | Ultra-wideband supports ranging between compatible devices, making local reference devices a candidate to investigate. | Ranging to a device does not automatically identify the water boundary. Placement, body blockage, real-world error, compatibility, and multi-child operation need evaluation. The documented Android API also limits background ranging reports; a background phone alert cannot be assumed to work. |
| [CDC prevention guidance](https://www.cdc.gov/drowning/prevention/index.html) | Established guidance centers supervision, restricted pool access, and appropriate life jackets. | It does not validate this wearable or establish that a notification adds protection. The research must examine false reassurance as well as technical performance. |

These primary sources were opened on November 8, 2026. They support requirements and limitations, not product selection or a complete review of existing child alarms. Comparing existing boundary, gate, and immersion alarms is still needed, with their trigger conditions kept distinct.

## Requirements to investigate first

- **Useful warning time:** include sensor updates, uncertainty, processing, delivery, recognition, and caregiver response. An alert generated before a crossing may still arrive too late. No buffer is assumed adequate without evidence.
- **Missed events and nuisance alerts:** assess varied paths, speeds, postures, clothing, obstructions, and boundary errors. Frequent false alarms may encourage muting or abandonment.
- **End-to-end delivery:** examine locked phones, app suspension, notification settings, radio dropout, receiver separation, discharged batteries, and multiple wearables. A transmitted message is not necessarily an alert a caregiver notices.
- **Pediatric wearability:** evaluate fit, removal, snagging, small parts, battery enclosure, skin contact, and interference with approved child equipment with relevant specialists. Do not scale the adult concept down and assume it is suitable.
- **Caregiver responsibility:** clarify pairing and handoff between adults, and which receiver is actively responsible. Avoid an interface that encourages caregivers to step away because monitoring appears active.
- **Privacy:** use secure, explicit caregiver pairing; minimize location storage and retention; avoid public child-location feeds. No child identities, household locations, or family movement records belong in this public research repository.

## Review package and evaluation path

The first review package is drafted:

- [Requirements, open parameters, and candidate approaches](child-warning-requirements.md): 16 proposed obligations, with a fictional fixed lake-shore segment as the first desk model.
- [Failure-scenario register](child-warning-failure-scenarios.md): 17 scenarios and a blank evidence record, including multiple wearables, handoff, timing, and compound failures.
- [Caregiver paper mock-up](child-caregiver-alert-mockup.md): seven draft screens; acknowledging a message does not clear its warning.
- [Staged evaluation plan](child-warning-evaluation-plan.md): review questions, decision register, and evidence gates before any field work.

Review this package with pediatric water-safety, human-factors, and positioning specialists before choosing hardware. Establish acceptance criteria before collecting performance data; successful demonstrations alone would not establish reliability. No specialist review or performance study has occurred.

Begin any later feasibility work with synthetic trajectories and inert tags or adult-operated surrogates in a dry area with a simulated boundary, away from water. Measure missed/late alerts, false alerts, uncertainty, delivery and acknowledgment delays, and fault visibility. Include failures such as a moved reference device, outdated boundary, and disconnected receiver. No child exposure, water-entry trial, deliberate supervision lapse, or recruitment is proposed here.

Only after reviewed evidence supports further work should pediatric wearability or field studies be separately designed and authorized. Alerting, flotation, and automatic inflation require distinct evidence. Saving a child's life is the purpose; it is not a result this project can yet claim.
