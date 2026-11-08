# Modular Cooperative License

The Modular Cooperative License, or MCL, is a modular software license
framework. In v1.2.0, it can be configured from a permissive, MIT-like floor to
profiles that are more restrictive than AGPLv3. Optional modules let a
Licensor choose how aggressively the license responds to distribution,
file-level reciprocity, SaaS use, cloud binary publication, patent retaliation,
temporary security coordination, staged preview publication, internal-use
reciprocity, anti-shim behavior, commercial competition, alternative
licensing, contributor intake, and optional AI training restriction.

The canonical license text in this repository is [`MCL-LICENSE`](./MCL-LICENSE).
Annex A lets the Licensor choose the exact posture.

## What MCL is for

MCL is designed for projects that want more precision than a conventional
copyleft license usually gives them. Its text focuses on the places where modern
software businesses tend to create ambiguity, including:

- sham plugin boundaries
- hosted wrappers around reciprocal code
- cloud-only deployment artifacts
- private fork cycling
- control-plane gating
- selective publication of source without meaningful operational materials

The goal is not to absorb every adjacent system. The goal is to draw stronger,
clearer lines around the systems that are functionally part of the same covered
work.

## How MCL is structured

MCL has two layers:

- **Base Terms** in Clauses `1` through `10`
- **Optional Modules** activated in Annex A for the relevant version,
  distribution, deployment, or release

In practice, that means the same base license text can support several policy
profiles without forcing every project into the same posture. With no modules
activated, v1.2.0 is the permissive floor. Activating `MOD-FILE` restores a weak
file-level reciprocity baseline, and stronger modules push further from there.

Annex B includes example presets, but the actual legal effect always comes from
the completed activation block in Annex A.

## Module summary

| Module | Purpose | Notable effect |
|--------|---------|----------------|
| `MOD-AI` | Restrict machine learning training use | Field-of-use restriction |
| `MOD-BIN` | Require deployable cloud artifacts and operational materials | Strong cloud publication duties |
| `MOD-CLA` | Support contributor agreements and controlled relicensing | Adds contributor intake and relicensing machinery |
| `MOD-COM` | Restrict direct substitute commercial use | Field-of-use restriction |
| `MOD-DIST` | Require full reciprocal source publication on distribution | Whole-work distribution copyleft |
| `MOD-FILE` | Require modified files to stay available under MCL on distribution | Weak or file-level reciprocity |
| `MOD-INT-A` | Permit internal use without extra public reciprocity | Internal-use safe harbor; deemed active if no `MOD-INT` variant is marked |
| `MOD-INT-B` | Require internal reciprocity for integrated internal systems | Internal sharing obligation |
| `MOD-INT-C` | Require public release of the internally used covered work | Public release of internal covered-work version |
| `MOD-INT-D` | Require public release of the internally used covered work and integrated internal systems | Strongest internal-use reciprocity |
| `MOD-NET` | Trigger reciprocity for network or SaaS operation | Public source for running network version |
| `MOD-PAT` | Add patent retaliation and stronger patent-litigation termination | Optional patent-aggression response |
| `MOD-PLUG` | Police fake extension boundaries and anti-shim behavior | Strong integral-component rules |
| `MOD-PUB` | Prevent long-lived private forks | Public fork publication clock |
| `MOD-SEC` | Allow temporary private security coordination and trusted disclosure | Deferred public publication for embargoed security fixes |
| `MOD-STAGE` | Allow temporary staged preview releases and later publication | Deferred public publication for preview branches or releases |
| `MOD-SUB` | Permit a fully authorized steward to offer alternative licenses | Explicit alternative-licensing authority |

## What's new in v1.2.0

Version 1.2.0 keeps the module architecture and the purpose of every module. It
narrows overbroad definitions, fixes enforcement mechanics, and removes the
GNU compatibility bridges. In short:

- **Integral Component** (Clause 2.14) now applies to components that are
  Specific to the Covered Work, plus private-interface dependence, and it is a
  condition on a Licensee's exercise of the grant. General-purpose tools such as
  identity providers, databases, and payment processors are excluded.
- **Output and Runtime Components** (Clauses 3.6 and 3.7) say that generated
  Output is not a Covered Work, with a designated-runtime exception for
  compilers and similar tools.
