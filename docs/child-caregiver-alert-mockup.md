# Caregiver alert: paper mock-up

[Use case](child-water-proximity-use-case.md) · [Requirements](child-warning-requirements.md) · [Failure scenarios](child-warning-failure-scenarios.md)

Version 0.1 — November 8, 2026. Simulated interface copy for review. No location, wearable, radio, alert notification, or monitoring service is connected. All labels refer to fictional Wearable A and fictional Lake boundary A.

[Open the print-ready paper screens](assets/child-alert-paper-v1.html). Download/open that file in a browser to print one scenario per page. The file is static HTML/CSS with no scripts, data collection, or operational controls. The screen copy below is also available directly in GitHub.

## Draft screens

Every screen carries **"RESEARCH MOCK-UP · NO LIVE MONITORING"** and **"Keep close supervision. No alert does not mean safe."** A phone-like layout explores a caregiver receiver; it does not select a phone architecture.

| Screen | Main message and supporting copy | Action or state |
| --- | --- | --- |
| S00 — Not configured | **Warnings unavailable.** Boundary and receiver setup are incomplete. Do not rely on this concept for monitoring. | No acknowledgment action. |
| S01 — Receiving updates | **Receiving updates.** No approach alert in this simulated scenario. This does not establish the child's safety. | Wearable A; Lake boundary A; Receiver A. No green safe state or invented distance. |
| S02 — Possible approach | **Check the child immediately.** Wearable A may be approaching the water boundary. Position is an estimate. | **Acknowledge message**; event remains unresolved. |
| S03 — Message acknowledged | **Check the child immediately.** Message acknowledged. The possible approach remains unresolved. Acknowledgment does not confirm the child's location or safety. | Button changes to **Message acknowledged**; it does not dismiss the warning. |
| S04 — Updates lost | **Check the child. Updates unavailable.** Wearable A's location is not current. Monitoring cannot determine approach. | Acknowledgment records receipt only; unavailable status remains. |
| S05 — Approach plus fault | **Check the child immediately.** Earlier possible approach is unresolved. Location updates are now unavailable. | Acknowledgment leaves both messages visible. This is not replaced by a quieter generic fault screen. |
| S06 — Handoff pending | **Receiver handoff pending.** Receiver B has not accepted. Receiver A remains assigned. Confirm responsibility directly with the other adult. | No completed-transfer indication. A phone assignment does not prove supervision. |

These messages are wording candidates, not validated response instructions. Alerts for multiple wearables would need an additional reviewed layout; the single-wearable screens do not implement F10. The paper handoff screen does not implement pairing or acceptance. No sound, vibration, emergency call, or inflation is triggered by this mock-up.

## State rules for the draft

Start unavailable until required setup is valid. A current update alone does not prove a boundary, pairing, receiver, or child attachment is valid. From any receiving state, a missing prerequisite produces unavailable status. If an approach was unresolved before the failure, keep it visible with the fault. Acknowledgment only changes message-receipt status.

Do not infer resolution because a timer expires, communication resumes, a device restarts, or a caregiver taps the screen. Future incident-resolution and repeat-alert rules must be agreed in the requirements review. All scenarios here are manually selected for review; they are not driven by a detection algorithm.

## Review questions

- What would the caregiver do after each screen, and how quickly do they understand which wearable needs attention?
- Do they distinguish "receiving updates" from "the child is safe"?
- After acknowledging a message, do they still understand that the warning is unresolved?
- Does unavailable status cause a misleading assumption about the child's last position?
- Is an approach still noticeable when a fault appears at the same time?
- Who does the caregiver believe is responsible during an unaccepted handoff?

No caregiver sessions have been conducted. Collecting observations or recruiting participants needs a separate reviewed protocol and consent plan. A simulated interactive preview accompanies the conversation for wording review; it performs no monitoring and is not an operational prototype.

Internal presentation checks on November 8, 2026 covered all seven preview states at desktop and narrow-screen widths, acknowledgment preserving the approach/fault messages, and the static screens fitting their print page boxes. The layouts were visually inspected. These checks do not establish caregiver comprehension, notification delivery, sensing performance, or safety.
