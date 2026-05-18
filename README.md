# Modular Cooperative License

The Modular Cooperative License, or MCL, is a modular software license
framework. In v1.1.1, it can be configured from a permissive, MIT-like floor to
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
activated, v1.1.1 is the permissive floor. Activating `MOD-FILE` restores a weak
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
| `MOD-INT-A` | Permit internal use without extra public reciprocity | Internal-use safe harbor |
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

## Compatibility notes

MCL is a custom license. It is not identical to GPL-3.0, AGPL-3.0, Apache-2.0,
or any other stewarded license.

The no-module v1.1.1 floor is the permissive end of the framework. `MOD-FILE`
adds weak reciprocity. Stronger modules can then push the license well beyond
ordinary copyleft.

The current license text includes conditional GPLv3 and AGPLv3 compatibility
bridges for qualifying activation profiles. Those bridges are unavailable when
certain blocker modules are active.

Important cautions:

- `MOD-COM` is not open source in the OSI sense
- `MOD-AI` is not open source in the OSI sense
- `MOD-SEC` is not open source in the OSI sense
- `MOD-STAGE` is not open source in the OSI sense
- profiles that activate `MOD-AI`, `MOD-BIN`, `MOD-COM`, `MOD-INT-B`,
  `MOD-INT-C`, `MOD-INT-D`, `MOD-PUB`, `MOD-SEC`, or `MOD-STAGE` do not use
  the AGPLv3 bridge
- profiles that activate `MOD-NET` do not use the GPLv3 bridge, but may still
  use the AGPLv3 bridge if no other blocker modules are active
- `MOD-CLA`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`,
  `MOD-PLUG`, and `MOD-SUB` do not by themselves disable the relevant bridge,
  except that `MOD-NET` is AGPL-only for compatibility purposes
- the compatibility section in [`MCL-LICENSE`](./MCL-LICENSE) is the governing
  text for actual use

## How to apply MCL

1. Copy [`MCL-LICENSE`](./MCL-LICENSE) into the root of your project.
2. Complete Annex A for the exact project and version you are licensing.
3. Activate only the modules you actually want.
4. Publish any additional materials required by the active modules, such as:
   - Corresponding Source
   - compliance records
   - Operational Materials
   - extension API documentation
   - contributor agreement materials
5. Add a repository-level or file-level notice identifying the applicable MCL
   version and the location of the license text.

If you want a starting point instead of a blank configuration, review the preset
profiles in Annex B and then tailor the activation block for your actual policy.
In v1.1.1, no modules gives you the permissive floor, while `MOD-FILE` gives you
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
