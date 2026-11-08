# GNU-alternative example

This example shows how a steward who wants GPL or AGPL compatibility under
v1.2.0 grants it explicitly for its own material. MCL v1.2.0 has no automatic
GNU bridge (Clause 9.3), so the grant is recorded in the `Additional Permissions
and Alternative Licenses` section of Annex A, and `MOD-CLA` makes sure the
foundation actually holds the rights it is granting.

## Good fit

- Foundations or single stewards that want their project usable in AGPL-licensed
  combinations
- Projects that want MCL's anti-shim and patent terms by default but accept an
  AGPL option as a deliberate trade-off

## Bad fit

- Projects with fragmented rights and no contributor agreement; the grant reaches
  only material the granting holder can license
- Projects that want the anti-shim and patent terms to survive every downstream
  choice

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Lantern Mesh

Version or Release Identifier:
3.0.0

Copyright Holder(s):
Lantern Mesh Foundation

Contact for Legal Notices:
legal@lanternmesh.example

Primary Public Repository:
https://git.example/lantern-mesh/mesh

Governing Law:
Berlin, Germany

Venue (optional):
Courts of Berlin, Germany.

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
https://docs.lanternmesh.example/extensions

Integral Component Designations Beyond the Default Definition:
None beyond the default definition.

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
https://lanternmesh.example/legal/cla

Permitted Relicensing Scope:
Future MCL versions, and AGPL-3.0-only as an alternative license for the
Covered Work, as granted in the Additional Permissions and Alternative
Licenses section below.

RUNTIME COMPONENTS (Clause 3.7)
Runtime Components:
none

ADDITIONAL PERMISSIONS AND ALTERNATIVE LICENSES (Clause 9.3, MOD-SUB)
Steward (if MOD-SUB is active):
Not applicable because MOD-SUB is inactive.

Additional Permissions or Alternative Licenses Granted by Rights Holders:
Lantern Mesh Foundation grants each recipient the option to use, modify, and
convey Lantern Mesh 3.0.0 and later versions under AGPL-3.0-only instead of
this License, as to all material for which the Foundation holds the necessary
rights, including Contributions licensed to it under the CLA.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
A recipient who exercises the AGPL-3.0-only option for a copy receives that
copy under AGPL-3.0-only alone. The Foundation chose this deliberately so that
Lantern Mesh can be combined with AGPL-licensed projects.
```

## Notes

- A recipient who does not exercise the option stays under MCL with every active
  module.
- A recipient who exercises the option takes that material under AGPL-3.0-only
  alone. The MCL module terms, including the `MOD-PLUG` Integral Component
  rules, no longer apply to that copy and its descendants. This is the downgrade
  that Clause 9.3(b) describes, accepted here on purpose.
- The grant reaches only material the granting rights holder can license
  (Clause 9.3(c)). The `MOD-CLA` configuration and Clause 3.8 are what bring
  contributions inside that set. Third-party contributions made without the CLA
  are not covered.
- `MOD-SUB` is not required. Clause 6.14(f) notes that a rights holder with
  sufficient rights may offer alternative licenses whether or not it is active.
  `MOD-SUB` would only record a steward and scope.
- Repeat the grant in the Annex A of every release it is meant to cover. Each
  copy is governed by the Annex A that accompanied it (Clause 1.4).
