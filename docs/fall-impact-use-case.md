# Falls and impact cushioning

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Horse-to-vest warning](horse-warning-use-case.md)

Research brief, version 0.1 — November 8, 2026. No impact-protection hardware, algorithm, or test has been developed or validated by Vest.

## Intent and scenarios

The user proposes a comfortable wearable that recognizes an impending fall and inflates in time to cushion impact, including falls from a horse, a motorcycle, or altitude. Falls from altitude are explicitly retained as a long-term stretch goal at the user's request. Recording a goal does not establish its feasibility or authorize hazardous testing.

| Scenario | Desired contribution | Questions specific to the scenario |
| --- | --- | --- |
| Horse riding | Reduce injury when a rider is thrown or falls. | Separation versus horse-and-rider falling together; obstacles, rotation, trampling, and equipment fit. |
| Motorcycle | Reduce injury during a crash, ejection, or ground impact. | Horizontal motion, collision before separation, sliding, abrasion, and repeated impacts. |
| Fall from altitude | Explore whether a wearable system can improve survivability through deceleration and/or cushioning. | Impact energy, available stopping distance, body orientation, coverage, and interaction with established descent equipment. |
| Other rapid falls | Preserve the broader aspiration for later definition. | Specify the activity, user, impact surface, and failure mechanism before treating this as one use case. |

The linked horse-monitoring concept also proposes warning the rider before a spook and eventually supporting an emergency dismount. That intent is recorded separately; deliberate jumping is not established as a safe response or a test method.

## Existing baseline and evidence

**Electronic motorcycle airbags:** Alpinestars describes the Tech-Air 5 as a wearable system using accelerometers, gyroscopes, and crash classification to trigger inflation. It is a relevant comparator for automatic detection, not evidence that its algorithm works for horse riding, aviation, or every fall. Manufacturer performance claims are not population injury-reduction estimates. [Product description](https://www.alpinestars.com/products/tech-air-5-system)

**Tethered equestrian airbags:** Helite's equestrian guide describes mechanical activation through rider separation from the saddle attachment. It also identifies a non-activation case when the horse falls and the rider stays in the saddle. Fit, attachment, coverage, and intended activity matter. This is not a general falling-speed detector. [Manufacturer guide](https://www.helite.com/content/uploads/2022/10/2020-09-USER-GUIDE-EQUESTRIAN.pdf)

**Real-world motorcycle outcomes:** A 2025 study of French powered-two-wheeler crash data from 2019–2022 found no statistically significant adjusted association between airbag use and fatality risk (adjusted odds ratio 0.80; 95% CI 0.53–1.21). This does not establish no benefit, equivalence, or a benefit for Vest. Observational selection, relatively few airbag users, and limited injury detail constrain interpretation. Author affiliations include an airbag manufacturer. [Study record](https://pubmed.ncbi.nlm.nih.gov/40930641/)

**Equestrian outcomes:** A 2019 retrospective analysis of 3,305 eventing falls found higher odds of serious/fatal injury among air-jacket users. That association does not prove the jackets caused injury: rider, fall, equipment, and activity differences require further study. It also does not support assuming universal protection because airbags are sold commercially. [Study record](https://pubmed.ncbi.nlm.nih.gov/31160233/)

These are selected starting sources, not an exhaustive review. No specific model or combination is selected for Vest, and the baseline does not replace helmets or other activity-appropriate protection.

## Why a falling-speed threshold is insufficient

The useful event is an impending harmful impact, not simply fast movement. A motorcycle rider can strike an obstacle without a long vertical fall; normal riding, jumps, mounting, and abrupt movements can resemble parts of a fall. Proposed requirements therefore include activity-specific event recognition, body orientation, available time before first contact, and the consequences of false inflation. No threshold or sensor combination has been selected.

Measure the entire timing chain: sensing window, classification, any radio delay, actuator response, and inflation to a protective state. A quoted inflation duration alone does not establish protection before impact. An accelerometer measures acceleration rather than a direct, reliable distance-to-ground signal; integrating motion is subject to error. These are engineering requirements to evaluate, not a working detector.

## Cushioning and the altitude stretch goal

The body still has kinetic energy to dissipate. At fixed mass, doubling speed quadruples kinetic energy; cushioning must manage stopping distance, force distribution, and how the body contacts the surface. [NASA energy explanation](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/conservation-of-energy/)

Project inference: a thin wearable cushion has limited deformation distance, so evidence from selected motorcycle or riding impacts cannot justify a claim that it makes a high-altitude fall survivable. High-altitude research must separately assess slowing descent before contact and managing the remaining impact. No safe height, speed, or body load has been established.

Parachute systems provide an existing aerial-deceleration baseline. USPA describes automatic activation devices that initiate reserve deployment under specified conditions, while emphasizing that they are backups. A Vest airbag is not a substitute for a parachute, fall-arrest equipment, or qualified training. [USPA equipment recommendations](https://www.uspa.org/SIM/4)

Keep altitude falls in the catalog as an open research ambition. A first feasibility review should involve aerospace and impact-biomechanics expertise, define the intended altitude/velocity/orientation range, and examine energy management and compatibility with established equipment. It may conclude that a vest-sized cushion is insufficient, that a separate deceleration architecture is required, or that no practical design is supported. None of those outcomes should be hidden by removing the use case.

## Proposed requirements and first evaluation

| Requirement area | Evidence to seek |
| --- | --- |
| Recognition | Missed incidents and false activations in separately labeled riding, motorcycle, and other datasets; no claim of one universal model. |
| Timing | End-to-end margin before first relevant impact, including any horse-to-rider communication. |
| Protection | Instrumented-surrogate measurements of loads, chest deformation, coverage, and unintended loading across body positions and impact surfaces. |
| Repeated contact | Protection after the first strike, including loss of pressure, tearing, sliding, and further impacts. |
| Fit and compatibility | Expansion space, retention, riding movements, and interference with helmets, garments, controls, or other protective systems. |
| Readiness | Correct model/mode, power or cartridge condition, service/recall status, and clear unavailable states. |
| False confidence | Whether wearers interpret a warning or an inflated vest as permission to jump or take greater risks. |

Begin with exact-manual review and a comparison of existing products against a specific unmet need. Then use inert garments, ordinary dry movements, and staged status examples for comfort/readiness research. Do not merge the horse and motorcycle datasets or outcome claims simply because both use inflation.

Later work could use recorded-event analysis and specialist instrumented dummies or impact fixtures, under a separate reviewed protocol. Do not ask people to fall, jump off horses, crash motorcycles, or attempt altitude drops to test the idea. A dummy result or better classifier score would not establish a real-world survival benefit.

## Verification gaps and decisions

The [Alpinestars manual index](https://www.alpinestars.com/pages/product-manuals) was located, but its linked Tech-Air 5 manual exceeded the web reader's size limit. Only relevant excerpts of the Helite guide were checked. Full model/market/revision, compatibility, service, and approval review remains necessary before equipment selection. Research summaries above use indexed primary-source abstracts; direct retrieval of the motorcycle publisher article and some PubMed pages was restricted or incomplete. Obtain the full papers before detailed study design.

Open decisions are which near-term riding scenario matters most, what specific gap existing products leave, and the scope of the altitude feasibility study. No common chamber, gas system, automatic trigger, or protection claim is shared with the water or avalanche designs without separate evidence.
