# Evidence and sources

[Home](../README.md) · [Decisions](decisions.md) · [Prototype](prototype.md)

Source review date: **November 8, 2026**. This ledger preserves the voice-conversation research and its limitations. Core sources were reopened during documentation; entries marked “follow-up” retain prior research findings and need renewed full-source review before use in operational guidance. Product descriptions are manufacturer claims, not independent validation of Vest.

This ledger covers the original water scenario. See the [avalanche research brief](avalanche-use-case.md) for snow-burial sources and separate limitations; boating evidence does not validate avalanche equipment.

Additional source summaries are in the [fall-impact brief](fall-impact-use-case.md) and [horse-warning brief](horse-warning-use-case.md). Each distinguishes existing-product behavior, observational research, and proposed requirements; evidence does not transfer automatically across activities.

## Wear, fit, and readiness

| Evidence | Finding and implication | Limits |
| --- | --- | --- |
| [USCG annual report listing](https://www.uscgboating.org/statistics/accident_statistics.php) and [2024 report](https://uscgboating.org/library/accident-statistics/Recreational-Boating-Statistics-2024.pdf) | Latest available annual report at review: 2024; the listing indicated 2025 pending November 16. There were 556 deaths; 76% drowned where cause was known; 87% of drowning victims were not wearing a PFD where use was known. | Recorded fatal-case proportions, not a product risk-reduction estimate or proof nonwear caused each death. |
| [2025 USCG wear observation study](https://uscgboating.org/library/national-live-jacket-wear-study/2025-Life-Jacket-Wear-Rate-Observation-Study-Report.pdf) | Adult wear excluding personal watercraft: 9.7%; adult kayakers: 76.4%. | Missing 33 of 125 sites, historically with higher wear, may slightly underestimate overall use. Motorboater patterns do not generalize to kayakers. |
| [Quistberg et al., 2014](https://pmc.ncbi.nlm.nih.gov/articles/PMC4310692/) | Cross-sectional study of 675 adult small-motorboat users in western Washington, with data collected in 2008: perceived discomfort associated with lower wear; inflatable use with higher wear. | Observational association, not causation or proof that a new vest increases wear. |
| [Matched cohort study](https://pubmed.ncbi.nlm.nih.gov/20889519/) — follow-up | USCG 2000–2006 data: adjusted drowning RR 0.51, 95% CI 0.35–0.74. | Extensive exclusions and missing data may bias the estimate. It is not an estimate for our product. |
| [NIOSH field guidance](https://www.cdc.gov/niosh/docs/2013-131/pdfs/2013-131.pdf), [study](https://pubmed.ncbi.nlm.nih.gov/22123533/) — follow-up | Roughly 200 commercial fishermen evaluated PFDs; preferences differed by activity and suitable foam and inflatable options existed. | Commercial work differs from recreational paddling. |
| [MAIB: Eder Sands](https://www.gov.uk/maib-reports/fall-overboard-from-fishing-vessel-eder-sands-with-loss-of-1-life) | Probable loss of a loosely fitted lifejacket; investigation trials reproduced slipping out. | Commercial-fishing case, not a population frequency or universal mechanism. |
| [USCG Safety Alert 13-16](https://www.dco.uscg.mil/Portals/9/DCO%20Documents/5p/CG-5PC/INV/Alerts/1316.pdf) — follow-up | Documents fatal unsuccessful-inflation incidents and hazards involving leaks, fabric deterioration, and incorrectly fitted CO2 cylinders. | No population failure rate. Prior direct fetch returned 403; obtain and review an accessible official copy. |
| [MAIB: Orca/Shoreway](https://assets.publishing.service.gov.uk/media/555b29fde5274a74ca000007/MAIBInvReport10_2015.pdf) — follow-up | Skipper's lifejacket did not inflate; loose cylinder and previously triggered mechanism were identified. | Incident evidence, not comparative reliability. |

## Alerting and exposure

[CDC's commercial-fishing falls analysis](https://www.cdc.gov/mmwr/volumes/67/wr/mm6716a2.htm) examined 204 fatal falls during 2000–2016. Unwitnessed falls and difficult recovery motivate investigating hands-free alerts, but do not quantify benefits for lake recreation. Review its [erratum](https://www.cdc.gov/mmwr/volumes/67/wr/mm6721a7.htm) before using precise subgroup figures (follow-up).

[NWS cold-water guidance](https://www.weather.gov/safety/coldwater) distinguishes immediate cold shock from later hypothermia. Water temperature alone neither diagnoses hypothermia nor determines whether rescue is needed. Heating is not our initial intervention.

## Existing product baseline

| Product/source | Manufacturer-described capability | Dependency or limit |
| --- | --- | --- |
| [Ocean Signal PLB3](https://oceansignal.com/products/plb3-ais-personal-locator-beacon/) | Satellite Cospas-Sarsat alerting plus local AIS; no phone required. Correctly fitted and armed compatible lifejacket inflation can deploy its antenna and activate it (semi-automatic). | Insufficient inflation may require manual help; antenna orientation, clearance above water, and sky view matter. **No DSC transmission.** |
| [ACR ResQLink AIS](https://www.acrartex.com/products/resqlink-ais-personal-locator-beacon/) — follow-up | Another satellite/local beacon with lifejacket-inflation activation. | Installation and activation dependencies require its exact manual; not interchangeable with PLB3 instructions. |
| [sMRT ALERT](https://www.smrtsos.com/products/distress-beacons/smrt-alert), [manual](https://www.smrtsos.com/perch/resources/smrt-alert-manual-en-26.pdf) | Armed water activation after two seconds; local AIS/DSC. | Compatible receivers must be within range. Insufficient sensor contact can require manual activation; manual detail needs renewed review. |

[NOAA RLS explanation](https://www.sarsat.noaa.gov/faqs/): receipt/localization/routing acknowledgment does not establish rescue dispatch or arrival time. [NOAA beacon testing policy](https://www.sarsat.noaa.gov/emergency_beacon-testing/): use manufacturer self-test procedures or authorized controlled testing; no casual live distress broadcasts. The planned dry study uses inert representations for beacon tasks.

## Interpretation

Comfort, correct fit, maintenance, and hands-free alerting are plausible priorities supported by different kinds of evidence. Their ordering is a working judgment, not proof of the greatest causal impact. Existing products already address important parts of the original idea. Neither novelty nor efficacy of any proposed Vest hardware has been established.

## Link access check

All external source URLs in these drafts were attempted on November 8, 2026. The USCG alert returned HTTP 403, the Elite owner manual was inaccessible to the web reader, and the NIOSH study PubMed page presented a browser challenge. Other URLs returned source content. Successful retrieval is not a complete manual review; the follow-up and instruction-mapping gaps above remain open.
