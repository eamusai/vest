# Child water-approach warning: research requirements

[Home](../README.md) · [Use case](child-water-proximity-use-case.md) · [Failure scenarios](child-warning-failure-scenarios.md) · [Caregiver mock-up](child-caregiver-alert-mockup.md) · [Evaluation plan](child-warning-evaluation-plan.md)

Version 0.1 — November 8, 2026. Proposed requirements for specialist review, not a device specification approved for use. No hardware, operational software, field data, or demonstrated protective benefit exists.

## Purpose and first setting

Investigate whether an additional warning can give a supervising caregiver useful notice before a young child who cannot yet swim reaches water. The motivating setting is a family lake visit. The system must not encourage a caregiver to relax supervision or treat an alert as a substitute for restricting access. Saving a child's life is the intended benefit; it is not an established outcome.

For the first desk-based model, use a fictional, fixed shoreline segment and an inland warning boundary. This preserves the lake motivation while making geometry explicit. Later dry work would represent that boundary on land away from water. No actual lake, child, address, or travel history is selected or recorded. Pool access is a useful comparator, not a replacement for the lake use case.

The model assumes a known hazard region, a defined area in which location estimates are meaningful, and at least one designated caregiver receiver. It must represent unknown areas and invalid boundaries explicitly. Changing water levels, docks, multiple water bodies, waves, missing map features, and new locations invalidate any assumption of universal coverage. The boundary must be on the approach side of the hazard; it is not the shoreline itself and it is not a safe-distance recommendation.

Initial scope includes one or more synthetic wearable identities and one or more caregiver receivers. It excludes automatic inflation, propulsion, contaminant clearance, drowning diagnosis, automated emergency-service calls, and advice that a child may enter water. No age, body-size range, garment, phone platform, or radio technology has been selected.

These exclusions define this **first warning-research phase**, not the complete product goal. The [child water-safety brief](child-water-proximity-use-case.md) also records intended child-appropriate flotation and urgent caregiver alerts after accidental entry. Those functions require a separate child-specific requirements and validation effort; the 16 requirements below do not establish in-water protection.

## Functional chain and terms

The proposed chain is **hazard definition → wearable position and uncertainty → approach assessment → receiver presentation → caregiver response**. Each link can fail independently.

- **Hazard region:** the mapped water-side area in a synthetic scenario; not a claim to know every hazard.
- **Warning boundary:** a separately defined inland trigger region. Its distance and shape are unresolved research parameters.
- **Available:** dependencies satisfy specified validity checks. This describes information availability, never child safety.
- **Approach event:** independently defined ground truth in a scenario, including event start and the eventual hazard crossing if any. The detection algorithm does not define its own ground truth.
- **Alert stages:** created, transmitted, received, presented, acknowledged, and physically responded to. These are distinct records.
- **Incident:** a warning event associated with one wearable, boundary revision, and event identity. Acknowledgment changes receipt status, not the underlying event or child's condition.

If a position estimate's uncertainty overlaps the warning region, the system must not silently classify it as away from the hazard. Candidate conservative warning and unavailable behavior need specialist evaluation; neither is currently validated. Distance to the parent and water-contact detection do not substitute for distance to the hazard boundary.

## Proposed requirements and verification

"Shall" below expresses a proposed design obligation. It does not claim implementation or compliance. Scenario IDs refer to the [failure-scenario register](child-warning-failure-scenarios.md).

| ID | Proposed requirement | Review or verification evidence |
| --- | --- | --- |
| R01 | Record the hazard geometry, warning boundary, coverage area, revision, source, and validation status separately. Invalidate unsupported or changed geometry. | Inspect synthetic boundary records; exercise F01, F02, F12. |
| R02 | Pair each wearable with the intended caregiver receiver explicitly; distinguish simultaneous wearables without child names in research records. | Pairing and multi-wearable cases F09, F10. |
| R03 | Include position uncertainty, acquisition time, and data age in approach assessment; reject missing, out-of-order, or stale information as a current location. | F03, F04, F15 with independent event records. |
| R04 | Identify a supported approach promptly under stated conditions; evaluate total warning time rather than only processing time. | F01, F05 and measured stage times in the evaluation plan. All timing limits remain unresolved. |
| R05 | Show missing dependencies explicitly. Battery loss, missing reference devices, lost connections, and possible removal must not look like absence of hazard. Do not claim removal detection unless demonstrated. | F04, F06–F08, F12, F14. |
| R06 | Distinguish message transmission from presentation on the designated receiver. Audit locked-screen, background, permissions, muted audio, and receiver-off behavior. | F05, F06, F13. An unreachable receiver cannot be assumed to display its own failure. |
| R07 | Keep warning status independent of acknowledgment. Acknowledgment must not clear the hazard, restore availability, or act as a global mute. | F07, F10, F11; mock-up S02, S03, S05. |
| R08 | Maintain each wearable's unresolved warnings and faults independently; a new event for another wearable must not be hidden by the current screen. | F10; evaluate simultaneous presentation and escalation. |
| R09 | Make caregiver handoff explicit and accepted by the receiving adult. Keep the previous designated receiver until acceptance; if continuity is lost, show unavailable rather than inventing supervision. | F09; mock-up S06. This records receiver responsibility, not proof of human supervision. |
| R10 | Preserve an unresolved approach when a fault occurs. Recovery must not silently erase the incident; boundary, identity, fresh data, and communication validity must be re-established. | F07, F11, F14, F15; mock-up S05. |
| R11 | State that no alert is not proof of safety. Use readable text and more than color alone. Avoid reassuring maps, green readiness scores, or unvalidated exact distances. | S00–S06 review and caregiver comprehension questions. |
| R12 | Define alert repetition, prioritization, and nuisance management without a hidden permanent mute. Evaluate distraction and alarm fatigue. | F10, F11, F16. No sound pattern or escalation interval is selected. |
| R13 | Establish child-specific fit, attachment, removal, skin contact, snagging, small-part, battery, and compatibility requirements before hardware selection. | Pediatric wearability review; F08. Adult vest art supplies no such evidence. |
| R14 | Use explicit authorized pairing, minimum data, bounded retention, and controlled access. Do not expose child locations or identities publicly. | Threat and data-flow review; F17. Synthetic records only in this phase. |
| R15 | Evaluate environmental and maintenance limits, including body obstruction, clothing, moisture, handling, reference displacement, and power depletion. | F03, F08, F12, F14 with separately reviewed methods. No operating limits are claimed yet. |
| R16 | Keep records of assumptions, failures, limitations, and revisions. Make no field-readiness claim until the relevant validation is completed. | All scenarios, evidence ledger, and stage decisions. |

