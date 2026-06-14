# Requirements Profile
A Requirements Profile (RP) is the operational layer that connects the RCRE measurement model to a specific engineering workflow.

An RP defines:
- who consumes the requirement,
- for what engineering task,
- with what required information,
- and through which accessible artifacts.

In simple terms, an RP makes the evaluation context explicit.

## Why Requirements Profiles Are Needed
Reader-centricity is not a context-free property of a requirement sentence. The same requirement may be sufficient for one reader but insufficient for another.

For example:
- a safety manager may need safety-goal and evidence linkage,
- a software engineer may need fault-detection logic and state behavior,
- a verification engineer may need test conditions and expected outcomes,
- a supplier may need interface assumptions and allocation boundaries.

An RP prevents RCRE from becoming a generic checklist. It ensures that assessment is grounded in the actual reader role and expected task.

## RP Components
A public-level RP can be described using the following structure:

Reader Role
Use Context
Expected Engineering Task
Required Information
Accessible Artifacts

## Missing Information
RCRE does not assume that every detail must be written inside one requirement statement.

Missing information may be handled in different ways:
- it may need to be clarified immediately,
- it may be recoverable through an accessible reference,
- it may be intentionally deferred to a downstream artifact,
- or it may not be missing for the current reader task.

This distinction is important because reader-centricity is about supporting reader-side use, not about making every requirement longer.


## Related Pages 
- Previous: [Measurement Model](measurement-model.md)
- Next: [Discussion](discussion.md)
- [Back to Home](../)
