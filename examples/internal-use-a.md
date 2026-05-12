# Internal-use-A example

This example shows the most permissive internal-use variant. It preserves the
core public reciprocity modules while allowing internal deployment without the
extra internal-sharing or public-internal-release rules.

## Good fit

- Companies that want strong public reciprocity but ordinary internal use
- Projects that do not want to force publication of internal-only adaptations

## Bad fit

- Projects that want reciprocal access for integrated internal systems
- Projects that want public release of the internally used version

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.0
====================================================================

Software Name:
Beacon Ops

Version or Release Identifier:
3.0.0

Copyright Holder(s):
Beacon Ops Cooperative

Contact for Legal Notices:
legal@beaconops.example

Primary Public Repository:
https://git.example/beacon-ops/platform

Governing Law:
Colorado, United States

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
https://developer.beaconops.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-CLA CONFIGURATION
CLA Location:
Not applicable because MOD-CLA is inactive.

Permitted Relicensing Scope:
Not applicable because MOD-CLA is inactive.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Internal use by a parent company and wholly owned subsidiaries follows the
license definition of a single legal entity.
```
