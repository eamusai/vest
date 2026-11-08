# Child-warning evaluation plan and open decisions

[Requirements](child-warning-requirements.md) · [Failure scenarios](child-warning-failure-scenarios.md) · [Paper mock-up](child-caregiver-alert-mockup.md) · [Next steps](next-steps.md)

Version 0.1 — November 8, 2026. Proposed research progression. This package contains documentation and simulated interface material only. It is not a protocol approval, completed expert review, or permission to expose children to a hazard.

## Stage gates

| Stage | Work and deliverable | Exit evidence | Current status |
| --- | --- | --- | --- |
| A — Document preparation | Define scope, candidate approaches, requirements, failure scenarios, and alert copy. | Links and traceability checked; limitations and unresolved parameters explicit; simulated acknowledgment preserves warnings. | Draft package created. Internal document/interface checks only. |
| B — Specialist review | Review water-boundary assumptions, caregiver behavior, pediatric suitability, sensing options, and architecture failures. | Recorded review by relevant specialists; dispositions for each issue; agreed initial scope and numerical performance criteria. | Not conducted. No reviewers contacted or appointed. |
| C — Synthetic feasibility | Build a separately scoped test model with known trajectories, independent event truth, delayed/missing reports, and fault injection. | Reproducible cases across F01–F17, frozen criteria, denominators and timing uncertainty; no unreported misses or excluded outage time. | Proposed; no detector or trajectory simulator implemented. |
| D — Dry surrogate feasibility | Under a reviewed plan, compare candidate positioning hardware with independent reference measurements in a dry area away from water. | Error distributions and tails by condition, latency, fault behavior, power limits, nuisance/missed/late events; independent review of remaining risk. | Proposed; no equipment selected or obtained. |
| E — Human-factors and pediatric decisions | Separately review caregiver comprehension studies and any later child-specific fit research, with consent, privacy, and stopping rules. | Justified protocols and qualified oversight appropriate to the activity. No claim that laboratory performance proves protection. | Proposed; no recruitment, fit work, or field deployment. |

Later field validation, standards/regulatory review, manufacturing quality, and product claims require additional work; this outline is not an exhaustive certification path. Progress may stop or redirect at any gate.

## Measures to define and preserve

For each approach event, preserve an independent onset definition and whether the warning was presented before the required deadline. Record the path, boundary revision, conditions, and unavailable intervals. Collect sensing, processing, transport, presentation, acknowledgment, and response times separately where measurable; report unavailable measurements explicitly.

Minimum reporting categories are event count, missed events, late events, false warnings per observation time, coverage/unavailable time, position and boundary error distributions, data age, stage delays, and fault detection/recovery behavior. Caregiver understanding and response belong to separate approved studies, not inferred from a button click. Evaluate simultaneous wearables and compound failures rather than only isolated happy paths.

Before any performance study, freeze the intended population/setting, target rates and time budgets, independent truth method, conditions, exclusions, and analysis. Determine sample size from those targets and a justified uncertainty analysis. Do not choose a reassuring success percentage or run count without that work. Hold out complete paths/sessions/conditions when evaluating a tuned model; avoid treating neighboring samples from one event as independent events.

## Immediate review decisions

| Decision | Proposed working assumption | Needed to resolve it |
| --- | --- | --- |
| Initial environment | A fictional, fixed lake-shore segment represented in dry space; no real water exposure. | Review whether this captures the intended approach problem and what lies outside coverage. |
| Wearable vs. garment | Evaluate the warning function before committing to an inflatable vest or child garment. | Pediatric fit and foreseeable-misuse requirements; no scaled-down adult design. |
| Positioning | Compare GPS/map and local ranging/reference approaches; select neither yet. | Measured error/latency feasibility, deployment burden, boundary assurance, and receiver constraints. |
| Receiver | Compare a phone with a dedicated local receiver. | What happens when the receiver cannot show its own failure, or the phone is suspended/muted/off? |
| Warning and fault behavior | Preserve unresolved approach warnings when information is lost; acknowledgment is receipt only. | Specialist agreement on prioritization, repetition, recovery, and caregiver comprehension. |
| Multiple caregivers | Explicit acceptance for a transfer; no silent inference of supervision. | Handoff failure review, overlapping alerts, and continuity requirements. |
| Numerical limits | All performance, timing, age/size, range, and power limits remain open. | Named review roles and documented rationale before performance testing. |
| Child privacy | Synthetic labels and maps only; no child location or family identifiers in the repository. | Later data-minimization, consent, access, retention, and deletion plan before collecting real records. |

## Questions for specialists

For pediatric water-safety and human-factors reviewers: could any status or warning encourage less supervision, what unintended responses might it provoke, and what evidence would show useful comprehension? What child-specific garment and attachment risks must be addressed before choosing a wearable form?

For positioning and reliability reviewers: how will boundary errors and changing shorelines be bounded, how often do large location errors occur, and how will the system reveal stale information, moved references, and unavailable receivers? Can a practical architecture deliver the required warning time under adverse conditions?

For study-design and privacy reviewers: what independent ground truth and sample sizes support the claims, how will missed/late events and unavailable time be reported, and what minimum data is necessary? Which observations can be collected without involving children or water exposure?

This is a reusable review brief. No messages have been sent to specialists, no participants recruited, and no study results recorded. The immediate next milestone is resolving Stage B decisions, followed by a separately scoped synthetic evaluation—not a family lake trial.
