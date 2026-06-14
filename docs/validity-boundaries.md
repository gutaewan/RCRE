# Validity Boundaries

This page summarizes the current boundaries of the Reader-Centric Requirements Engineering (RCRE) research program.

RCRE is presented here as a research framework for diagnosing requirement consumability. It should not be interpreted as a universal compliance method, a complete tool, or a validated defect classifier.

## RCRE Is Not a Compliance Claim

RCRE does not replace existing requirement quality standards, functional safety reviews, or compliance-oriented assessments.

A reader-consumption weakness does not automatically mean that a requirement is factually wrong, non-compliant, unsafe, or unusable. It indicates that additional reader support may be needed for a specific role and task.

RCRE should therefore be used as a complementary diagnostic perspective, not as a substitute for established engineering review practices.

## RCD Is a Diagnostic Flag

In RCRE, a reader-consumption diagnostic flag should be interpreted as a follow-up signal.

It may indicate that a reader needs additional support to:

* formulate role-specific questions,
* recover the intended meaning,
* access supporting artifacts,
* identify the next engineering action,
* understand where missing information should be refined.

An RCD should not be interpreted as a conventional defect label unless an organization explicitly defines such a policy.

## Thresholds Require Calibration

Any operational threshold used in RCRE assessment should be treated as context-specific.

Thresholds may depend on:

* organizational maturity,
* role expectations,
* artifact accessibility,
* toolchain integration,
* lifecycle stage,
* domain-specific practices,
* evaluator training,
* expected evidence quality.

A threshold that is useful in one organization or domain may not be appropriate in another. Future work should focus on calibration procedures and task-performance validation.

## Requirements Profiles Affect the Result

RCRE assessment depends on the Requirements Profile used for evaluation.

A Requirements Profile defines:

```text
Reader Role
Use Context
Expected Engineering Task
Required Information
Accessible Artifacts
```

If an RP omits an important reader role, assumes an unrealistic task, or defines artifact accessibility incorrectly, the resulting assessment may not represent the actual workflow.

For this reason, RP construction decisions should be documented, including:

* selected reader roles,
* expected tasks,
* required information,
* accessible artifacts,
* role-applicability assumptions,
* known exclusions.

## Reliability Requires Further Study

RCRE assessment uses observable evidence, but expert judgment is still involved.

Evaluators may differ in how they judge whether evidence is:

* absent,
* implicit,
* partially explicit,
* explicit,
* accessible,
* sufficient.

Future studies should include:

* independent initial ratings,
* inter-rater reliability analysis,
* evaluator training materials,
* anchor examples,
* replication exercises.

## Public Data Limitation

Industrial requirements often contain confidential project information. Therefore, full requirement text, artifact links, project identifiers, role-specific scoring records, and detailed empirical data may not be publicly released.

Future public resources may include:

* sanitized examples,
* synthetic benchmark requirements,
* simplified RP templates,
* controlled replication packages,
* public-facing scoring examples.

## No Universal Rubric

RCRE does not prescribe a single detailed rubric for all requirement types, domains, and organizations.

Reader-centricity depends on:

```text
Reader Role
Engineering Task
Required Information
Accessible Artifacts
Domain Context
```

An interface requirement, functional safety requirement, diagnostic requirement, cybersecurity requirement, and service requirement may require different information to support reader-side consumption.

The invariant part of RCRE is the construct-based logic:

```text
Define the reader role
Define the task
Define the required information
Define accessible artifacts
Collect observable evidence
Assess Role-Interrogativity, Interpretability, and Actionability
Interpret the diagnostic profile
```

What changes across domains is the Requirements Profile and the operational meaning of sufficient evidence.

## Current Claim Boundary

At this stage, RCRE should be understood as a research framework for diagnosing reader-centric requirement consumability.

The current public preview does not establish:

* a universal threshold,
* a universal defect rate,
* causal differences among organizations,
* a complete scoring standard,
* proven performance improvement after remediation.

These issues require replicated studies, calibrated thresholds, retained independent ratings, and before-after evaluations of downstream engineering tasks.

## Related Pages 
- Previous: [Discussion](discussion.md)
- Next: [Examples](examples.md)
- [Back to Home](../)
