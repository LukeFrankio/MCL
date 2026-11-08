# Compiler-toolchain example

This example shows an MCL-licensed compiler whose compiled programs embed a
small runtime library. It uses `Runtime Components` (Clause 3.7) so that
programs built with the compiler are not pulled into the compiler's reciprocity
just because the runtime is linked into them.

## Good fit

- Compilers, interpreters, bundlers, and code generators that embed runtime code
  in their output
- Language projects that want strong reciprocity for the toolchain itself but not
  for the programs people build with it

## Bad fit

- Projects whose runtime contains substantial standalone functionality they want
  to protect, since unmodified embedding is allowed under any terms
- Projects with no clean boundary between runtime code and compiler source

## Filled Annex A

```text
====================================================================
LICENSE ACTIVATION BLOCK
Modular Cooperative License v1.2.0
====================================================================

Software Name:
Quill Toolchain

Version or Release Identifier:
1.4.0

Copyright Holder(s):
Quill Language Project

Contact for Legal Notices:
legal@quill-lang.example

Primary Public Repository:
https://source.example/quill/quill

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
[x] MOD-DIST   Distribution Copyleft
[x] MOD-FILE   File-Level Reciprocity
[x] MOD-INT-A  Internal Use, Permissive Variant
[ ] MOD-INT-B  Internal Use, Reciprocal Variant
[ ] MOD-INT-C  Internal Use, Public Covered-Work Release Variant
[ ] MOD-INT-D  Internal Use, Public Integrated-System Release Variant
[ ] MOD-NET    Network and SaaS Copyleft
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
https://docs.quill-lang.example/plugin-api

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
The Quill standard runtime library in the `runtime/` directory and the
generated-code startup stubs in the `stubs/` directory, in unmodified form.

ADDITIONAL PERMISSIONS AND ALTERNATIVE LICENSES (Clause 9.3, MOD-SUB)
Steward (if MOD-SUB is active):
Not applicable because MOD-SUB is inactive.

Additional Permissions or Alternative Licenses Granted by Rights Holders:
none

ADDITIONAL PROJECT-SPECIFIC CLARIFICATIONS
Programs compiled by Quill are Output. Output that embeds the unmodified
Runtime Components above may be Distributed under terms chosen by its author,
subject to Clause 3.7. Compiler plugins that use only the documented plugin API
are intended to remain separate works unless they satisfy the Integral
Component definition.
```

## Notes

- Output (Clause 3.6) is not a Covered Work merely because the compiler generated
  it, except to the extent it contains copied or adapted protected expression,
  such as templates, stubs, or runtime code.
- The designated Runtime Components (Clause 3.7) may be embedded in Output and
  Distributed under terms of the program author's choice if the author preserves
  the required notices (Clause 4.1), the runtime remains available under MCL
  from its original source, and the Output is not a vehicle for Distributing the
  rest of the compiler or a substitute for it.
- A modified runtime component stays under MCL. Only unmodified Runtime
  Components get the exception.
- The compiler, its own source, and any plugin that is an Integral Component stay
  Covered Work. A plugin that uses only the documented API and meets the
  Separate Work tests (Clause 2.26) does not.
- This profile has no `MOD-NET`. If the project also runs a hosted playground
  that executes the compiler for third parties, add `MOD-NET` and expect the
  Clause 6.2 duties for that service.
