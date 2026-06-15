# Reader-Centric Requirements Engineering

This repository hosts the public preview site for Reader-Centric Requirements Engineering (RCRE).

RCRE studies how requirements become consumable by intended engineering readers. It focuses on three dimensions:

- Role-Interrogativity,
- Interpretability,
- Actionability.

This repository currently contains public-facing conceptual materials only. Empirical data, detailed scoring materials, confidential examples, and full evaluation results are withheld until the related paper has been submitted and reviewed.

## Public Preview Status

This repository is an early research communication site, not a complete tool release.

## License

The site content and future templates will be released under an appropriate open license after publication planning is finalized.

## Contact

Contact information will be added after the public release scope is finalized.

graph TD
    classDef default fill:#f9f9f9,stroke:#333,stroke-width:1px;
    classDef highlight fill:#e1f5fe,stroke:#0288d1,stroke-width:2px;
    classDef decision fill:#fff3e0,stroke:#f57c00,stroke-width:2px;
    classDef final fill:#e8f5e9,stroke:#388e3c,stroke-width:2px;

    subgraph Step 1: Objective Measurement
        E1(Evaluator 1<br>Independent Score)
        E2(Evaluator 2<br>Independent Score)
        E3(Evaluator 3<br>Independent Score)
    end

    subgraph Step 2: Disagreement Identification
        COMP{Scores<br>Identical?}:::decision
    end

    subgraph Step 3: Evidence-Driven Calibration
        RP[Cross-reference with<br>Requirements Profile]:::highlight
        EVID[Search for Explicit Evidence<br>in Artifacts DBC, ICD, etc.]:::highlight
        ADJ[Adjust Score Conservatively<br>if Evidence is Implicit/Missing]:::highlight
    end

    subgraph Step 4: Policy-Based Decision
        FIN[Final Consensus Score<br>M_RI, M_IN, M_AC]:::final
        TH{Below<br>Threshold 0.5?}:::decision
        RCD1((RCD = 1<br>Defect Flag))
        RCD0((RCD = 0<br>Pass))
    end

    E1 --> COMP
    E2 --> COMP
    E3 --> COMP

    COMP -- No Disagreement --> FIN
    COMP -- Disagreement Detected --> RP
    RP --> EVID
    EVID --> ADJ
    ADJ -. Re-evaluate .-> COMP

    FIN --> TH
    TH -- Yes --> RCD1
    TH -- No --> RCD0
