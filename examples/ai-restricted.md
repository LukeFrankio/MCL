# AI-restricted example

This example shows a reciprocal network profile that also activates `MOD-AI` to
restrict machine learning training or tuning use without separate permission.

## Good fit

- Projects that want strong reciprocity and an explicit anti-training policy
- Codebases whose steward wants to allow ordinary use but not model training

## Bad fit

- Projects seeking open-source compatibility norms
- Projects that want automatic GPL or AGPL compatibility (MCL v1.2.0 has none;
  see Clause 9.3)

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Pine Compiler

Version or Release Identifier:
0.9.0

Copyright Holder(s):
Pine Compiler Project

Contact for Legal Notices:
licensing@pinecompiler.example

Primary Public Repository:
https://code.example/pine-compiler/pine

Governing Law:
Massachusetts, United States

Venue (optional):
Not specified; the Clause 8.5 defaults apply.

Notification Method for MOD-PUB:
[ ] Issue or pull request in the primary repository
[ ] Email or web form identified below
[ ] Other durable written method described below
Details:
Not applicable because MOD-PUB is inactive.

ACTIVATED MODULES
[x] MOD-AI     Machine Learning Training Restriction
[ ] MOD-BIN    Cloud Binary and Deployment Release
[ ] MOD-CLA    Contributor License Agreement and Relicensing
[ ] MOD-COM    Commercial Non-Competing Restriction
[x] MOD-DIST   Distribution Copyleft
[x] MOD-FILE   File-Level Reciprocity
[x] MOD-INT-A  Internal Use, Permissive Variant
[ ] MOD-INT-B  Internal Use, Reciprocal Variant
[ ] MOD-INT-C  Internal Use, Public Covered-Work Release Variant
[ ] MOD-INT-D  Internal Use, Public Integrated-System Release Variant
[x] MOD-NET    Network and SaaS Copyleft
[x] MOD-PAT    Patent Retaliation and Enhanced Termination
[x] MOD-PLUG   Plugin, Boundary, and Anti-Shim Enforcement
[ ] MOD-PUB    Public Fork Requirement
[ ] MOD-SEC    Security Embargo and Trusted Disclosure
[ ] MOD-STAGE  Staged Preview and Deferred Publication
[ ] MOD-SUB    Steward Alternative Licensing Authority

MOD-COM CONFIGURATION
Primary Commercial Function:
Not applicable because MOD-COM is inactive.

Permitted Uses (optional):
Not applicable because MOD-COM is inactive.

MOD-PLUG CONFIGURATION
Documented Extension API Location:
https://developer.pinecompiler.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-SEC CONFIGURATION
(Blank fields take the defaults in Clause 5.8.)
Trusted Actor Categories:
Not applicable because MOD-SEC is inactive.

Maximum Embargo Window:
Not applicable because MOD-SEC is inactive.

Security Publication Trigger:
Not applicable because MOD-SEC is inactive.

Permitted Non-Public Materials:
Not applicable because MOD-SEC is inactive.

MOD-STAGE CONFIGURATION
(Blank fields take the defaults in Clause 5.8.)
Permitted Preview Channels or Recipients:
Not applicable because MOD-STAGE is inactive.

Maximum Staging Window:
Not applicable because MOD-STAGE is inactive.

Staged Publication Trigger:
Not applicable because MOD-STAGE is inactive.

Abandoned Preview Rule:
Not applicable because MOD-STAGE is inactive.

MOD-CLA CONFIGURATION
CLA Location:
Not applicable because MOD-CLA is inactive.

Permitted Relicensing Scope:
Not applicable because MOD-CLA is inactive.

RUNTIME COMPONENTS (Clause 3.7)
Runtime Components:
none

ADDITIONAL PERMISSIONS AND ALTERNATIVE LICENSES (Clause 9.3, MOD-SUB)
Steward (if MOD-SUB is active):
Not applicable because MOD-SUB is inactive.

Additional Permissions or Alternative Licenses Granted by Rights Holders:
none

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Machine learning training or tuning use requires separate written permission
from the project steward when MOD-AI is active.
```
