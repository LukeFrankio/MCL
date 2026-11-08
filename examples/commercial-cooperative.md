# Commercial-cooperative example

This example shows the strongest commercial posture in the current repository:
strong reciprocity plus a non-competing restriction, steward alternative
licensing authority, and CLA infrastructure.

## Good fit

- Stewarded projects that want reciprocity and a protected commercial lane
- Projects with a planned dual-licensing or commercial licensing program

## Bad fit

- Community projects seeking OSI-style norms
- Projects that want automatic GPL or AGPL compatibility (MCL v1.2.0 has none;
  see Clause 9.3)

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Northwind Boards

Version or Release Identifier:
5.1.0

Copyright Holder(s):
Northwind Boards, Inc.

Contact for Legal Notices:
legal@northwindboards.example

Primary Public Repository:
https://code.example/northwind/boards

Governing Law:
Texas, United States

Venue (optional):
Not specified; the Clause 8.5 defaults apply.

Notification Method for MOD-PUB:
[ ] Issue or pull request in the primary repository
[x] Email or web form identified below
[ ] Other durable written method described below
Details:
Use the publication notice form at https://northwindboards.example/legal/pub.

ACTIVATED MODULES
[ ] MOD-AI     Machine Learning Training Restriction
[x] MOD-BIN    Cloud Binary and Deployment Release
[x] MOD-CLA    Contributor License Agreement and Relicensing
[x] MOD-COM    Commercial Non-Competing Restriction
[x] MOD-DIST   Distribution Copyleft
[x] MOD-FILE   File-Level Reciprocity
[x] MOD-INT-A  Internal Use, Permissive Variant
[ ] MOD-INT-B  Internal Use, Reciprocal Variant
[ ] MOD-INT-C  Internal Use, Public Covered-Work Release Variant
[ ] MOD-INT-D  Internal Use, Public Integrated-System Release Variant
[x] MOD-NET    Network and SaaS Copyleft
[x] MOD-PAT    Patent Retaliation and Enhanced Termination
[x] MOD-PLUG   Plugin, Boundary, and Anti-Shim Enforcement
[x] MOD-PUB    Public Fork Requirement
[ ] MOD-SEC    Security Embargo and Trusted Disclosure
[ ] MOD-STAGE  Staged Preview and Deferred Publication
[x] MOD-SUB    Steward Alternative Licensing Authority

MOD-COM CONFIGURATION
Primary Commercial Function:
A hosted multi-tenant project-planning and kanban service for enterprise teams.

Permitted Uses (optional):
Self-hosted deployment by an organization for its own projects, and use of
the covered work as a component of a product that does not replicate the hosted
planning service.

MOD-PLUG CONFIGURATION
Documented Extension API Location:
https://developer.northwindboards.example/extensions

Integral Component Designations Beyond the Default Definition:
The hosted entitlement gateway and policy engine are designated Integral
Components for public SaaS releases.

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
https://northwindboards.example/legal/cla

Permitted Relicensing Scope:
Future MCL versions and commercial licenses issued directly by Northwind Boards,
Inc.

RUNTIME COMPONENTS (Clause 3.7)
Runtime Components:
none

ADDITIONAL PERMISSIONS AND ALTERNATIVE LICENSES (Clause 9.3, MOD-SUB)
Steward (if MOD-SUB is active):
Northwind Boards, Inc.

Additional Permissions or Alternative Licenses Granted by Rights Holders:
Separate commercial licenses issued directly by Northwind Boards, Inc. for
material to which it holds the necessary rights. No GPL or AGPL alternative is
granted.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Support and managed-service offerings are not exempt from MOD-COM if they are
practical substitutes for the identified hosted service.
```
