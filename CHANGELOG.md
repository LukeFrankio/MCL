# Changelog

This changelog tracks repository changes separately from changes to the license
text itself.

Unless an entry says otherwise, the canonical license remains **Modular
Cooperative License Version 1.2.0**.

## 2026-11-08 — v1.2.0 critique-driven rework

This entry records a rework of v1.1.1 following a clause-by-clause critique of
the full text. The module architecture and the purpose of every module are
unchanged. The changes narrow overbroad definitions, fix enforcement mechanics,
close drafting gaps, and remove the GPLv3 and AGPLv3 compatibility bridges.

### Repository updates

- Replaced `MCL-LICENSE` with **Version 1.2.0**.
- Updated `README.md`: moved to v1.2.0, rewrote the compatibility notes (no
  GNU bridge, open-source status per Clause 9.6), added a "What's new in v1.2.0"
  section, updated the `MOD-INT-A` row, and updated the how-to-apply steps for
  the new Annex A fields and the machine-readable `MCL-Modules:` line.
- Updated `examples/README.md`: moved to v1.2.0 and added notes on the new Annex
  A fields, the removal of GNU compatibility, open-source status per example,
  and the deemed `MOD-INT-A` default.
- Updated all 14 example Annex A blocks to the v1.2.0 template: version header,
  `Venue`, `Permitted Uses` for `MOD-COM`, the Clause 5.8 defaults note under
  `MOD-SEC` and `MOD-STAGE`, `Runtime Components`, and `Additional Permissions
  and Alternative Licenses`. Filled the steward and alternative-license fields
  for `sublicensing.md` and `commercial-cooperative.md`, and the `Permitted
  Uses` field for `commercial-cooperative.md`.
- Replaced the "GPL or AGPL compatibility paths" good-fit and bad-fit wording in
  the examples that previously qualified for a bridge.
- Added five examples for v1.2.0 features: `examples/gnu-alternative.md` (an
  explicit AGPL option through Additional Permissions, with `MOD-CLA`),
  `examples/compiler-toolchain.md` (Output and Runtime Components),
  `examples/source-available-noncompete.md` (`MOD-COM` on the permissive floor,
  `Permitted Uses`, and a delayed Apache-2.0 option),
  `examples/personal-use-carveout.md` (`MOD-INT-C` and `MOD-PUB` with the
  personal-use carve-outs), and `examples/compliance-and-notices.md` (Annex D
  notices and Annex C Compliance Records, including Clause 6.2(h)).
- Added the new examples to the `examples/README.md` index and open-source
  status notes.

### License updates

**GNU compatibility**

- Removed the automatic GPLv3 and AGPLv3 bridges. Clause 9.3 is now "No
  Automatic GNU Compatibility; Licensor-Granted Additional Permissions", and
  Clause 9.2 no longer claims compatibility with any GNU-family license. The
  bridge could not be made non-downgrading, because adding one GNU-licensed file
  would let a recipient shed the module terms for that copy and its descendants.
  Copies received under 1.1.x keep the bridge that accompanied them (Clause 1.4).
- Added the Annex A section "Additional Permissions and Alternative Licenses"
  so a rights holder can grant GNU compatibility, or any other alternative
  license, for its own material as a deliberate, recorded choice. `MOD-SUB` now
  names its steward there and is declaratory.

**Integral Component and related definitions**

- Rewrote Clause 2.14. A component is an Integral Component if it is Specific to
  the Covered Work and satisfies a control, mediation, core-function, or Unified
  Product criterion (F1 to F4), or if it depends on private interfaces (F5). An
  independent reimplementation that copies nothing does not satisfy F5.
- Excluded general-purpose tools, including general-purpose identity providers
  and payment processors, and Static Disconnected Work Product from Clause 2.14.
- Made Clause 2.14 operate only as a condition on a Licensee's exercise of the
  grant, not as a claim that a component is a Derivative Work.
