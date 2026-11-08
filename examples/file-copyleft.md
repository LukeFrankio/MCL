# File-copyleft example

This example shows the weak reciprocal layer in MCL v1.2.0. It activates
`MOD-FILE` so distributed modified files stay under MCL and their source is made
available, while the larger surrounding work does not automatically become
whole-work copyleft.

## Good fit

- Projects that want weak or file-level reciprocity
- Stewards who want something closer to MPL-style behavior than full copyleft
- Teams that liked the old v1.0 baseline and want to restore it explicitly

## Bad fit

- Projects that want the permissive no-module floor
- Projects that want full distribution copyleft or network copyleft
- Projects that want stronger commercial or internal-use restrictions
- Projects that want automatic GPL or AGPL compatibility (MCL v1.2.0 has none;
  see Clause 9.3)

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Quartz Forms

Version or Release Identifier:
1.2.0

Copyright Holder(s):
Quartz Forms Collective

Contact for Legal Notices:
legal@quartzforms.example

Primary Public Repository:
https://code.example/quartz/forms

Governing Law:
Oregon, United States

Venue (optional):
Not specified; the Clause 8.5 defaults apply.

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
[ ] MOD-DIST   Distribution Copyleft
[x] MOD-FILE   File-Level Reciprocity
[ ] MOD-INT-A  Internal Use, Permissive Variant
[ ] MOD-INT-B  Internal Use, Reciprocal Variant
[ ] MOD-INT-C  Internal Use, Public Covered-Work Release Variant
[ ] MOD-INT-D  Internal Use, Public Integrated-System Release Variant
[ ] MOD-NET    Network and SaaS Copyleft
[ ] MOD-PAT    Patent Retaliation and Enhanced Termination
[ ] MOD-PLUG   Plugin, Boundary, and Anti-Shim Enforcement
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
Not applicable because MOD-PLUG is inactive.

Integral Component Designations Beyond the Default Definition:
Not applicable because MOD-PLUG is inactive.

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
Distributed modified files remain under MCL when MOD-FILE is active, but the
surrounding larger work is not subject to whole-work copyleft by this module
alone.
```
