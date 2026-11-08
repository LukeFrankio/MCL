# Source-available non-compete example

This example shows the lightest way to protect a commercial lane: the
permissive no-module floor plus `MOD-COM`, with a `Permitted Uses` list and a
time-delayed Apache-2.0 option granted through the Additional Permissions
section. No `MOD-INT` variant is marked, so `MOD-INT-A` is deemed active
(Clause 5.5).

## Good fit

- Single-vendor projects whose main concern is a competitor reselling a hosted
  version
- Projects that want source availability and broad non-competing use without
  reciprocity obligations

## Bad fit

- Projects that want derivative works to stay open (`MOD-DIST`, `MOD-FILE`, and
  `MOD-NET` are not active)
- Projects that want to call themselves open source (`MOD-COM` is not open
  source in the OSI sense, see Clause 9.6)

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Beacon Reports

Version or Release Identifier:
5.2.0

Copyright Holder(s):
Beacon Analytics Ltd.

Contact for Legal Notices:
legal@beaconanalytics.example

Primary Public Repository:
https://source.example/beacon/reports

Governing Law:
England and Wales

Venue (optional):
Courts of England and Wales.

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
[x] MOD-COM    Commercial Non-Competing Restriction
[ ] MOD-DIST   Distribution Copyleft
[ ] MOD-FILE   File-Level Reciprocity
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
A hosted, multi-tenant business-intelligence reporting service that lets
customers build dashboards and scheduled reports from their own databases.

Permitted Uses (optional):
Self-hosted use by an organization for its own reporting, consulting and
integration work for a customer's own installation, embedding the covered work
in a product whose primary function is not hosted business-intelligence
reporting, and non-commercial research and education.

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
Beacon Analytics Ltd. additionally licenses each release of Beacon Reports
under Apache-2.0, at the recipient's option, from the date that is 24 months
after that release was first made publicly available. Until that date, only this
License applies to that release.

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Support and consulting for a customer's own installation are Permitted Uses.
Operating a hosted service for third parties that is a practical substitute for
the Primary Commercial Function is not permitted however it is described
(Clause 6.10(e)).
```

## Notes

- With no `MOD-DIST` or `MOD-FILE`, the permissive floor lets recipients keep
  their own modifications closed. `MOD-COM` restricts only substitute offerings.
- `MOD-COM` has no effect unless the Primary Commercial Function is specific
  (Clause 6.10(b)). Describe the product and its main workflow, not a market.
- The `Permitted Uses` field (Clause 6.10(g)) makes the allowed lane explicit,
  which is more predictable than relying on the practical-substitute factors
  alone.
- MCL has no built-in expiry. The time-delayed Apache-2.0 option above is an
  explicit alternative-license grant (Clause 9.3(c)), the way fair-source style
  conversion would work. It is a policy choice and not required.
- Because each copy is governed by the Annex A that accompanied it (Clause 1.4),
  carry the same grant in the Annex A of every release.
