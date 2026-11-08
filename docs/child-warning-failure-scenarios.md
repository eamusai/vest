# Child-warning failure scenarios

[Requirements](child-warning-requirements.md) · [Caregiver mock-up](child-caregiver-alert-mockup.md) · [Evaluation plan](child-warning-evaluation-plan.md)

Version 0.1 — November 8, 2026. A proposed scenario register, not test results or an exhaustive hazard analysis. All subjects, locations, and events are synthetic. No child or water exposure is proposed.

## Scenario register

The expected behavior is a requirement to review. It is not evidence that sensors can recognize the fault. "Unavailable" means the proposed information service cannot make its intended assessment; it does not mean the child is away from water.

| ID | Injected situation | Expected behavior to evaluate | Required evidence / requirement links |
| --- | --- | --- | --- |
| F01 | A dry synthetic path approaches and crosses the warning boundary, then the modeled hazard edge. | A wearable-specific warning is presented within the prespecified timing budget. Record warning and hazard-crossing times separately. | Independent trajectory and event times; R01, R04. |
| F02 | Wrong boundary, omitted nearby water, or a changed shoreline. | Invalid or unsupported coverage is visible. No implied protection beyond the validated geometry. A map error that cannot be detected is an explicit residual risk. | Boundary revision and change assumptions; R01. |
| F03 | Position jumps, body blockage, or uncertainty overlaps the warning region. | Uncertain approach is not silently labeled away. Compare proposed warning/unavailable behavior, including nuisance cost. | Reference trajectory, uncertainty, conditions; R03, R15. |
| F04 | Position reports stop while the last fix was inland. | Stale information becomes unavailable under the reviewed age rule; do not keep a fresh-looking position. | Acquisition/receipt times and unavailable transition; R03, R05. |
| F05 | Warning is created early but queued and presented after hazard crossing. | Count a late warning rather than a successful detection. Distinguish generation from presentation. | Stage times and clock uncertainty; R04, R06. |
| F06 | Phone locked, app suspended, notification permissions disabled, receiver off, or radio disconnected. | Record what can and cannot be noticed. Never assume a disconnected receiver reports its own failure; an independent notification route is an open architecture question. | Receiver-specific delivery/presentation evidence; R05, R06. |
| F07 | An approach warning is active when location or communication fails. | Keep the unresolved warning alongside unavailable status. Acknowledgment cannot clear either. | S05 and event continuity; R05, R07, R10. |
| F08 | Wearable removed, misworn, depleted, or left on an object. | Do not claim that tracking the object proves the child's position. Evaluate whether removal can be detected; unknown removal remains a failure risk. | Attachment/removal review and power record; R05, R13, R15. |
| F09 | Wrong pairing, wrong receiver, or an unaccepted caregiver handoff. | Show identity and designated receiver. Handoff stays pending; prior assignment remains until acceptance, without implying actual human supervision. | Pairing/handoff record; R02, R09. |
| F10 | Two wearables produce events, or one has a fault while the other approaches. | Both remain independently visible. Acknowledging A does not silence B; prioritization must not discard either. | Per-wearable event/acknowledgment records; R02, R07, R08, R12. |
| F11 | Acknowledged event persists, reappears, or repeats near the boundary. | No "all clear" from acknowledgment. Review recurrence and alert repetition without silent permanent muting. | Incident grouping and unresolved status; R07, R10, R12. |
| F12 | Reference device moves or fails; boundary configuration changes during monitoring. | Invalidate dependent estimates/configuration. Do not continue under old geometry or silently erase an incident. | Dependency and revision records; R01, R05, R15. |
| F13 | Caregiver misses, misunderstands, or cannot act on a presented warning. | Count presentation separately from acknowledgment and response. Review wording and escalation, without assuming availability of another adult. | Dry role-play observations only if separately approved; R06, R11. |
| F14 | Power loss, restart, or recovery while an incident is unresolved. | Restart unavailable; re-establish prerequisites and preserve incident history. No automatic claim of safe conditions. | Restart/recovery sequence; R05, R10, R15. |
| F15 | Duplicate, reordered, delayed, or replayed messages; clock mismatch. | Do not present stale events as fresh positions. Preserve event identity and record uncertainty in timing. | Message identity/order and clock analysis; R03, R10. |
| F16 | Many harmless movements trigger warnings. | Measure false warnings and understandability alongside misses. Do not "fix" nuisance alarms by concealing coverage loss. | False alerts per observation time, scenarios, and tuning record; R11, R12. |
| F17 | Unauthorized pairing or unnecessary sharing of location history. | Reject unauthorized access in the eventual design; research records contain synthetic identities and minimum information. | Data-flow/threat review; R14. |

## Blank observation record

No rows have been executed. Use one record per scenario instance in future authorized work. Requirement R16 applies to every record: preserve assumptions, revisions, failures, and unresolved limitations rather than recording only successful cases.

| Field | Value to record |
| --- | --- |
| Scenario and revision | F-ID, requirement IDs, protocol revision |
| Inputs | Synthetic trajectory, boundary revision, injected fault, wearable/receiver labels |
| Ground truth | Approach onset, warning-boundary crossing, hazard-edge crossing if any; independently determined |
| Alert stages | Created, transmitted, received, presented, acknowledged; unavailable stages explicitly marked |
| Response | Observed response in a separately approved dry role-play, or "not measured" |
| Timing quality | Clock source/alignment and uncertainty; no false precision |
| Result | Expected behavior, observed behavior, missed/late/false warning, fault visibility, unresolved issue |
| Review | Reviewer role, evidence location, decision and rationale; no participant identity in the repository |

## Interpretation rules

An approach event with no usable warning is a miss. A warning presented after the required deadline is late even if the detector fired earlier. A fault indication is not counted as a successful approach warning. Unavailable time and excluded conditions remain in reporting, rather than disappearing from the denominator. The exact event and deadline definitions must be frozen before performance evaluation.

Report counts and denominators before percentages. Separate detection, delivery, comprehension, and response; none alone demonstrates lives saved. Zero misses in a small demonstration is not a reliable upper bound on failure probability. An unresolved privacy, identity, warning-suppression, or false-reassurance issue blocks progression until reviewed. See the [evaluation plan](child-warning-evaluation-plan.md) for stage gates and open numerical criteria.
