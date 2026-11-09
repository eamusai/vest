# Decisions and roadmap

[Home](../README.md) · [Evidence](evidence.md) · [Next steps](next-steps.md)

Decision record — November 8, 2026. These choices come from the project conversation; they are proposals for research, not results. The later child-protection priority supersedes the earlier adult-first ordering.

| Decision | Reason | Revisit when |
| --- | --- | --- |
| **Prioritize child water safety before and after entry; start with approach-warning research.** | The user made helping save a young child's life the central aim and clarified that intended protection also includes flotation and urgent alerts after entry. | Evidence or an explicit priority change warrants a different next step. |
| Start the child track with requirements, failure scenarios, and a paper caregiver-alert concept. | No warning system or demonstrated benefit exists; location, boundary, delivery, and response must all be evaluated. | Reviewed requirements support separately authorized dry feasibility work. |
| Keep the adult comfort, fit, readiness, and hands-free-alerting work as a secondary track. | Existing research and the paper companion remain useful without transferring adult assumptions to children. | A specific adult problem warrants further work alongside the priority track. |
| Retain inflatable concepts for adult research without prescribing them for children. | The original preference concerned adult comfort; pediatric eligibility and design require separate evidence. | Activity, fit, or equipment requirements favor another design. |
| In the adult companion, separate initial installation/service from before-outing checks. | Repeated installation is not automatically a required pre-use action. | Exact manuals prescribe a different schedule. |
| Explore open sharing rather than patents. | Aim to hand reproducible, tested work to capable manufacturers/researchers. | Original documents now use CC BY 4.0; future software/hardware licensing needs explicit scope. |

## Priority progression: child water-approach warning

1. **Now:** review the draft young-child and caregiver requirements, fictional fixed-shoreline model, candidate approaches, and unresolved parameters with relevant specialists.
2. **First deliverable drafted:** [16 proposed requirements](child-warning-requirements.md), [17 failure scenarios](child-warning-failure-scenarios.md), [seven paper screens](child-caregiver-alert-mockup.md), and an [evaluation plan](child-warning-evaluation-plan.md). Define numerical acceptance criteria before performance work; no distance or response-time guarantee is assumed.
3. **If justified:** separately plan synthetic-path and dry surrogate evaluation away from water, using inert tags or adults rather than children. Evaluate missed/late alerts, nuisance alerts, communication failures, and caregiver understanding.
4. **Before pediatric or field work:** obtain specialist review of fit, wearability, foreseeable misuse, privacy, supervision effects, and the proposed study. The current brief authorizes no recruitment or child exposure.
5. **Eventual handoff:** reproducible work with bounded evidence, failure modes, and limitations. Saving a child's life remains the aim, not a demonstrated outcome.

The [child-warning brief](child-water-proximity-use-case.md) is the source of the current priority requirements. No alarm replaces supervision or barriers.

## Earlier adult roadmap — retained as secondary

1. **Next within the adult track:** resolve manual verification gaps in the documented comparator and mock-up.
2. **Before recruiting:** map each scored task and companion item to official instructions, review task safety and consent, and prepare inert fault examples.
3. **Formative dry pilot:** compare manufacturer instructions alone with those instructions plus the companion; revise or discard confusing features. Observe comfort with unmodified equipment.
4. **Only if warranted:** investigate specific physical changes for observed needs with qualified collaborators. Do not assume approval remains valid after modification.
5. **Later controlled work:** rescue-mannequin comparisons could examine normal/partial/failed inflation, body posture, antenna clearance, simulated local messages, and spray false triggers. Requires a separate reviewed protocol and authorized radio testing. None has been executed.
6. **Eventual handoff:** reproducible design files, bounded test evidence, limitations, maintenance information, and selected licensing. Publication remains a separate decision.

## Deferred ideas

The original concept combined comfortable uninflated wear, automatic inflation, temperature sensing/heating, distress signaling, and eventually propulsion toward safety for an incapacitated wearer. Heating, propulsion, and new backup buoyancy are outside the first prototype.

One candidate would infer failed or partial inflation using pressure, temperature, and actual chamber expansion, then deploy independent backup buoyancy. Preserve it as an unvalidated research idea: novelty, sensing reliability, safety, and benefit are unknown. Prior-art discussion found related alerts, heating, distributed sensors, antenna selection, and self-checks; no complete patent landscape or freedom-to-operate analysis was performed.

The original adult scenario does not cover children, whitewater, every activity, or every body type. The new child-warning priority has its own requirements and evidence; it is not an extension of adult equipment approval or the adult pilot.

## Added use case: avalanche burial

On November 8, 2026, the user requested a skiing/snowboarding avalanche scenario and proposed inflation to create breathing space, subsequent deflation, automatic avalanche detection, and using chamber air for breathing. The [avalanche brief](avalanche-use-case.md) preserves these as separate, unvalidated research questions and compares them with existing equipment and studies. This remains a separate track without selecting a universal vest, breathing apparatus, or automatic trigger. No additional hardware work or human experiments have been conducted.

## Added use cases: falls and horse-to-vest warning

