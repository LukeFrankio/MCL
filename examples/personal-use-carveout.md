# Personal-use carve-out example

This example shows strong organizational transparency with individual-friendly
edges. `MOD-INT-C` requires organizations to publish the exact version they use
internally, and `MOD-PUB` requires private forks to go public, while both
modules carve out personal, non-commercial use by natural persons.

## Good fit

- Public-benefit and civic software where organizations should publish what they
  run but hobbyists should not be burdened
- Projects that want private fork cycling closed off for organizations only

## Bad fit

- Projects that want organizations to be able to use the software internally
  without publishing (use `MOD-INT-A` instead)
- Projects that want to call themselves open source (`MOD-INT-C` and `MOD-PUB`
  are not open source in the OSI sense, see Clause 9.6)

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Commons Ledger

Version or Release Identifier:
2.0.0

Copyright Holder(s):
Commons Ledger Association

Contact for Legal Notices:
legal@commonsledger.example

Primary Public Repository:
https://git.example/commons-ledger/ledger

Governing Law:
Ontario, Canada

Venue (optional):
Not specified; the Clause 8.5 defaults apply.

Notification Method for MOD-PUB:
[x] Issue or pull request in the primary repository
[ ] Email or web form identified below
[ ] Other durable written method described below
Details:
Open an issue in the primary repository using the Fork Notice template.

ACTIVATED MODULES
[ ] MOD-AI     Machine Learning Training Restriction
[ ] MOD-BIN    Cloud Binary and Deployment Release
[ ] MOD-CLA    Contributor License Agreement and Relicensing
[ ] MOD-COM    Commercial Non-Competing Restriction
[x] MOD-DIST   Distribution Copyleft
[x] MOD-FILE   File-Level Reciprocity
[ ] MOD-INT-A  Internal Use, Permissive Variant
[ ] MOD-INT-B  Internal Use, Reciprocal Variant
[x] MOD-INT-C  Internal Use, Public Covered-Work Release Variant
[ ] MOD-INT-D  Internal Use, Public Integrated-System Release Variant
[x] MOD-NET    Network and SaaS Copyleft
[x] MOD-PAT    Patent Retaliation and Enhanced Termination
[x] MOD-PLUG   Plugin, Boundary, and Anti-Shim Enforcement
[x] MOD-PUB    Public Fork Requirement
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
https://docs.commonsledger.example/extensions

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
Individuals using or forking Commons Ledger for personal, non-commercial
purposes, with no third-party access, are within the personal-use carve-outs of
MOD-INT-C and MOD-PUB.
```

## Notes

- `MOD-INT-C` (Clause 6.8) requires public release of the exact internally used
  version within 30 days of first internal operation. Clause 6.8(e) exempts a
  natural person's personal, non-commercial use with no third-party access.
- `MOD-PUB` (Clause 6.4) starts a 90-day clock for private forks. Clause 6.4(j)
  exempts a fork kept by a natural person for personal, non-commercial use that
  is never Distributed, never offered for Network Use, and not used in
  production by or for any legal entity. The 90 days start on the date those
  conditions stop being true.
- Internal Use (Clause 2.15) now covers a natural person and, for a person,
  members of the person's household, plus rented cloud infrastructure where the
  provider acts only as a provider.
- The carve-outs do not reach employees acting for a company or any use that
  gives a third party access. Those still trigger the module obligations.
