# Security-embargo example

This example shows a project that wants strong reciprocal publication duties,
but also wants a controlled security-embargo workflow so trusted maintainers or
operators can receive patches before the full source disclosure becomes public.

## Good fit

- Security-sensitive infrastructure projects
- Projects whose downstream maintainers need early defensive access
- Stewards who want public publication after a bounded embargo window

## Bad fit

- Projects seeking ordinary OSI-style open-source timing
- Teams that want permanent private security branches
- Projects without a real trusted-recipient workflow

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.1.1
====================================================================

Software Name:
Iron Gate Proxy

Version or Release Identifier:
7.2.0

Copyright Holder(s):
Iron Gate Systems, Inc.

Contact for Legal Notices:
legal@irongateproxy.example

Primary Public Repository:
https://code.example/iron-gate/proxy

Governing Law:
Virginia, United States

Notification Method for MOD-PUB:
[ ] Issue or pull request in the primary repository
[x] Email or web form identified below
[ ] Other durable written method described below
Details:
Use security-notices@irongateproxy.example for MOD-PUB and coordinated security
release notices.

ACTIVATED MODULES
[ ] MOD-AI     Machine Learning Training Restriction
[x] MOD-BIN    Cloud Binary and Deployment Release
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
[x] MOD-PUB    Public Fork Requirement
[x] MOD-SEC    Security Embargo and Trusted Disclosure
[ ] MOD-STAGE  Staged Preview and Deferred Publication
[ ] MOD-SUB    Steward Alternative Licensing Authority

MOD-COM CONFIGURATION
Primary Commercial Function:
Not applicable because MOD-COM is inactive.

MOD-PLUG CONFIGURATION
Documented Extension API Location:
https://developer.irongateproxy.example/extensions

Integral Component Designations Beyond the Default Definition:
See INTEGRAL_COMPONENTS.md

MOD-SEC CONFIGURATION
Trusted Actor Categories:
Downstream Linux distribution maintainers, managed service operators, and
contracted incident-response partners under written security coordination terms.

Maximum Embargo Window:
14 days.

Security Publication Trigger:
The earliest of full public release of the patched version, 80 percent rollout
of the hosted fix, or expiration of the 14-day embargo window.

Permitted Non-Public Materials:
Source patches, patched binaries, mitigation instructions, deployment notes, and
non-secret operational materials reasonably necessary for defensive rollout.

MOD-STAGE CONFIGURATION
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

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
MOD-SEC is intended only for defensive patch coordination and may not be used to
withhold ordinary product features or roadmap work.
```
