
# Research Landscape

This page summarizes the research landscape behind Reader-Centric Requirements Engineering (RCRE).

RCRE is positioned at the intersection of requirement quality, requirement writing guidance, usability-oriented concerns, measurement in requirements engineering, and reader-side requirement consumption.

The purpose of this page is to explain the research context of RCRE without disclosing unpublished empirical data, detailed scoring materials, or confidential industrial examples.

<img width="2262" height="3345" alt="fig_related_work_landscape" src="https://github.com/user-attachments/assets/a65c5f9b-9d92-45c9-98cf-34bea129ea85" />


## Overview

Traditional requirements engineering has long studied how to produce high-quality requirements. Existing work has emphasized whether requirements are complete, consistent, unambiguous, feasible, verifiable, traceable, and necessary.

RCRE builds on this foundation but shifts the analytical focus.

```text
Traditional focus:
Is the requirement well-written?

RCRE focus:
Can the intended reader consume the requirement for a specific engineering task?
```

This shift does not reject conventional requirement quality. Instead, it asks how conventional quality attributes become practically useful from the reader’s perspective.

## Core Problem Space

Requirements are often treated as authored statements. From this view, a requirement is considered good when it satisfies established quality attributes.

However, a requirement may be well-written and still be difficult for downstream readers to use.

For example, a requirement may be:

* clear at the sentence level,
* traceable in a formal tool,
* verifiable in principle,
* and consistent with a review checklist,

but still leave an intended reader unable to determine:

* what question should be asked,
* what meaning should be recovered,
* what artifact should be consulted,
* what decision should be made,
* or what engineering action should follow.

This is the problem space addressed by RCRE.

## Research Landscape Map

The RCRE research landscape can be summarized as follows:

```text
Requirement Quality Attributes
        ↓
Requirement Writing Guidelines
        ↓
Usability, Understandability, and Human-Centered RE
        ↓
Measurement and Inspection Approaches
        ↓
Reader-Side Requirement Consumption
        ↓
Reader-Centricity Construct
        ↓
RI / IN / AC Diagnostic Dimensions
        ↓
Requirements Profile-Based Operationalization
        ↓
Evidence-Based Diagnostic Assessment
```

Each layer contributes to RCRE, but none of them fully subsumes the reader-centricity problem.

## 1. Requirement Quality Attributes

Requirement quality research provides the foundation for evaluating requirements as engineering artifacts.

Commonly discussed quality attributes include:

* completeness,
* correctness,
* consistency,
* unambiguity,
* verifiability,
* traceability,
* feasibility,
* necessity.

These attributes remain essential. They help reduce ambiguity, rework, verification gaps, and lifecycle inconsistencies.

RCRE does not replace these attributes. Instead, it asks whether they are sufficient to explain reader-side requirement use.

For example:

```text
Completeness asks:
Is necessary information present?

RCRE asks:
Is the information needed by the intended reader present, accessible, or appropriately deferred?
```

```text
Traceability asks:
Can related artifacts be followed?

RCRE asks:
Can the intended reader use those links to recover meaning and determine action?
```

```text
Verifiability asks:
Can compliance be checked?

RCRE asks:
Can the intended reader derive the required verification, acceptance, or follow-up task?
```

## 2. Requirement Writing Guidelines

Requirement writing guidelines and controlled expression approaches help improve the form of requirements.

They may include:

* structured writing rules,
* controlled natural language,
* requirement patterns,
* boilerplates,
* ambiguity reduction techniques,
* template conformance checks.

These approaches improve syntactic and semantic regularity. They are especially useful for making requirements clearer, more consistent, and easier to review.

From the RCRE perspective, writing quality is necessary but not sufficient.

A requirement can follow a writing template and still fail to support a reader’s task if role-specific information, context, rationale, accessible references, or downstream action hooks are missing.

```text
Writing guideline focus:
How should the requirement be written?

RCRE focus:
Can the written requirement be consumed by the intended reader?
```

## 3. Usability, Understandability, and Human-Centered RE

Usability-oriented research has influenced requirements engineering in several ways.

Relevant areas include:

* usability as a system quality attribute,
* usability requirements,
* user-centered requirements elicitation,
* human-centered design,
* understandability of requirements techniques,
* readability and cognitive load,
* usability of requirements documents and methods.

RCRE is related to this line of work, but it changes the object of analysis.

In many usability studies, the focus is the final system, product, service, or development method. RCRE focuses on the requirement itself as an information artifact consumed by engineering readers.

```text
Product usability:
Can users effectively use the system?

Requirement consumability:
Can engineering readers effectively use the requirement?
```

In RCRE, the “reader” is not only an end user. The reader may be a designer, verification engineer, software engineer, hardware engineer, functional safety engineer, supplier, service engineer, project manager, or other downstream stakeholder.

## 4. Measurement and Inspection Approaches

Requirements engineering has a long tradition of measurement and inspection.

Relevant approaches include:

* requirements quality measurement,
* Goal-Question-Metric derivation,
* quality requirement evaluation,
* perspective-based inspection,
* empirical requirements quality studies,
* checklist-based review,
* evidence-based assessment.

RCRE builds on this measurement-oriented tradition.

