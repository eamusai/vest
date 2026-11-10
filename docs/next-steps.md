# Open questions and next steps

[Home](../README.md) · [Evidence](evidence.md) · [Roadmap](decisions.md)

Updated November 9, 2026. None of the proposed study work has been executed.

## Highest priority: child water safety before and after entry

The [child water-safety brief](child-water-proximity-use-case.md) takes precedence over the other tracks. The aim is to help save a young child's life through caregiver warnings before water entry and child-appropriate flotation with urgent alerts after entry. Approach warnings remain the first research phase. Its draft [requirements specification](child-warning-requirements.md), [failure register](child-warning-failure-scenarios.md), [paper alert mock-up](child-caregiver-alert-mockup.md), and [evaluation plan](child-warning-evaluation-plan.md) do not specify or validate after-entry protection. They are review materials, not deployable safety hardware.

1. Review the fictional fixed-shoreline starting model and the 16 proposed requirements. Resolve the intended child age/size range, coverage assumptions, receiver responsibility, and approach-event definition. Preserve broader water environments as open scope rather than assuming universal detection.
2. Extend the scoped comparison of access, immersion, geographic-boundary, and local-ranging approaches. Obtain pediatric water-safety, positioning, and human-factors review; none has happened yet. Use the evaluation plan's questions without treating this as authorization to contact people.
3. Resolve the open numerical limits and architecture questions: position/boundary uncertainty, information age, warning time, detection rates, power, and how an unreachable receiver's failure can be noticed. Choose no warning distance or performance guarantee without evidence.
4. Freeze acceptance criteria and a separately reviewed synthetic/dry evaluation plan. The 17 scenarios are proposed, not executed; no child recruitment or water exposure is included.
5. Review the seven paper screens for false reassurance, acknowledgment confusion, and handoff misunderstanding. Establish child-appropriate wearability and privacy requirements before selecting hardware or creating child CAD.

For the after-entry goal, separately define pediatric flotation, fit/retention, body orientation and airway-support goals, entry detection, urgent alert delivery, and failure behavior with relevant specialists. Review any proposed automatic inflation independently of the adult equipment. Develop a reviewed bench/mannequin evaluation proposal before considering further work; no child water-entry trial or protective claim is authorized by this clarification.

## Adult track: before testing

1. Finish reviewing the Elite owner manual, PLB3 manual, fitting guide diagrams, and applicable equipment labels. Confirm revisions, market, eligibility, and compatibility; resolve conflicts with manufacturers. Record exact page/section references for each companion item and scored task.
2. Determine which requirements apply to installation, service, and each outing. Replace broad research prompts with a reviewed, traceable sequence before any operational use. Keep the current draft visibly incomplete until then.
3. Review the follow-up sources in the evidence ledger, including the inaccessible USCG alert and CDC erratum. Keep incident examples separate from prevalence estimates.
4. Have a qualified boating-safety/human-factors reviewer examine the companion and protocol. Expert interviews may improve the next revision; they are not prerequisites to these initial drafts.
5. Specify recruitment, consent, privacy, equipment suitability, facilitator preparation, and the inert fault-example answer key. Obtain equipment only after that plan is agreed. No purchase or recruitment has occurred.

## Questions the adult pilot can help answer

- Which required information is hardest to find or understand?
- Does separating installation from outing preparation reduce omissions or create new confusion?
- Do people understand “Checked” as a user report rather than a device diagnosis?
- Which movements create pressure or restriction, and does ordinary prescribed adjustment resolve it?
- Are errors tied to the paper design, instruction complexity, unfamiliarity, or equipment fit?

## Questions the adult pilot cannot answer

Will a system inflate, keep an incapacitated person's airway clear, transmit successfully in a particular posture, or bring rescuers in time? Does it reduce deaths? Are new heating, propulsion, or backup-buoyancy designs safe or novel? These require different evidence and separately designed studies.

It also cannot validate child water-approach detection, pediatric garment suitability, or the effectiveness of caregiver alerts. The [adult appearance concept](appearance-concept.md) adds no engineering evidence; any later CAD needs defined requirements and specialist review.

## Avalanche research track

