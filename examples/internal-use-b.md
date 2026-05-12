# Internal-use-B example

This example shows the reciprocal internal-use variant. It keeps the same public
reciprocity baseline as the A profile, but requires access for materially
integrated internal systems.

## Good fit

- Projects that want internal reciprocity without forcing public release
- Platforms where integrated internal extensions should be shared with the teams
  that rely on them

## Bad fit

- Organizations that want fully private internal integrations
- Projects that want public release of the exact internally used version

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.0
====================================================================

Software Name:
Meridian Planner

Version or Release Identifier:
2.7.3

Copyright Holder(s):
Meridian Planner, LLC

Contact for Legal Notices:
legal@meridianplanner.example

Primary Public Repository:
https://source.example/meridian/planner

Governing Law:
Illinois, United States

Notification Method for MOD-PUB:
[ ] Issue or pull request in the primary repository
[ ] Email or web form identified below
[ ] Other durable written method described below
Details:
Not applicable because MOD-PUB is inactive.

ACTIVATED MODULES
[ ] MOD-AI     Machine Learning Training Restriction
[ ] MOD-BIN    Cloud Binary and Deployment Release
[ ] MOD-CLA    Contributor License Agreement and Relicensing
[ ] MOD-COM    Commercial Non-Competing Restriction
[x] MOD-DIST   Distribution Copyleft
[ ] MOD-INT-A  Internal Use, Permissive Variant
[x] MOD-INT-B  Internal Use, Reciprocal Variant
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
https://developer.meridianplanner.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-CLA CONFIGURATION
CLA Location:
Not applicable because MOD-CLA is inactive.

Permitted Relicensing Scope:
Not applicable because MOD-CLA is inactive.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Integrated internal workflow modules are expected to be available to the teams
that use or maintain them when MOD-INT-B is active.
```
