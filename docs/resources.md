# Resources

This page summarizes the planned public resources for Reader-Centric Requirements Engineering (RCRE).

The current repository is a public preview. Detailed empirical data, industrial examples, full scoring materials, and confidential evaluation artifacts are not included at this stage.

## Research Context Materials

The following public-facing materials summarize the research context of RCRE:

- [Research Landscape](research-landscape.md)
- [Research Positioning](research-positioning.md)
- [Conventional Quality Map](conventional-quality-map.md)
- [Terminology](terminology.md)
- [Research Roadmap](research-roadmap.md)

## Available Now

The following materials are available in the current public preview:

* RCRE overview,
* conceptual model summary,
* reader-centricity dimension descriptions,
* Requirements Profile concept,
* public validity boundaries,
* synthetic example format,
* publication list.

## Planned After Paper Submission

The following materials may be added after manuscript submission:

* simplified Requirements Profile template,
* public-facing reader-consumption checklist,
* synthetic requirement examples,
* figure source files,
* terminology summary,
* BibTeX entries for related publications.

These materials will remain public-safe and will not include confidential industrial data or detailed empirical scoring records.

## Planned After Review or Publication

The following materials may be considered after review or publication:

* refined scoring guide,
* sanitized case examples,
* synthetic benchmark dataset,
* controlled replication package,
* evaluator training examples,
* prototype tool documentation.

The release scope will depend on publication status, confidentiality constraints, and the maturity of the measurement materials.

## Not Currently Public

The following materials are not public at this stage:

* industrial requirement datasets,
* full empirical evaluation results,
* actual project role profiles,
* detailed scoring records,
* confidential artifact links,
* complete scoring rubrics,
* organization-specific thresholds,
* ECU-level contextual details,
* unpublished reviewer-sensitive materials.

## Suggested Repository Structure

A minimal public repository structure is:

```text
rcre/
├── index.md
├── README.md
├── _config.yml
└── docs/
    ├── overview.md
    ├── conceptual-model.md
    ├── measurement-model.md
    ├── requirements-profile.md
    ├── discussion.md
    ├── validity-boundaries.md
    ├── examples.md
    ├── resources.md
    └── publications.md
```

## Future Resource Types

Future releases may include several types of resources.

### Templates

Templates may support early adoption of RCRE without exposing the full research dataset.

Possible templates include:

* Requirements Profile template,
* reader-role definition template,
* expected-task description template,
* required-information table,
* accessible-artifact checklist,
* missing-information disposition sheet.

### Checklists

Public checklists may help readers apply RCRE thinking at a lightweight level.

Possible checklist questions include:

* Who is expected to consume this requirement?
* What engineering task should the reader perform?
* What information is required for that task?
* Is the information present in the requirement?
* If not present, is it recoverable through an accessible artifact?
* Is the missing information intentionally deferred to a downstream artifact?
* Can the reader determine the next engineering action?

These checklists are not intended to replace the full measurement model.

### Examples

Examples will use synthetic or sanitized requirements.

The purpose of examples will be to show how reader-centricity can be discussed, not to disclose confidential industrial materials.

Example materials may include:

* simplified requirement statements,
* reader-role examples,
* expected-task examples,
* required-information examples,
* possible reader-consumption issues,
* possible follow-up actions.

### Replication Materials

Replication materials may be released only when they can preserve the relevant reader-consumption characteristics without exposing confidential information.

Possible replication materials include:

* synthetic benchmark requirements,
* public scoring examples,
* simplified evaluation instructions,
* anonymized aggregate results.

## Requirements Profile Template Preview

A simplified public Requirements Profile template may use the following structure:

```text
Requirement ID:
Requirement Text:

Reader Role:
Use Context:
Expected Engineering Task:

Required Information:
- 
- 
- 

Accessible Artifacts:
- 
- 
- 

Potential Reader-Consumption Issue:
- 

Possible Follow-Up:
- 
```

This template is intentionally simplified. It does not represent the complete research scoring procedure.

## Missing-Information Disposition Preview

Future public materials may also include a simplified missing-information disposition sheet.

```text
Information Item:
Required for Current Reader Task? Yes / No
Available in Requirement? Yes / No
Recoverable through Accessible Artifact? Yes / No
Intentionally Deferred? Yes / No
Target Downstream Artifact:
Responsible Role:
Follow-Up Needed:
```

This structure helps distinguish between information that should be clarified immediately, information that is recoverable through accessible references, and information that is intentionally refined in downstream work products.

## Prototype Tool Direction

A future RCRE prototype may support:

* Requirements Profile creation,
* reader-role selection,
* required-information mapping,
* evidence recording,
* RI / IN / AC diagnostic visualization,
* missing-information disposition tracking,
* export of review notes.

No prototype implementation is currently released.

## Contribution Policy

External contributions are not open at this stage.

After the research scope and publication plan are stabilized, contribution guidelines may be added for:

* terminology suggestions,
* synthetic examples,
* template improvements,
* tool-related issues,
* replication feedback.

## License

The license for public resources will be finalized after the publication and release strategy is determined.

Until then, the repository should be treated as a research preview rather than a complete open-source release.

## Related Pages 
- Previous: [Examples](examples.md)
- Next: [Publications](publications.md)
- [Back to Home](../)
