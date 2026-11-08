# Child left in a hot car: detection and emergency alerts

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Dog hot-car case](dog-hot-car-use-case.md) · [Highest-priority child water case](child-water-proximity-use-case.md)

Research brief, version 0.1 — source review November 8, 2026. No device, heat-exposure study, emergency-service integration, or protective performance has been demonstrated. Child water-approach warning remains the project's highest priority.

## Intended outcome

A child wears a device that recognizes possible unattended presence in a vehicle and dangerous heating, warns responsible adults, and alerts emergency services through a supported response path. The aim is to help someone reach the child before serious harm. Preserve automatic emergency escalation as an ambition, rather than reducing the idea to a phone reminder.

This would be a backup aid, never permission to leave a child in a vehicle. NHTSA advises never leaving a child unattended in a vehicle for any length of time; shade and partially open windows do not make that safe. Its guidance says to act immediately and call 911 when a child is seen alone in a locked car. A real emergency must not wait for an experimental device. [NHTSA heatstroke prevention](https://www.nhtsa.gov/campaign/heatstroke)

## Separate the detection problems

The following are proposed engineering questions, not established capabilities:

| Question | Candidate evidence | Important limitation |
| --- | --- | --- |
| Is the child present, with the device actually worn? | Wear/contact indication; independent vehicle occupancy sensing | A vest left on a seat can look present; a child without it can be invisible to the system. |
| Is this a vehicle context? | Paired vehicle signal, trip/door state, environmental observations | Being near a car or losing a radio connection does not establish being inside it. |
| Could the child be unattended? | Caregiver separation and explicit supervision handoff, considered with vehicle state | A phone left in the vehicle does not prove an adult is present. Proximity alone does not establish supervision. |
| Is heat risk increasing? | Local environmental temperature and trend, sensor quality, potentially a separate cabin reference | Garment, skin, cabin, and core temperatures are different measurements. No diagnosis or safe-temperature inference is established. |
| Can someone intervene? | Alert delivery, responsible recipient, current location, supported escalation route | A sent message does not establish rescue or even receipt. |

Compare wearable-only, vehicle-only, and combined approaches before choosing a vest. The first concern should be possible unattended occupancy; do not design a system that waits for signs of heatstroke. Children entering a parked vehicle without the wearable remain an explicit coverage gap. No safe unattended duration or alert threshold is selected here.

## Proposed response chain

1. Establish device/vehicle pairing, responsible caregiver, coverage, and readiness before a trip. Make unavailable protection conspicuous; a successful check is not a safety guarantee.
2. Recognize possible unattended occupancy or concerning environmental conditions. Preserve separate indications for uncertainty, faults, and possible danger.
3. Attempt local and caregiver alerts, with an agreed backup recipient and escalation policy. Neither caregiver acknowledgment nor a lost connection should silently clear an unresolved event.
4. Escalate through a jurisdiction-supported emergency or monitored-response integration. Define when escalation occurs, who receives it, and how failures are exposed. Do not require an unreachable caregiver's permission or invent a countdown in this brief.
5. Track message submission, recipient acceptance, any confirmed dispatch, and physical resolution as distinct states. Cancellation and resolution need reviewed criteria; pressing “seen” is not evidence that the child is out of danger.

The National 911 Program identifies location, callback number, and the nature of the emergency as information a call-taker may need. That supports including current location and its uncertainty, vehicle identification, observation age, and a reachable contact in a proposed incident packet. It does **not** establish that an automated wearable message is accepted by a local emergency center. [Calling 911](https://www.911.gov/calling-911/)

No emergency integration has been arranged. Regional coverage, responder acceptance, monitoring responsibilities, escalation timing, false-alert handling, and communications outages must be resolved before claiming automatic emergency notification. Test endpoints must be simulated; no unarranged calls to emergency services are part of this work.

## Requirements and failure scenarios to review

| Proposed requirement | Failure to exercise with simulated data or inert surrogates |
| --- | --- |
| Report missing, unworn, disconnected, and depleted devices distinctly. | Device removed; battery fails; child is present without a tag. |
| Do not equate a nearby phone or acknowledged alert with supervision. | Caregiver phone remains in car; wrong adult accepts; handoff is incomplete. |
| Preserve unresolved events during faults. | Radio, cellular service, application, or backend fails during an alert. |
| Show evidence age and location uncertainty. | Underground parking, old coordinates, wrong vehicle, or a moving vehicle. |
| Evaluate temperature sampling at the intended placement. | Sunlight on sensor, body warming, shade, calibration drift, or thermal lag. |
| Keep simultaneous children and recipients distinguishable. | Two wearables are swapped or one child's event hides another. |
| Review pediatric wearability and restraint compatibility before hardware selection. | Garment bulk, harness interference, overheating, snagging, or accessible parts. |
| Minimize location and child data. | Unnecessary trip history, unauthorized pairing, or disclosure through alerts. |

No inflatable mechanism is proposed for this case. Do not modify child restraints or assume the adult vest concept is appropriate for a car seat. A qualified child passenger safety and pediatric review must establish any permissible garment and sensor arrangement.

## First safe research steps

Review existing occupant-detection and reminder approaches alongside this proposal. With appropriate specialists, define the intended ages, vehicle environments, supported emergency workflow, and measurable acceptance criteria: missed occupancy/events, false alerts, detection and delivery delay, information freshness, energy reserve, and unresolved escalation failures. Numerical limits remain open.

Start with paper incident scenarios and synthetic event sequences. A separately reviewed bench plan could use inert mannequins and instrumented fixtures to evaluate sensing and communications, including temperature conditions without occupants. No child, animal, or volunteer is to be left in a vehicle or exposed to heat for testing. Later human-factors or pediatric work would require its own authorization and review.

Proceed only if the evidence supports both reliable detection and a usable response path. Neither part alone demonstrates prevention of injury or death.
