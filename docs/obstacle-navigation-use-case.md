# Obstacle sensing and navigation assistance

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Decisions](decisions.md)

Open research concept, version 0.1 — November 9, 2026. No navigation device, selected sensor system, user study, or demonstrated protective benefit exists. Child water safety remains the project's highest priority.

## Intended application

Explore a vest for blind and low-vision people that uses sensors to detect nearby objects and obstacles, then conveys useful information about the surroundings to the wearer. Possible feedback includes directional vibrations or other accessible cues representing obstacle location, distance, and urgency. The aim is to support spatial awareness and obstacle avoidance while preserving the wearer's control over movement.

The user's long-term ambition is to make movement through complex environments possible even without sight, including **running through a forest at night while avoiding obstacles**. Keep that ambition visible as an open area to pursue. Collision-free movement, safe running speed, complete coverage, and reliable operation in darkness are not established capabilities.

Hummingbird agility inspired the idea. The proposed biological sensing mechanism remains unresolved; no further hummingbird investigation is part of this addition, and no wing-based technology is claimed to have been identified or reproduced.

## Proposed sensing and feedback flow

1. Sensors worn on or connected to the vest observe the surrounding space. Candidate approaches could include depth/ranging sensors or cameras; no technology or placement is selected.
2. Processing estimates relevant obstacle positions and distances, together with uncertainty and information age. Coverage must account for the wearer's body and movement, not just a narrow path directly in front of a sensor.
3. The vest communicates understandable cues, potentially through a spatial arrangement of vibration points. The wearer must be able to distinguish an obstacle indication from a suggested direction of travel and from a device fault.
4. Missing, blocked, stale, or unreliable sensing produces a clear unavailable indication. Silence must not be interpreted as proof that the way is clear.

Related work already explores this general approach: the ALVU study combined distance sensors with tactile feedback and reported controlled walking tasks involving 12 blind users. That provides a relevant comparator, not evidence that this Vest concept can support nighttime forest running. [Katzschmann, Araki, and Rus, 2018](https://pubmed.ncbi.nlm.nih.gov/29522402/)

## Open questions

- **Coverage:** How would the system handle branches at head height, trunks, thin obstacles, roots, uneven ground, and drop-offs? Detecting an object and establishing traversable ground are different problems.
- **Conditions:** What remains detectable in darkness, rain, fog, dense vegetation, and changing light? Sensor performance must be measured in the intended conditions.
- **Timing:** Can sensing, processing, cue interpretation, and the wearer's response occur early enough at the intended movement speed? No range, latency limit, or safe speed is specified.
- **Usability:** Which cues are understandable, comfortable, and learnable without overwhelming the wearer or masking useful environmental sounds? Multiple obstacles and competing Vest alerts need explicit handling.
- **Reliability:** How are power loss, blocked sensors, garment movement, lost connections, and false or missed detections exposed?
- **Accessibility and privacy:** How can blind and low-vision users shape the design, pairing, controls, and training? What data can be processed locally without retaining unnecessary images or travel history?

## Next step

Record the concept now; hardware selection and a detailed study remain open. Any later work should be developed with blind and low-vision collaborators and orientation-and-mobility expertise. Begin with requirements, recorded or synthetic scenes, and bench evaluation before separately reviewed, controlled walking studies. Consider the wearer's usual mobility aids and strategies rather than assuming replacement.

Outdoor running and nighttime forest use remain later research ambitions requiring their own evidence. This brief authorizes no recruitment, obstacle-running trials, or reliance on an experimental vest for navigation.