The user requested automatic impact cushioning for horse riding, motorcycle falls, altitude falls, and potentially other rapid falls. They explicitly asked to retain altitude falls as a long-term reach rather than remove the idea because it is difficult. The [fall-impact brief](fall-impact-use-case.md) keeps that ambition while separating deceleration, impact cushioning, and activity-specific evidence.

The user also described a monitor worn by the horse, connected to the rider's vest, intended to predict a spook and warn the rider, with inflation potentially assisting an emergency dismount. The [horse-warning brief](horse-warning-use-case.md) records the full intended flow. Advance prediction, the benefit of a warning, and safe dismount cushioning are unvalidated; the concept is not an instruction to jump or automatically dismount. The [catalog](use-cases.md) preserves all of these cases. No hardware or live intervention has been added.

## Sharing decision and diagrams

On November 8, 2026, the user accepted the recommendation to license the original documents and conceptual diagrams under [CC BY 4.0](../LICENSING.md), allowing commercial reuse with attribution. The [visual overview](overview.md) adds a use-case map and a proposed research progression. Public release is intended as early research seeking review, not a validated design release. The repository owner will make the final visibility change; this documentation update does not do so. Third-party sources are excluded from the license grant, and future software/hardware licensing remains a separate scope decision.

## Child priority and appearance illustration

Later on November 8, 2026, the user made warning a caregiver before a young child approaches water the highest priority over all other use cases. The README, catalog, visual overview, and next steps now reflect that ordering. This records the motivation without adding family details or child data to the repository.

The user also approved an initial [adult appearance illustration](appearance-concept.md). It is retained as a labeled exterior concept from the earlier adult track, with generation provenance. No CAD, child fit, internal architecture, or tested garment is implied.

## Added use case: harmful-water alerts

The user requested sensors on the vest to recognize harmful bacteria or other water hazards and promptly warn the wearer to leave the water. The [water-quality brief](water-quality-use-case.md) preserves direct sensing as a research ambition while separating target-specific detection, indirect measurements, and advisory information. No instant broad-spectrum detector is established. Child water-approach warning remains the highest priority, and no proposed system currently establishes that a lake visit is safe.

## Child research specification

The user asked to proceed with next steps and fully develop the child case. The review package now traces proposed requirements to failure scenarios, distinguishes warning delivery from caregiver response, preserves unresolved warnings through acknowledgment and lost updates, and identifies open performance parameters. A static paper interface and a simulated conversation preview support wording review only. No detector, trajectory simulator, monitoring service, hardware, or human study has been implemented or conducted. Specialist review is the next evidence gate.

## Added use cases: child and dog hot-car alerts; horse calming

On November 8, 2026, the user requested three further scenarios: detecting a child left in a hot car and alerting emergency services; doing the same for a dog; and a horse-worn vest connected to monitoring that detects stress and uses suitable modalities to calm the horse, aiming to prevent spooking or bucking off the rider.

The [child hot-car brief](child-hot-car-use-case.md) and [dog hot-car brief](dog-hot-car-use-case.md) preserve emergency escalation as an intended outcome while separating occupancy, supervision uncertainty, heat sensing, communications, responder acceptance, and physical resolution. They require separate pediatric and veterinary evidence; neither selects thresholds or claims an operating emergency integration. Initial research uses paper scenarios and inert surrogates, never unattended children or animals in vehicles.

The [horse calming brief](horse-calming-use-case.md) distinguishes intervention on the horse from the existing rider-warning case. Acoustic, tactile, and handler-mediated options remain hypotheses. Passive observation precedes any separately reviewed intervention; neither sensor changes nor apparent quietness alone establish welfare benefit. No mounted intervention, induced spook, automatic airbag trigger, or claim of preventing bucking is approved.

Child water-approach warning remains the highest priority. These additions expand the catalog without selecting a universal garment or authorizing purchases, expert outreach, recruitment, experiments, or emergency calls. Repository visibility was checked and is now public; this update changes documentation, not access settings.

## Clarification: protection after a child enters the water

On November 8, 2026, the user reported reader confusion about whether the intended vest would help after a child enters the water. They approved explicitly stating both parts of the child-safety goal: advance caregiver warning and child-appropriate flotation with urgent caregiver alerts after accidental entry. Earlier wording described the first warning-research phase too narrowly to make the full intended benefit clear.

The README, child brief, catalog, overview, and next steps now distinguish the full goal from the initial review package. Excluding automatic inflation from that package does not remove after-entry protection from the research ambition. The existing 16 requirements, 17 scenarios, and seven paper screens still address before-entry warnings only. Child flotation and after-entry alerting require separate requirements, pediatric suitability review, and validation. No design, automatic trigger, field trial, demonstrated lifesaving result, or guarantee of rescue is established by this wording change.

## Added application: obstacle navigation

On November 9, 2026, the user requested a vest that senses surrounding obstacles and conveys that information to a blind or low-vision wearer. The [navigation concept](obstacle-navigation-use-case.md) preserves nighttime forest running as a long-term ambition. At the user's request, hummingbird investigation stopped; hummingbirds remain inspiration with the sensing mechanism unresolved. The concept is recorded without selecting hardware or claiming collision-free navigation. Child water safety remains the highest priority.