- Raised the Unified Product threshold in Clause 2.31 and added a note that a
  shared vendor or hosting environment does not by itself create one.
- Removed the circular "combined with it to the extent licensed" wording from
  Clause 2.7. Clarified Separate Work as the way to rebut an Integral Component
  presumption (Clauses 2.26, 7.2, 7.3).
- Made `MOD-PLUG` designations a rebuttable presumption that cannot reach
  general-purpose tools or components that are not Specific to the Covered Work
  (Clause 6.5(b)).
- Replaced intent-based tests with effect-plus-no-independent-justification
  tests in Clauses 4.6 and 7.6, and made the `MOD-COM` presumption count factors
  (i) through (iv) only (Clauses 6.10(c), 7.9).

**Output and compilers**

- Added Clause 3.6 (Output is not a Covered Work) and Clause 3.7 (Runtime
  Components exception designated in Annex A). Updated Clause 2.29 accordingly.

**Termination, contributions, and plumbing**

- Rewrote Clause 8.1 and Clause 8.2 with provisional and permanent
  reinstatement, a 30-day cure from notice, a good-faith classification path,
  and preserved liability for pre-cure breach.
- Protected downstream recipients when a Licensee's rights terminate (Clause
  3.4).
- Added the original release and Contributors to the patent grant (Clauses 2.4,
  2.5, 3.2) and added inbound=outbound contribution licensing (Clause 3.8).
- Clarified that the grants are conditioned on compliance (Clause 1.10) and what
  happens when Annex A is missing or unclear (Clause 1.9).
- Defined Licensee and User (Clauses 2.33 and 2.34), and made `MOD-INT-A` deemed
  active when no `MOD-INT` variant is marked (Clause 5.5).
- Added defaults for blank `MOD-SEC` and `MOD-STAGE` fields (Clause 5.8).
- Added a Venue field and a governing-law default that works with multiple
  Licensors (Clause 8.5), and a duty to substantiate exemption claims on request
  (Clause 4.7).
- Reserved Clauses 4.4 and 4.5 and cleaned up stacked "and" connectors in Clauses
  6.1, 6.3, 6.4, 6.7 through 6.11, and Annex C.

**Modules**

- `MOD-NET`: added a lightweight path for unmodified upstream operation (Clause
  6.2(h)) and a matching retention rule (Clause 7.7).
- `MOD-BIN`: clarified that private mirrors serving digest-identified public
  content are not non-public, that bit-for-bit reproducibility is not required,
  and replaced "material breach" with a plain failure-to-satisfy statement
  (Clause 6.3).
- `MOD-PUB`, `MOD-INT-C`, and `MOD-INT-D`: added a personal-use carve-out for
  natural persons (Clauses 6.4(j), 6.8(e), 6.9(e)) and extended Internal Use to
  natural persons and rented infrastructure (Clause 2.15).
- `MOD-AI`: added an express reservation of rights, a machine-readable
  reservation recommendation, and a statement that the module does not override
  statutory exceptions that cannot be limited by contract (Clause 6.11).
- `MOD-COM`: added a `Permitted Uses` list in Annex A (Clause 6.10(g)).
- `MOD-CLA`: made the Licensor's obligations enforceable by Contributors as
  third-party beneficiaries to the extent permitted by law (Clause 6.15(h)).

**Open-source status and metadata**

- Added Clause 9.6 stating which modules are not open source in the OSI sense
  (`MOD-AI`, `MOD-COM`, `MOD-PUB`, `MOD-SEC`, `MOD-STAGE`, `MOD-INT-B`,
  `MOD-INT-C`, `MOD-INT-D`) and which go beyond conventional network copyleft
  (`MOD-BIN`, `MOD-PLUG`). Added Note 3 and the per-module statements.
- Updated SPDX guidance to recommend preset-specific identifiers and a
  machine-readable `MCL-Modules:` line (Clauses 9.1, 9.4, Annex D).
- Updated Annex A, Annex B, and Annex C (new item (n)) for Version 1.2.0.

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