However, RCRE argues that reader-centricity should not be assessed only through impression-based judgment or generic checklists. It should be operationalized through:

```text
Construct Dimension
        ↓
Measurement Goal
        ↓
Evaluation Question
        ↓
Observable Metric
        ↓
Observable Indicator
        ↓
Evidence Variable
        ↓
Diagnostic Profile
```

This structure helps connect conceptual meaning to observable evidence.

## 5. Reader-Side Requirement Consumption

The remaining gap concerns reader-side consumption.

A requirement becomes consumable when the intended reader can move through a minimum consumption chain:

```text
Role-specific questioning
        ↓
Meaning recovery
        ↓
Follow-up action
```

This chain is the conceptual basis of reader-centricity.

A requirement may fail at any point in this chain:

* the reader may not know what question the requirement is expected to answer,
* the reader may not be able to recover the intended meaning,
* the reader may not know which action, decision, artifact, or refinement should follow.

RCRE treats these failures as reader-consumption problems rather than merely sentence-level writing problems.

## 6. Reader-Centricity as a Construct

RCRE defines reader-centricity as a higher-order construct for explaining requirement consumability.

It is organized into three diagnostic dimensions.

### Role-Interrogativity

Role-Interrogativity concerns whether a requirement supports the questions that intended readers must ask before acting.

It is related to:

* reader role identification,
* role-specific information needs,
* responsibility boundaries,
* inquiry entry points.

### Interpretability

Interpretability concerns whether intended readers can recover the requirement’s meaning through a short, reliable, and accessible interpretation path.

It is related to:

* terminology clarity,
* identifier clarity,
* engineering context,
* accessible references,
* assumption control,
* ambiguity control,
* interpretation path manageability.

### Actionability

Actionability concerns whether intended readers can determine the appropriate downstream engineering action.

It is related to:

* explicit action cues,
* conditions and triggers,
* action targets,
* acceptance criteria,
* decision criteria,
* downstream artifact links.

These dimensions should remain analytically separate because a requirement may be strong in one dimension and weak in another.

## 7. Requirements Profile-Based Operationalization

RCRE uses Requirements Profiles to connect the measurement model to specific workflows.

A Requirements Profile defines:

```text
Reader Role
Use Context
Expected Engineering Task
Required Information
Accessible Artifacts
```

This is necessary because reader-centricity is not a context-free property of a requirement sentence.

The same requirement may be sufficiently consumable for one reader but insufficient for another. For example, a requirement may provide enough information for safety review but not enough information for software design, verification planning, supplier implementation, or service interpretation.

A Requirements Profile prevents RCRE from becoming a universal checklist. It makes explicit who is consuming the requirement, for what task, with what information need, and through which accessible artifacts.

## 8. Research Gap

The research gap addressed by RCRE can be summarized in four deficits.

### Conceptual Deficit

Reader-centricity needs a clear construct definition.

Without a construct definition, it remains a general preference rather than a research object that can be discussed, refined, and evaluated.

### Measurement Deficit

Reader-centricity needs observable indicators and evidence-based scoring logic.

Without observable indicators, assessment may depend too heavily on evaluator intuition or tacit expertise.

### Boundary Deficit

Reader-centricity needs to be distinguished from conventional quality attributes.

Without boundary clarification, it may be mistaken for completeness, usability, traceability, verifiability, or general readability.

### Empirical Deficit

Reader-centricity needs evaluation in realistic engineering settings.

Without empirical evaluation, its diagnostic utility for industrial requirements remains unclear.

## 9. RCRE Research Position

RCRE can be summarized as follows:

```text
RCRE is not mainly about how to write a good requirement.

RCRE is about whether an already written requirement can be consumed
as engineering input by intended readers for their role-specific tasks.
```

This positions RCRE as a complementary research direction in requirements engineering.

It connects:

* requirement quality,
* writing guidance,
* usability and understandability,
* measurement and inspection,
* reader-side interpretation,
* downstream engineering action.

## 10. Future Research Space

Future RCRE research may include:

* threshold calibration,
* inter-rater reliability studies,
* task-performance validation,
* before-and-after remediation studies,
* domain-specific Requirements Profiles,
* synthetic benchmark datasets,
* public scoring examples,
* tool-supported diagnostic workflows,
* role-specific requirement views,
* artifact-access support,
* explicit refinement-path tracking.

Potential application domains include:

* functional safety requirements,
* interface requirements,
* diagnostic requirements,
* cybersecurity requirements,
* service requirements,
* system requirements,
* software requirements.

## Public Scope of This Page

This page is a public-facing research landscape.

It does not include:

* industrial requirement datasets,
* detailed empirical results,
* full scoring rubrics,
* project-specific role profiles,
* confidential examples,
* unpublished review-sensitive materials.

More detailed materials may be added after manuscript submission, review, or publication.

---

## Related Pages

* [Overview](overview.md)
* [Conceptual Model](conceptual-model.md)
* [Measurement Model](measurement-model.md)
* [Requirements Profile](requirements-profile.md)
* [Discussion](discussion.md)
* [Validity Boundaries](validity-boundaries.md)
* [Resources](resources.md)
* [Publications](publications.md)
* [Back to Home](../index.md)

