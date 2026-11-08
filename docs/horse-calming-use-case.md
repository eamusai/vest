# Horse-worn stress monitoring and calming research

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Horse-to-rider warning](horse-warning-use-case.md) · [Rider impact protection](fall-impact-use-case.md)

Research brief, version 0.1 — source review November 8, 2026. No monitoring model, calming device, animal intervention, or rider trial has been developed or conducted. Child water-approach warning remains the highest priority.

## The user's intended system

The **horse** wears a vest connected to a monitoring device. The proposed system detects signs of rising stress and applies suitable calming modalities, aiming to reduce the chance of spooking or bucking and thereby help protect the rider. Automatic sensing and intervention are retained as the long-term ambition.

This is separate from the existing horse-to-rider warning case: an alert tells a person something; a calming intervention changes what the horse experiences. Detecting stress, predicting a spook, calming the horse, and preventing rider injury each need separate evidence. A lower heart rate or lack of visible movement alone does not demonstrate a beneficial emotional state or improved safety.

## What preliminary evidence supports

| Primary research | Finding relevant to exploration | Limit on transfer to this concept |
| --- | --- | --- |
| [Music and geriatric horses](https://pubmed.ncbi.nlm.nih.gov/31203990/) | A study of 20 older warmblood horses reported temporary changes in resting heart-rate and variability measures consistent with relaxation during a repeated music intervention. | Stable-based findings in older horses do not validate an immediate wearable cue, detection-triggered playback, or prevention of spooking or bucking. |
| [Wither scratching and neck patting, 2016](https://researchoutput.csu.edu.au/en/publications/physiological-and-behavioral-responses-of-horses-to-wither-scratc/) | In 18 horses following a short ridden obstacle course, wither scratching was associated with more relaxed-type behavior than the comparison treatments. | Human touch in that setting does not establish that an actuator, vibration, or pressure garment will have the same effect or prevent a fall. |

These are abstract-level findings from a preliminary scan, not a completed evidence review. Full methods, effect sizes, study limitations, and reproducibility need review before selecting a modality. The [existing warning brief](horse-warning-use-case.md) separately records arousal and startle research; none establishes reliable advance warning for every horse or setting.

## Candidate modalities, with no selected treatment

| Research option | Question to resolve before live use |
| --- | --- |
| A familiar acoustic cue, familiar voice, or music | Does this individual horse tolerate it, and does it help in the relevant context without startling the horse or distracting the rider? |
| A familiar tactile cue or carefully evaluated tactile actuator | Can a device reproduce a useful cue without pressure, irritation, interference with tack, or a novel sensation that increases stress? Human-touch evidence is not actuator evidence. |
| A handler-facing prompt to pause and assess the stressor | Is changing the activity or environment more appropriate than applying stimulation? Can the handler respond without distraction or an unsafe maneuver? |

These are hypotheses, not recommended operating modes. No sound level, vibration pattern, pressure, location, or exposure duration is specified. Initial scope excludes drugs, aversive stimulation, restrictive compression, and automatic rider-airbag activation. A device must not mask signs of pain, illness, poor tack fit, or an unsuitable situation so that riding continues.

## Proposed sensing and control sequence

1. **Observe first.** Investigate candidate physiology and motion alongside independently assessed behavior and context. Distinguish exertion, excitement, discomfort, environmental heat, and sensor artifacts from the intended stress construct. Record uncertainty rather than assigning a definitive emotion from one sensor.
2. **Establish individual fit and baseline.** Review the horse-worn garment for pressure, rubbing, heat retention, snagging, movement restriction, and tack interference. No universal fit or shared rider-vest design is assumed.
3. **Keep the first research mode passive.** Observe without delivering cues, riding advice, or inflation commands. Any study needs its own approved plan; this brief does not authorize collecting animal data.
4. **If justified, study one handler-controlled cue.** After veterinary/behavioral review and familiarization, compare a specified cue against an appropriate control in comfortable, unmounted conditions. A qualified handler must be able to stop it immediately.
5. **Consider automation only after evidence.** Automatic delivery would need validated eligibility, timing, output limits, fault handling, and demonstrated benefit beyond a competent handler's usual management. Preventing spooks, bucking, or injuries would remain additional claims requiring appropriate evidence.

No horse stress estimate should command a rider to jump or automatically inflate the rider's vest. The existing warning, dismount, and impact concepts retain their own safety questions.

## Failure modes and welfare requirements

| Failure or uncertainty | Proposed requirement |
| --- | --- |
| Normal exercise or pain classified as fear | Evaluate context and behavior; surface uncertainty; allow assessment of the underlying cause. |
| Sudden spook without measurable warning | Preserve missed-event analysis; never imply no alert means a predictable or safe horse. |
| Sound or touch increases arousal | Predefine welfare stop rules and immediate output cessation; do not automatically intensify the cue. |
| Actuator movement contaminates the sensor | Test this feedback path independently; prevent repeated self-triggered stimulation. |
| Lost link, stale data, depleted battery, or software restart | Default the intervention output to off, expose the fault, and preserve an event log for review. |
| Incorrect horse pairing or wrong baseline | Verify identity and configuration; do not carry learned settings across horses without evidence. |
| Output stuck on or unexpectedly repeated | Provide a local stop independent of the remote app and bounded output duration/intensity; exact limits need specialist determination. |
| Apparent quietness misread as improvement | Include independent behavioral and welfare observations, not only heart rate, immobility, or rider perception. |
| Handler relies on the system to continue an unsuitable activity | Clearly state uncertainty and keep trained human judgment central. |

## Next research step and success criteria

Prepare an evidence review and observational protocol with an equine veterinarian, qualified behavior specialist, and welfare oversight. No contact or recruitment has been authorized. Define measurable outcomes before collecting data: sensor validity across gait and context, false/missed detections, cue-related adverse behavior, comfort, and recovery assessed by independent observers. Separate within-horse learning from performance on unfamiliar horses and settings.

Bench-test output controls and faults on inert fixtures first. Any subsequent animal study requires separate authorization, consent, welfare review, and stop criteria. The initial proposal includes no deliberate fright, induced bucking, mounted intervention trial, or rider falls. Stop or revise the concept if the device adds stress or cannot distinguish its own effects from the target signal. A successful calming measure in one setting would still not establish rider protection.
