# Visual overview

[Home](../README.md) · [Use-case catalog](use-cases.md) · [Decisions](decisions.md)

November 8, 2026. These diagrams organize research, not the components of a tested product. Text descriptions are included for readers who cannot view Mermaid diagrams.

## Research areas

```mermaid
flowchart TD
    V["Vest research"]
    V --> W["Water safety<br/>First dry usability project"]
    V --> A["Avalanche<br/>Breathing space and rescue"]
    V --> I["Impact cushioning"]
    V --> H["Horse-to-vest warning<br/>Prediction research"]
    I --> R["Horse riding and motorcycles<br/>Separate impact scenarios"]
    I --> F["Falls from altitude<br/>Long-term stretch goal"]
    H -.-> D["Emergency dismount assistance<br/>Unvalidated stretch concept"]
    I -.-> D
    classDef current fill:#e8f1fa,stroke:#285d85,color:#172e40;
    classDef stretch fill:#fff3df,stroke:#8a641e,color:#49340f;
    class W current;
    class F,D stretch;
```

The first defined project is the [water preparation companion](prototype.md) and its proposed dry usability study. Other branches are [avalanche research](avalanche-use-case.md), [impact protection](fall-impact-use-case.md), and [horse-to-vest warning](horse-warning-use-case.md). Falls from altitude remain an explicit long-term goal. The dashed connections indicate that emergency dismount assistance depends on both warning/response research and impact research; they do not imply that a warning makes jumping safe.

The catalog also retains other rapid falls for later definition. None of these branches establishes a universal vest, common trigger, or shared safety certification.

## Proposed path from idea to evidence

```mermaid
flowchart TD
    C["Current: source review, concepts,<br/>paper mock-up and draft protocols"]
    C --> Q["Next: resolve requirements and manual gaps<br/>with relevant specialists"]
    Q --> U["Proposed: dry usability<br/>and non-interventional observation"]
    U --> G{"Evidence supports<br/>further investigation?"}
    G -->|No| R["Revise, narrow or stop the concept"]
    R --> Q
    G -->|Yes| B["Separately reviewed specialist studies<br/>Bench, mannequin or other appropriate methods"]
    B --> E["Assess results, failure modes<br/>and remaining validation needs"]
    E -->|More work needed| R
    E -->|Evidence supports handoff| P["Reproducible documentation<br/>with bounded claims and limitations"]
    classDef current fill:#e8f1fa,stroke:#285d85,color:#172e40;
    class C current;
```

Only the documentation stage exists today. The next step is resolving requirements and source gaps; dry usability and any later specialist work remain proposed. Progress depends on evidence and may lead to revision or abandonment. This diagram does not authorize experiments, prescribe one validation route for every use case, or imply certification.

Early research documents can be shared for review before later stages are complete. Public sharing and a reuse license do not establish that the device ideas work. See [next steps](next-steps.md) and [license scope](../LICENSING.md).
