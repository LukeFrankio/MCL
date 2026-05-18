# Staged-preview example

This example shows a project that wants reciprocal publication but also wants a
bounded preview workflow for alpha, beta, nightly, or canary releases before the
full source publication catches up.

## Good fit

- Projects with public preview or nightly channels
- Teams that want to stage incomplete features before upstream publication
- Stewards who want eventual publication on a clear time or release trigger

## Bad fit

- Projects seeking immediate source publication for every preview artifact
- Teams that want a permanent private development line
- Projects that do not need any preview cadence beyond normal public releases

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.1.1
====================================================================

Software Name:
Nimbus Console

Version or Release Identifier:
3.4.0-preview

Copyright Holder(s):
Nimbus Console Project

Contact for Legal Notices:
legal@nimbusconsole.example

Primary Public Repository:
https://git.example/nimbus/console

Governing Law:
Washington, United States

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
[x] MOD-STAGE  Staged Preview and Deferred Publication
[ ] MOD-SUB    Steward Alternative Licensing Authority

MOD-COM CONFIGURATION
Primary Commercial Function:
Not applicable because MOD-COM is inactive.

MOD-PLUG CONFIGURATION
Documented Extension API Location:
https://developer.nimbusconsole.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-SEC CONFIGURATION
Trusted Actor Categories:
Not applicable because MOD-SEC is inactive.

Maximum Embargo Window:
Not applicable because MOD-SEC is inactive.

Security Publication Trigger:
Not applicable because MOD-SEC is inactive.

Permitted Non-Public Materials:
Not applicable because MOD-SEC is inactive.

MOD-STAGE CONFIGURATION
Permitted Preview Channels or Recipients:
Employees, design partners, authenticated nightly users, and public beta users
when a release is clearly labeled as preview.

Maximum Staging Window:
45 days.

Staged Publication Trigger:
The earliest of public beta release, general availability, or expiration of the
45-day staging window.

Abandoned Preview Rule:
A staged branch that never leaves the permitted preview channels may be
discarded privately if it is abandoned before general release.

MOD-CLA CONFIGURATION
CLA Location:
Not applicable because MOD-CLA is inactive.

Permitted Relicensing Scope:
Not applicable because MOD-CLA is inactive.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
All public preview builds must be labeled as preview or beta releases while
MOD-STAGE is being used to defer full public source publication.
```
