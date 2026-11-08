# Horse-to-vest warning and emergency dismount research

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Rider impact protection](fall-impact-use-case.md) · [Horse calming research](horse-calming-use-case.md)

Research brief, version 0.1 — source review November 8, 2026. No device, predictive model, animal study, or rider trial has been developed or conducted.

## The user's intended system

A horse wears sensors that monitor the horse, with a connection to the rider's vest. The goal is to recognize an impending spook early enough to warn the rider before control is lost. The user also imagines an emergency dismount supported by vest inflation, including a jump from the horse.

Preserve that complete idea as a research ambition. It contains three distinct claims that need evidence: useful prediction before the reaction; reliable, timely delivery of a warning; and a response that improves outcomes. Neither enough time to dismount nor safe landing with an airbag is established. The draft does not prescribe immediate dismounting or jumping in response to an alert.

The later [horse-worn stress monitoring and calming brief](horse-calming-use-case.md) explores a separate intervention on the horse, including candidate acoustic or tactile cues. A rider warning and a calming intervention are different functions; evidence for one does not validate the other. Both retain passive observation as the first proposed research mode, and neither selects an automatic rider-airbag trigger.

## What the evidence supports so far

| Source | Relevant result | What it does not establish |
| --- | --- | --- |
| [Sympathetic arousal study, 2023](https://pmc.ncbi.nlm.nih.gov/articles/PMC9855141/) | Electrodermal signals in 15 horses responded to both feeding and startle conditions. | Arousal is not specific to danger or fear; this was not a validated warning of an imminent mounted-riding spook. |
| [Behavioral and cardiac startle study](https://pmc.ncbi.nlm.nih.gov/articles/PMC11611493/) | Researchers measured behavior, heart rate, and variability in retired Thoroughbreds around a standardized startle test and training. | Measuring a response does not prove a usable signal exists before its onset. |
| [Gobbo et al., 2025](https://pubmed.ncbi.nlm.nih.gov/40628935/) | Machine-learning analysis of 101 Lipizzan horses investigated features associated with fear reactivity and fearfulness. | Trait/reactivity classification is different from predicting the next spook several seconds in advance in a new horse. |

This is a preliminary evidence scan, not proof that prediction is impossible or that a product works. The first two papers were available as indexed source content; direct PMC access presented browser challenges. The third abstract was retrieved directly. Full methods, validation, and conflicts-of-interest review remains a prerequisite to designing a study.

## Candidate observations, without choosing hardware

Potential signals include heart rate and beat-to-beat variation, motion/posture, and other physiological measures supported by equine research. Their value must be established against exercise, gait changes, excitement, discomfort, environment, and sensor artifacts. Candidate placement must be reviewed for rubbing, pressure, snagging, and interference with tack. No attachment location or physiological threshold is prescribed here.

Start with individual baselines and context, while testing whether any finding transfers to unfamiliar horses, riders, tack, and environments. A sudden external stimulus may provide little or no advance warning. Do not label a system that recognizes movement after onset as predicting the spook.

## Link to the rider's vest

The proposed path is horse sensing, risk estimation, local communication, and a rider-facing indication. The initial research mode should record candidate events without issuing live riding advice or triggering inflation. A warning interface can first be evaluated using recordings and an inert vest away from horses.

Later requirements include correct horse/rider pairing, signal age, communication delay, dropout, battery state, and explicit unavailable indications. Absence of an alert must not mean that the horse is safe. Alert sound, vibration, rider distraction, and the horse's reaction to any signal are themselves evaluation questions.

Keep the warning function and the rider airbag's deployment logic separately validated. A higher arousal estimate must not automatically become an inflation command or a directive to leave the saddle. False or late warnings, changed rider movement, and unexpected inflation could increase risk.

## Evaluate prediction and the response separately

First define an event with equine-behavior and veterinary specialists, including observable onset and annotation uncertainty. In later authorized observational work, use synchronized behavior and sensor records, independent annotations, and naturally occurring events. Do not deliberately frighten horses or create mounted falls for this project.

For analysis, count missed events, false warnings per riding hour, positive predictive value, and usable lead time after processing and communication. Test on held-out horses and sessions; do not split adjacent windows from one incident across training and evaluation. Compare against a simple baseline and expert observation. No numerical performance target or dataset has been selected.

Even good prediction would not establish the benefit of dismounting. A separate human-factors and equestrian-safety review must ask whether any suggested response is practical and safer in context. Study understanding with tabletop scenarios first. Emergency dismount cushioning remains a stretch idea requiring independent impact evidence; no human jumping trial or automatic dismount instruction is included.

## Next decisions

Identify the riding context, define what counts as a spook, and clarify whether the first useful output is retrospective training feedback or a prospective warning. Seek equine veterinary/behavioral and rider-safety input before recruiting horses or riders. Record welfare, consent, data retention, and stopping criteria in any future protocol. No animal recruitment, equipment purchase, or intervention is authorized by this brief alone.
