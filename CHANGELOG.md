# Changelog

This changelog tracks repository changes separately from changes to the license
text itself.

Unless an entry says otherwise, the canonical license remains **Modular
Cooperative License Version 1.1.1**.

## 2026-05-17 — v1.1.1 stress-test hardening

This entry records the follow-up drafting fixes and version bump after a second,
more aggressive stress test of the v1.1 text.

### Repository updates

- Updated `README.md` to explain the split between the GPLv3 bridge and the
  AGPLv3 bridge more precisely.
- Updated `README.md` and the example set to reflect **Version 1.1.1**.

### License updates

- Bumped the working text from **MCL Version 1.1** to **MCL Version 1.1.1**.
- Split Clause `9.2` and Clause `9.3` so `MOD-NET` can follow the AGPLv3
  compatibility path without creating a GPLv3 washing loophole.
- Clarified that `MOD-SEC` timing controls over the `MOD-NET` 72-hour emergency
  publication rule for qualifying embargoed security changes.
- Added a narrow safe harbor in `MOD-PUB` for private experimental forks that
  are never distributed, never exposed to third parties, never used in
  production, and are discarded promptly.
- Clarified that `MOD-AI` does not by itself prohibit ordinary interactive
  development-tool use unless the licensee separately opts into or requests
  model-improvement use of the covered work.
- Clarified that `Operational Materials` and `MOD-BIN` need structural
  reproducibility, not disclosure of account-specific or provider-assigned
  cloud identifiers.
- Clarified that `MOD-BIN` does not by itself erase the operative scope of an
  active internal-use module for internal cloud deployments.
- Clarified in the General-Purpose Tool safe harbor that ordinary configuration
  alone does not automatically make a gateway or similar tool an Integral
  Component.
- Clarified that large client-side compiled logic, including WebAssembly, is
  not automatically treated as Static Disconnected Work Product.
- Clarified that deliberate dilution of Unified Product factors does not by
  itself defeat Unified Product status.
- Clarified that the affiliate or common-control shell-company pattern does not
  defeat `MOD-PAT`.
- Clarified that `MOD-PUB` does not force publication of strictly internal-only
  forks while `MOD-INT-A` or `MOD-INT-B` still applies, and aligned the preset
  descriptions with that internal-use safe harbor.
- Clarified that cure and reinstatement do not extinguish historical monetary
  remedies for pre-cure breach.
- Clarified that `MOD-AI` does not treat ordinary debugging and analysis as
  training use, but does reach repeated generative-template or RAG-style source
  ingestion aimed at producing a substitute implementation.
- Added a reasonable-efforts direct-notice requirement before relying on
  contributor silence under `MOD-CLA` relicensing notice procedures.

## 2026-05-16 — v1.1 permissive-floor redesign

This entry records the architectural redesign that makes the standard MCL
framework itself span from a permissive floor to much more restrictive custom
profiles.

### Repository updates

- Updated `README.md` to describe the v1.1 range from permissive floor to
  strong custom restriction.
- Updated `examples/README.md` to distinguish the permissive floor from the new
  file-level reciprocity example.
- Updated `examples/core-only.md` to reflect the permissive no-module floor.
- Updated example files to the v1.1 activation block format.
- Added `examples/file-copyleft.md`.

### License updates

- Bumped the working text from **MCL Version 1.0** to **MCL Version 1.1**.
- Recast MCL from an always-reciprocal framework into a modular framework with
  permissive base terms.
- Moved the weak reciprocal baseline out of the always-on base and into the new
  `MOD-FILE` module.
- Made patent retaliation optional through the new `MOD-PAT` module.
- Refactored `MOD-SUB` into a steward alternative-licensing authority module.
- Clarified that `MOD-CLA` and `MOD-SUB` do not by themselves disable the
  GPLv3 or AGPLv3 compatibility bridge.
- Clarified that `MOD-SEC` and `MOD-STAGE` authorize only temporal disclosure
  or publication deferrals, not structural separateness arguments.
- Updated Annex A, Annex B, SPDX guidance, and the suggested source notice for
  Version 1.1.

## 2026-05-16 — Staged disclosure modules

At the time of this change, the repository still tracked **MCL Version 1.0**.
That staged-disclosure work is now incorporated into the Version 1.1 working
text.

### Repository updates

- Updated `README.md` to document `MOD-SEC` and `MOD-STAGE`.
- Updated `examples/README.md` to index the staged-disclosure examples.
- Added `examples/security-embargo.md`.
- Added `examples/staged-preview.md`.
- Recorded the staged-disclosure expansion in this changelog.

### License updates

- Added the definitions `Embargoed Security Change`, `Staged Preview Release`,
  and `Trusted Actor`.
- Added `MOD-SEC` for temporary private security coordination and trusted
  defensive disclosure.
- Added `MOD-STAGE` for temporary staged preview releases and deferred public
  publication.
- Added framework rules, evidentiary burdens, Annex A configuration fields, and
  compatibility-blocker updates for the new modules.

## 2026-05-12 — Examples update

The repository remains on **MCL Version 1.0**. This entry adds supporting
materials and does not create a new license version.

### Repository updates

- Added `CHANGELOG.md`.
- Added `CONTRIBUTING.md`.
- Added the `examples/` folder.
- Added `examples/README.md` as an index for the example set.
- Added filled-out Annex A examples for core-only, community-network,
  strong-cloud, commercial-cooperative, internal-use variants A through D,
  AI-restricted use, sublicensing, and CLA/relicensing.
- Updated the root `README.md` to point readers to the new examples.

### License updates

- No license-version change.
- The canonical license text remains **MCL Version 1.0**.

## 2026-05-11 — Initial release

This entry records the first publication of the repository and the initial
public release of the license text.

### Repository updates

- Published the repository with the canonical `MCL-LICENSE` text.
- Added the root `README.md`.

### License updates

- Published the initial **Modular Cooperative License Version 1.0** text.
- Published the core terms, optional modules, and annexes that define the
  Version 1.0 specification.
