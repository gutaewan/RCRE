---

title: FSR RP Application Preview
nav_order: 9
------------

# FSR RP Application Preview

This page provides a public preview of how Requirements Profiles (RPs) can be instantiated for Functional Safety Requirements (FSRs).

The purpose of this page is to show how RCRE can be applied to a domain-specific requirement type without disclosing industrial datasets, detailed empirical scoring records, confidential examples, or full evaluation materials.

## Public Scope

This page summarizes:

* FSR-oriented RP items,
* reader roles used for FSR consumption,
* role-specific engineering tasks,
* a role-by-RP applicability matrix,
* public-level missing-information interpretation.

This page does not provide:

* industrial FSR text,
* actual scoring records,
* empirical results,
* ECU-specific data,
* organization-specific thresholds,
* confidential artifact links,
* complete reviewer-sensitive scoring details.

## FSR Requirements Profile

An FSR Requirements Profile defines the reader-side context in which a functional safety requirement is evaluated.

```text
RP_FSR = <Reader Role, Use Context, Expected Engineering Task, Required Information, Accessible Artifacts>
```

For FSR evaluation, accessible artifacts may include:

* HARA,
* Safety Goals,
* Functional Safety Concept,
* Technical Safety Concept if available,
* Item Definition,
* E/E Architecture,
* Interface Control Documents if referenced,
* review comments,
* issue logs,
* supplier Q&A.

These artifacts are used only when they are explicitly identified and reasonably accessible to the intended reader.

## FSR RP Checklist Items

The following checklist is a public-facing summary of the FSR RP items. It is not a complete scoring rubric.

| No.   | RP Item                     | Primary Dimension | Applicable FSR Types      | Primary Roles      | Key Reader Question                                                                                         |
| ----- | --------------------------- | ----------------- | ------------------------- | ------------------ | ----------------------------------------------------------------------------------------------------------- |
| RP-01 | Safety Intent               | RI / IN           | All FSRs                  | All roles          | Can the reader recover the safety purpose this FSR serves?                                                  |
| RP-02 | Hazard or Safety Goal Link  | IN                | All FSRs                  | FSM, DE, VER       | Can the reader trace this FSR to a specific hazard or safety goal?                                          |
| RP-03 | ASIL or Safety Relevance    | IN / RI           | All FSRs                  | FSM, DE, VER       | Can the reader interpret the required safety integrity relevance and engineering implications?              |
| RP-04 | Safety Mechanism Intent     | RI / AC           | Mechanism-related FSRs    | DE, SWE, HWE, FSM  | Can the reader identify the type of safety mechanism or protective function required?                       |
| RP-05 | ECU or Role Allocation      | RI                | Allocation/interface FSRs | DE, PM, SWE, HWE   | Can the reader identify which ECU, function, or role is responsible?                                        |
| RP-06 | Interface Assumption        | RI / IN           | Interface-dependent FSRs  | DE, SWE, HWE       | Can the reader identify the signal, sender/receiver, protocol, or interface condition?                      |
| RP-07 | Fault Detection Condition   | AC                | Detection-related FSRs    | SWE, HWE, VER      | Can the reader derive the fault detection logic, trigger, threshold, or operating mode?                     |
| RP-08 | Fault Reaction Behavior     | AC                | Reaction-related FSRs     | DE, SWE, VER       | Can the reader derive the required system response when a fault is detected?                                |
| RP-09 | Safe State or Degraded Mode | AC                | Safe-state FSRs           | DE, SWE, HWE, VER  | Can the reader identify the expected safe state or degraded operation mode?                                 |
| RP-10 | Timing Constraint           | IN / AC           | Time-sensitive FSRs       | FSM, SWE, HWE, VER | Can the reader identify and interpret the timing requirement such as FTTI, FDTI, FRTI, timeout, or latency? |
| RP-11 | FTTI Rationale              | IN                | FTTI-critical FSRs        | FSM, DE, VER       | Can the reader understand why the timing constraint has the specified value?                                |
| RP-12 | Verification Implication    | AC                | Verifiable FSRs           | VER, FSM, PM       | Can the reader determine what verification objective, evidence type, or pass/fail criterion is needed?      |
| RP-13 | Responsibility Boundary     | RI                | Multi-party FSRs          | PM, DE, FSM        | Can the reader identify where responsibility boundaries begin and end?                                      |
| RP-14 | Reference Artifact          | IN                | All FSRs                  | All roles          | Are artifacts needed to recover missing information explicitly identified and accessible?                   |

## Reader Roles for FSR Consumption

The FSR RP is role-specific. Not every role is applicable to every FSR.