## Quantities that must be decided before performance testing

These are **open parameters**, not hidden default settings. Document their rationale, owner role, evidence, and review date before freezing a protocol.

| Open parameter | Why it matters | Evidence and review needed |
| --- | --- | --- |
| Intended age/size range and wearable form | Determines pediatric suitability and foreseeable removal or misuse. | Pediatric water-safety and human-factors input; later qualified fit work. |
| Coverage geometry and boundary validity rules | An accurate position relative to the wrong shore is still wrong. | Site/mapping model, positioning review, and change-detection assumptions. |
| Position/map error limits and confidence meaning | A mean error does not bound rare large errors. | Independent ground truth across conditions; define uncertainty calibration and tail errors. |
| Maximum information age and fault-detection time | A recent-looking stale fix can hide movement. | End-to-end timing and outage analysis, including clock faults. |
| Warning lead-time budget | Must include sensing, transport, presentation, recognition, and response. | Explicit approach scenarios and human-factors review; no assumed universal child speed or reaction time. |
| Acceptable missed/late-event rate and statistical evidence | A few successful demonstrations do not bound rare failures. | Risk analysis, prespecified analysis, confidence intervals, and sample-size justification. |
| Acceptable nuisance alerts per observation time | Frequent alerts may be ignored; reducing them may increase misses. | Measure both tradeoffs and caregiver interpretation. |
| Power reserve, operating conditions, and maintenance interval | Determines availability and foreseeable failure. | Hardware-specific testing after selection; none selected now. |
| Escalation, repeated alerts, recovery, and retention periods | Affects noticeability, distraction, incident continuity, and privacy. | Tabletop review and later separately approved evaluation. |

The review package can be checked for internal consistency now. It cannot pass an operational performance gate while these parameters remain unresolved.

## Candidate approaches and evidence boundaries

| Approach | Established behavior or source | Implication for this project |
| --- | --- | --- |
| Door/gate access warning | [CPSC Pool Safely](https://www.poolsafely.gov/parents/safety-tips/) describes barriers and door alarms as layers around pools. | Detects use of a particular access route; an open lake has no equivalent single gate. No child position is inferred from a door opening. |
| Water-contact or pool-disturbance alarm | A [CPSC study from 2000](https://www.cpsc.gov/Newsroom/News-Releases/2000/CPSC-Releases-Study-on-Pool-Alarm-Reliability) distinguished wristband contact alarms from surface/subsurface disturbance alarms. | Useful historical trigger categories, not a current product ranking. Their after-contact trigger does not meet the desired before-approach outcome. |
| Consumer geographic boundary alert | The [Garmin Bounce 2 manual](https://www8.garmin.com/manuals/webhelp/GUID-ED045F09-4EC3-41F5-AAAC-42B3A3836894/EN-US/GUID-A5E5ADD2-FA29-4EBF-A3E2-D885F4C11C65.html) describes entry/exit notifications for configured boundaries. | Demonstrates a boundary-notification pattern, not precise lake-edge detection, pediatric suitability, or a response-time guarantee. No purchase is recommended. |
| GPS position plus a mapped boundary | [GPS.gov](https://www.gps.gov/gps-accuracy) describes device and environmental accuracy limits. | Retain for comparison; ordinary GPS performance does not establish a reliable close-edge warning. |
| Local ranging plus reference geometry | [Android UWB documentation](https://developer.android.com/develop/connectivity/uwb) describes device ranging and platform constraints. | Candidate for a known bounded setting; requires infrastructure, verified geometry, real-world error analysis, and a viable receiver architecture. It does not directly detect water. |

The first three sources were opened for this package on November 8, 2026; GPS/UWB sources were reviewed in the use-case brief on the same date. This is a scoped comparison, not a complete market or patent survey. No architecture is selected. A phone receiver and a dedicated local receiver remain alternatives: phone convenience must be weighed against background/notification constraints; a separate receiver adds its own power, pairing, carrying, and failure burdens.
