# Harmful-water sensing and alerts

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Highest priority: child water-approach warning](child-water-proximity-use-case.md)

Research brief, version 0.1 — source review November 8, 2026. No sensor, water-quality model, working alert system, or protective benefit has been demonstrated by Vest. Child water-approach warning remains the highest priority.

## Intended benefit

Explore whether sensors associated with a vest can identify specified harmful bacteria or other water hazards and promptly alert the wearer to leave the water safely. For a child, the supervising caregiver would need the alert and responsibility for the response; the concept must not rely on a young child's judgment or ability to exit unaided.

The aspiration is an immediate warning, but **fast communication after detection is different from immediate detection**. Sampling and analysis may impose delay, and contact with water may already have occurred before a worn sensor obtains a sample. This is not a way to certify a lake as safe, prevent drowning, or justify entering questionable water.

The child-protection priority concerns warning before approach to water. This additional track concerns water quality. A favorable water-quality reading would never make water appropriate for an unsupervised child or a child unable to swim.

## Separate the targets

| Target or approach | What the source supports | What remains unproven for a vest |
| --- | --- | --- |
| Fecal indicator bacteria | EPA describes laboratory Enterococcus qPCR methods with results in less than four hours, compared with about 24 hours for culture methods. These indicators help beach managers assess microbial contamination. [EPA same-day monitoring research](https://www.epa.gov/water-research/development-and-validation-same-day-monitoring-methods-recreational-water) | These methods are not an instant wearable assay, and an indicator is not a detector for every pathogen. No method or target has been selected for Vest. |
| Cyanobacteria and their toxins | EPA describes exposure through contact and ingestion, and warns that appearance alone cannot establish whether a bloom is harmful. [EPA harmful-algal-bloom guidance](https://www.epa.gov/habs/how-people-and-animals-are-exposed-habs-and-their-toxins) | A bloom-related signal is not automatically a toxin measurement. The relevant organism or toxin, detection limit, and response require explicit definition. |
| Particular chemicals | EPA's sensor resources describe technologies for selected contaminants as well as common water measurements. [EPA Water Sensors Toolbox](https://www.epa.gov/water-research/water-sensors-toolbox) | A sensor for one substance cannot establish the absence of unrelated hazards. No general detector for "anything harmful" is established here. |
| General measurements or prediction | The same toolbox describes pH, temperature, conductivity, dissolved oxygen, turbidity, and predictive uses of chlorophyll measurements. | Our inference: these measurements can supply context or candidate warning signals, but they do not on their own establish pathogen-free or toxin-free water. Any proxy or model needs validation for its claimed target and setting. |

All three EPA sources were opened on November 8, 2026. This is an initial feasibility scan, not an exhaustive survey of emerging biosensors, a current beach clearance, or validation of a commercial product.

## Candidate routes to investigate

1. **Official advisory information:** explore presenting the relevant authority's closure or warning with its source, location, issue time, and coverage. This may help before entry, but it is an information service, not sensing by the vest. Missing, stale, or unavailable advisories must not become a "safe" state. No live advisory integration exists yet.
2. **General water measurements:** consider instrumented environmental observations as research data only. Do not label a generic sensor anomaly as confirmed bacteria or translate an ordinary reading into permission to swim.
3. **Target-specific sensing:** retain direct wearable detection as a longer-term research aim. First choose one defined hazard and compare candidate methods, detection time, specificity, calibration, maintenance, sample handling, power, and independent reference methods with water-quality specialists.

No route has been chosen, and the advisory route does not replace the user's direct-sensing ambition. Existing closures and public-health advice take precedence over a proposed device reading.

## Alert and failure questions

The proposed chain is sample or advisory acquisition, quality/validity assessment, a target-specific interpretation, and delivery of an understandable warning to the wearer and, where appropriate, caregiver. Distinguish a supported hazard indication, an uncertain result, and unavailable monitoring. Do not display an overall green "safe water" result.

Evaluate missed contaminants, false positives, interference, fouling, calibration drift, dry sensors, intermittent immersion, and delays. A vest may sit above the water; a measurement at one place and time need not represent exposure elsewhere. The display needs the measured target, sampling location/time, limitations, and sensor status. Different hazards may need different methods and responses.

Warnings should support an orderly, safe exit and caregiver assistance, not panic or automatic inflation. Alert delivery is not proof of recognition or completed exit. Water-quality alerts must remain separate from child approach detection, flotation, and emergency distress signaling.

## Next safe research step

Preserve the full idea, then narrow one initial hazard and intended environment with environmental microbiology/water-quality and human-factors specialists. Draft requirements and a paper alert interface; compare detection time and failure modes before choosing hardware.

Use published data, synthetic readings, and dry interface scenarios first. Any later analytical validation needs a separately reviewed laboratory plan and appropriate reference methods. This brief proposes no collection or culturing of harmful organisms, contaminated-water exposure, or human swimming trials. No person, especially a child, should enter water to see whether a prototype warns them.

Until evidence establishes a specific capability, the public description is research into harmful-water alerts, not a water-safety guarantee. If a suspected harmful bloom is present, follow official guidance to stay out rather than waiting for a device indication. [EPA guidance](https://www.epa.gov/habs/how-people-and-animals-are-exposed-habs-and-their-toxins)
