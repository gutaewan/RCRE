# Discussion

RCRE is intended to complement existing requirement quality practices, not replace them.

Conventional requirement reviews remain essential. They help evaluate whether requirements are clear, complete, consistent, traceable, feasible, verifiable, and aligned with relevant engineering expectations. RCRE adds a different diagnostic view: whether intended readers can consume a requirement for their role-specific engineering tasks.

In this sense, RCRE is not a stricter version of conventional requirement quality. It asks a different question:

> Does the requirement provide enough support for a specified reader to ask the right questions, recover the intended meaning, and determine what action should follow?

## Requirement Quality as a Reader-Task Relation

RCRE treats requirement quality not only as a property of an authored statement, but also as a relation among:

```text
Requirement
Reader Role
Engineering Task
Accessible Artifacts
```

A requirement may be acceptable in a conventional review but still require additional support for a particular downstream reader. For example, a requirement may express intent clearly but still leave a verification engineer without sufficient test conditions or acceptance criteria. Another requirement may be understandable to the authoring organization but difficult for a supplier to interpret because key interface assumptions are implicit.

This relational view is central to RCRE.

## Three Diagnostic Dimensions

RCRE organizes reader-centricity into three dimensions:

* **Role-Interrogativity (RI)**
  Whether the requirement supports the questions that intended readers must ask before acting.

* **Interpretability (IN)**
  Whether intended readers can recover the requirement’s meaning through a short, reliable, and accessible interpretation path.

* **Actionability (AC)**
  Whether intended readers can determine the appropriate downstream engineering action.

These dimensions should remain analytically separate. A requirement may support role-specific questioning but still be difficult to interpret. Another requirement may be interpretable but not actionable. A single overall score may hide these differences.

## Methodological Implication

RCRE separates three levels that are often mixed together in requirements assessment:

```text
Construct Model
        ↓
Measurement Model
        ↓
Requirements Profile
```

The construct model defines what reader-centricity means.
The measurement model translates the construct into dimensions, metrics, observable indicators, evidence variables, and diagnostic outputs.
The Requirements Profile instantiates the model for a specific reader role, task, required information, and artifact-access context.

This separation is important because RCRE should not become an arbitrary checklist. Each assessment should make explicit:

* which reader role is being considered,
* what task the reader is expected to perform,
* what information is required for that task,
* which artifacts are reasonably accessible,
* what observable evidence supports the assessment.

## Practical Implication

In industrial requirements engineering, RCRE can be used as a diagnostic extension to existing review processes.

It can help teams ask:

* Which reader role is expected to consume this requirement?
* What task must that reader perform?
* What information does that task require?
* Is the required information present, accessible, or intentionally deferred?
* Can the reader recover the intended meaning without excessive search or guesswork?
* Can the reader determine the next engineering action?

RCRE is especially useful when requirements cross role, organizational, supplier, lifecycle, or toolchain boundaries.

## Implications for Traceability and Tool Support

Traceability is valuable only when it supports practical meaning recovery.

A trace link may formally exist but still be insufficient if the linked artifact is inaccessible, overly broad, outdated, ambiguous, or not useful for the reader’s task. Similarly, a downstream artifact link supports actionability only when it helps the reader determine what work product, decision, test, design item, or evidence should follow.

Tool support for RCRE should therefore emphasize:

* role-specific requirement views,
* local definitions,
* accessible references,
* explicit refinement paths,
* links to downstream work products,
* visible responsibility boundaries.

## No Universal Rubric

RCRE does not prescribe a single universal rubric for all domains.

An interface requirement, functional safety requirement, diagnostic requirement, cybersecurity requirement, and service requirement may require different information to support reader-side consumption. Applying the same detailed checklist to all of them may either omit important domain-specific information or impose irrelevant criteria.

The invariant part of RCRE is the construct-based logic:

```text
Define the reader role
Define the task
Define the required information
Define accessible artifacts
Collect observable evidence
Assess RI, IN, and AC
Interpret the diagnostic profile
```

What changes across domains is the Requirements Profile and the operational meaning of sufficient evidence.

## Current Public Scope

This page provides a public-facing discussion of RCRE. It does not disclose industrial datasets, detailed scoring records, complete rubrics, project-specific role profiles, or empirical evaluation details.

More detailed discussion may be added after manuscript submission, review, or publication.


## Related Pages 
- Previous: [Requirements Profile](requirements-profile.md)
- Next: [Validity Boundaries](validity-boundaries.md)
- [Back to Home](../)