| Role                            | Expected Engineering Task                                                                                                          |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| DE — Design Engineer            | Derive system structure, functional allocation, interfaces, safe-state design, safety mechanism direction, and design constraints. |
| FSM — Functional Safety Manager | Review safety-goal linkage, hazard linkage, ASIL relevance, mechanism rationale, evidence expectations, and approval readiness.    |
| PM — Project Manager            | Coordinate responsibility, issue closure, supplier communication, milestone readiness, and downstream artifact ownership.          |
| VER — Verification Engineer     | Derive verification objectives, test conditions, expected outcomes, timing checks, and acceptance criteria.                        |
| SWE — Software Engineer         | Derive software safety behavior, fault-detection logic, reaction logic, state handling, and interface handling.                    |
| HWE — Hardware Engineer         | Identify hardware safety mechanisms, diagnostic assumptions, diagnostic coverage needs, and HW/SW interface implications.          |

## Role-by-RP Applicability Matrix

The following matrix shows a public-level view of which RP items are typically relevant to each reader role.

Legend:

```text
● Primary relevance
○ Secondary relevance
— Usually not applicable
```

| RP Item                        | Dim.  | DE | FSM | PM | VER | SWE | HWE |
| ------------------------------ | ----- | -: | --: | -: | --: | --: | --: |
| RP-01 Safety Intent            | RI/IN |  ● |   ● |  ● |   ● |   ● |   ● |
| RP-02 Hazard/SG Link           | IN    |  ● |   ● |  — |   ● |   ○ |   ○ |
| RP-03 ASIL Relevance           | IN/RI |  ● |   ● |  — |   ● |   ○ |   ○ |
| RP-04 Safety Mechanism         | RI/AC |  ● |   ● |  — |   ○ |   ● |   ● |
| RP-05 ECU/Role Allocation      | RI    |  ● |   ○ |  ● |   — |   ● |   ● |
| RP-06 Interface Assumption     | RI/IN |  ● |   ○ |  — |   — |   ● |   ● |
| RP-07 Fault Detection          | AC    |  ○ |   — |  — |   ● |   ● |   ● |
| RP-08 Fault Reaction           | AC    |  ● |   ○ |  — |   ● |   ● |   — |
| RP-09 Safe State               | AC    |  ● |   ○ |  — |   ● |   ● |   ● |
| RP-10 Timing Constraint        | IN/AC |  ○ |   ● |  — |   ● |   ● |   ● |
| RP-11 FTTI Rationale           | IN    |  ○ |   ● |  — |   ● |   — |   — |
| RP-12 Verification Implication | AC    |  — |   ● |  ● |   ● |   — |   — |
| RP-13 Responsibility Boundary  | RI    |  ● |   ● |  ● |   — |   — |   — |
| RP-14 Reference Artifact       | IN    |  ● |   ● |  ● |   ● |   ● |   ● |

## Missing-Information Interpretation

RCRE does not require every detail to be written inside the FSR itself.

For FSRs, some information may legitimately be:

* present in the FSR,
* recoverable through an accessible artifact,
* deferred to a downstream artifact,
* not applicable to the current reader role or task.

A public-level interpretation is as follows.

| Category                 | Meaning                                                                                   | Public Interpretation                                                           |
| ------------------------ | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| AM — Actionable Missing  | Required information is absent and not recoverable from accessible artifacts.             | Follow-up clarification may be needed.                                          |
| PM — Permissible Missing | Information is absent from the FSR but recoverable through explicit accessible artifacts. | The reference path should be clear and usable.                                  |
| DM — Deferred Missing    | Information is intentionally refined in a downstream artifact.                            | The target artifact, responsible role, or closure stage should be identifiable. |
| NM — Not Missing         | Information is sufficient for the current reader task.                                    | No missing-information follow-up is needed.                                     |

## Interpretation

This FSR RP preview demonstrates how the general RCRE measurement logic can be instantiated for a specific requirement type.

The invariant part of RCRE is:

```text
Reader Role
        ↓
Expected Task
        ↓
Required Information
        ↓
Accessible Evidence
        ↓
RI / IN / AC Diagnostic Profile
```

The domain-specific part is the RP instantiation. For FSRs, safety intent, hazard linkage, ASIL relevance, fault detection, fault reaction, safe state, timing, evidence expectations, and downstream refinement paths become important information elements.

## Public-Scope Caution

This page is a method preview. It is not a complete FSR evaluation package and should not be interpreted as a universal FSR scoring standard.

Detailed scoring examples, empirical results, industrial datasets, and confidential artifacts are intentionally withheld until the related manuscript has been submitted, reviewed, or published.

---

## Related Pages

* [Requirements Profile](requirements-profile.md)
* [Measurement Model](measurement-model.md)
* [Consensus Evaluation Procedure](consensus-evaluation-procedure.md)
* [Validity Boundaries](validity-boundaries.md)
* [Resources](resources.md)
* [Back to Home](../index.md)
