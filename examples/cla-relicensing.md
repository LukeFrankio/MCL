# CLA-relicensing example

This example shows a project that wants structured contributor intake and clear
future relicensing authority, but does not rely on the separate sublicensing
module.

## Good fit

- Stewarded projects with a formal contribution process
- Projects that may publish future MCL versions or named alternative licenses

## Bad fit

- Informal community projects with no CLA operations
- Single-rightsholder projects that only need direct sublicensing authority

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.0
====================================================================

Software Name:
Nimbus Toolkit

Version or Release Identifier:
1.3.0

Copyright Holder(s):
Nimbus Toolkit Project

Contact for Legal Notices:
legal@nimbustoolkit.example

Primary Public Repository:
https://git.example/nimbus/toolkit

Governing Law:
Virginia, United States

Notification Method for MOD-PUB:
[ ] Issue or pull request in the primary repository
[ ] Email or web form identified below
[ ] Other durable written method described below
Details:
Not applicable because MOD-PUB is inactive.

ACTIVATED MODULES
[ ] MOD-AI     Machine Learning Training Restriction
[ ] MOD-BIN    Cloud Binary and Deployment Release
[x] MOD-CLA    Contributor License Agreement and Relicensing
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
https://developer.nimbustoolkit.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-CLA CONFIGURATION
CLA Location:
https://nimbustoolkit.example/legal/cla

Permitted Relicensing Scope:
Future MCL versions, Apache-2.0 for selected utility subprojects, and direct
commercial licenses issued by the project steward.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Contributions are accepted only under the published CLA for releases that keep
MOD-CLA active.
```
