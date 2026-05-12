# AI-restricted example

This example shows a reciprocal network profile that also activates `MOD-AI` to
restrict machine learning training or tuning use without separate permission.

## Good fit

- Projects that want strong reciprocity and an explicit anti-training policy
- Codebases whose steward wants to allow ordinary use but not model training

## Bad fit

- Projects seeking open-source compatibility norms
- Projects that want GPL or AGPL compatibility paths

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.0
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
[x] MOD-INT-A  Internal Use, Permissive Variant
[ ] MOD-INT-B  Internal Use, Reciprocal Variant
[ ] MOD-INT-C  Internal Use, Public Covered-Work Release Variant
[ ] MOD-INT-D  Internal Use, Public Integrated-System Release Variant
[x] MOD-NET    Network and SaaS Copyleft
[x] MOD-PLUG   Plugin, Boundary, and Anti-Shim Enforcement
[ ] MOD-PUB    Public Fork Requirement
[ ] MOD-SUB    Sublicensing Permission

MOD-COM CONFIGURATION
Primary Commercial Function:
Not applicable because MOD-COM is inactive.

MOD-PLUG CONFIGURATION
Documented Extension API Location:
https://developer.pinecompiler.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-CLA CONFIGURATION
CLA Location:
Not applicable because MOD-CLA is inactive.

Permitted Relicensing Scope:
Not applicable because MOD-CLA is inactive.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Machine learning training or tuning use requires separate written permission
from the project steward when MOD-AI is active.
```