Read the [avalanche use case](avalanche-use-case.md) for the added skiing/snowboarding scenario. First compare existing deflating airbags and breathing-support systems with the proposed automatic activation and chamber-air ideas. Resolve exact manual/compatibility gaps and identify a specific unmet need before selecting equipment. A separate dry usability protocol and specialist mannequin/bench plan would be required; the water pilot does not validate snow-burial performance.

## Impact and horse-warning research tracks

Use the [catalog](use-cases.md) to retain the broader set of ideas. Compare existing rider airbags separately for [motorcycle and equestrian impacts](fall-impact-use-case.md). Keep altitude falls as a long-term feasibility question for aerospace and biomechanics specialists; do not infer protection from ordinary vest inflation.

For the [horse-to-vest warning](horse-warning-use-case.md), first establish whether a signal reliably precedes a spook with usable lead time. Begin with literature, expert review, and an observational-study proposal. Study alert interpretation away from horses before considering live warnings. Any emergency dismount concept needs separate evidence that the response helps; no deliberate jumps, induced spooks, or human impact trials are proposed.

## Child and dog hot-car research tracks

Develop the [child](child-hot-car-use-case.md) and [dog](dog-hot-car-use-case.md) cases separately. Compare wearable, vehicle occupancy, and combined approaches; address missing wearables and phones left in the car. Begin with possible unattended occupancy rather than waiting for heat illness. Pediatric and canine fit, measurements, and operating criteria need their own specialist review.

For each case, define a supported local emergency-response arrangement, including responsibility, location uncertainty, escalation, cancellation, and communication failure. A sent alert or caregiver acknowledgment is not confirmed dispatch or physical rescue. No emergency integration exists, no contacts have been made, and no live emergency calls are proposed. First use paper scenarios, simulated recipients, and a separately reviewed inert-fixture bench plan; never leave a child or animal in a vehicle or expose them to heat for testing. These tracks do not displace child water-approach warning.

## Horse stress and calming research track

Use the [horse calming brief](horse-calming-use-case.md) to distinguish stress estimation, spook prediction, intervention effects, and rider protection. Review full methods behind the preliminary music and touch findings with equine veterinary and behavior expertise. Compare candidate cues with appropriate controls; do not assume human touch or resting stable results transfer to an actuator during riding.

Prepare a passive observational proposal and bench-test output limits, independent stop controls, lost links, wrong pairing, and actuator-induced sensing artifacts on inert fixtures. Only separately authorized, welfare-reviewed work could consider a familiar handler-controlled cue in comfortable, unmounted conditions. No automatic calming, deliberate fright, induced bucking, or mounted intervention trial is ready to implement.

## Harmful-water sensing track

Use the [water-quality brief](water-quality-use-case.md) to select one initial hazard and setting with relevant specialists. Compare direct sensing, proxy measurements, and official advisories without treating them as equivalent. Establish detection delay, validity, reference methods, and false-negative risks before hardware selection. Begin with published data and paper alerts; no contaminated-water exposure or swimming trial is proposed. This track does not displace the child-approach priority.

## Vehicle tactile awareness research

Use the [vehicle-integrated tactile awareness brief](vehicle-tactile-awareness-use-case.md) to separate automotive and aviation scenarios. Compare selective seat warnings with richer surrounding-traffic cues, defining their meaning before choosing sensors or actuators. Begin with synthetic or recorded scenarios and an inert seat demonstration; separately reviewed simulator studies could examine interpretation, workload, multiple hazards, sensing failures, and conflict with existing alerts. The hummingbird work provides inspiration, not evidence of vehicle traffic detection. Automatic vehicle control is outside this application, and child water safety retains priority.

## Public sharing and manufacturer handoff

The original documentation and diagrams use [CC BY 4.0](../LICENSING.md). See the [visual overview](overview.md) and [release review](release-review.md) for public-facing material and remaining limitations. The repository is now public; publication does not validate the concepts. Preserve manufacturer links rather than copying manuals or drawings. Later manufacturer handoff needs documented tests, failures, uncertainties, revision history, and reproducibility requirements. The owner controls repository visibility.