- **Termination** (Clause 8.2) has provisional and permanent reinstatement, a
  good-faith classification path, and protection for downstream recipients.
- **Private and internal use** modules gain a personal-use carve-out, and the
  open-source status of every module is stated in Clause 9.6.
- **Contributions** are licensed inbound=outbound (Clause 3.8), and the patent
  grant now covers the original release (Clause 3.2).
- **No GNU bridge**; see the compatibility notes above.

See [`CHANGELOG.md`](./CHANGELOG.md) for the full list.

## Compatibility notes

MCL is a custom license. It is not identical to GPL-3.0, AGPL-3.0, Apache-2.0,
or any other stewarded license, and it is not approved by the OSI or endorsed
by the FSF.

The no-module v1.2.0 floor is the permissive end of the framework. `MOD-FILE`
adds weak reciprocity. Stronger modules can then push the license well beyond
ordinary copyleft.

**There is no GPL or AGPL compatibility bridge in v1.2.0.** Versions 1.1.x
contained conditional GPLv3 and AGPLv3 bridges for qualifying profiles. They
were removed because they could not be made safe: a permission to convey
MCL-covered portions under GNU terms lets a recipient add a single GNU-licensed
file and shed the reciprocity, anti-shim, and patent terms of the active
modules for that copy and its descendants. Copies received under 1.1.x keep the
bridge that accompanied them.

A rights holder who wants GNU compatibility, or any other alternative license,
for its own material can grant it explicitly in the new "Additional Permissions
and Alternative Licenses" section of Annex A (Clause 9.3). That is a deliberate,
scoped, recorded choice, not an automatic property of the license.

Open-source status (Clause 9.6):

- `MOD-AI`, `MOD-COM`, `MOD-PUB`, `MOD-SEC`, `MOD-STAGE`, `MOD-INT-B`,
  `MOD-INT-C`, and `MOD-INT-D` are not open source in the OSI sense. They add a
  field-of-use restriction, a delayed-publication exception, or a condition on
  private or internal use
- `MOD-BIN` and `MOD-PLUG` impose obligations beyond conventional network
  copyleft, and reviewers may not treat them as open source
- no claim is made that any other combination of modules satisfies the Open
  Source Definition, and none has been reviewed
- a Licensor should not describe a profile as open source if it activates any
  module named above
- the compatibility and status clauses in [`MCL-LICENSE`](./MCL-LICENSE)
  (Clauses 9.2, 9.3, and 9.6) are the governing text for actual use

## How to apply MCL

1. Copy [`MCL-LICENSE`](./MCL-LICENSE) into the root of your project.
2. Complete Annex A for the exact project and version you are licensing,
   including the Venue, Runtime Components, and Additional Permissions fields
   where they matter for your project.
3. Activate only the modules you actually want.
4. Publish any additional materials required by the active modules, such as:
   - Corresponding Source
   - compliance records
   - Operational Materials
   - extension API documentation
   - contributor agreement materials
5. Add a repository-level or file-level notice identifying the applicable MCL
   version, the active modules (the machine-readable `MCL-Modules:` line from
   Annex D), and the location of the license text. If you use a preset, you can
   refer to it as `LicenseRef-MCL-1.2.0-<PRESET>`, for example
   `LicenseRef-MCL-1.2.0-COMMUNITY`.

If you want a starting point instead of a blank configuration, review the preset
profiles in Annex B and then tailor the activation block for your actual policy.
In v1.2.0, no modules gives you the permissive floor, while `MOD-FILE` gives you
the weak file-level copyleft layer that older MCL drafts treated as the
baseline.
If you want concrete filled-out activation blocks, start from the examples in
[`examples/`](./examples/).

## Repository contents

- [`CHANGELOG.md`](./CHANGELOG.md) — repository-level change history
- [`CONTRIBUTING.md`](./CONTRIBUTING.md) — contribution and discussion guidance
- [`MCL-LICENSE`](./MCL-LICENSE) — canonical license text
- [`examples/`](./examples/) — filled-out Annex A examples for common policy
  postures

## Legal note

This repository publishes license text and supporting documentation. It does not
provide legal advice. If you plan to deploy MCL for real software or high-value
intellectual property, you should have the text reviewed by qualified counsel in
relevant jurisdictions.
