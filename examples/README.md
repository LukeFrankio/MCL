# Examples

This folder contains illustrative, fictional examples of completed Annex A
activation blocks for the Modular Cooperative License.

Use these files as starting points, not as drop-in production metadata. Replace
all software names, contact details, repository URLs, governing-law fields, and
project-specific clarifications before using any example in a real project.

## How to use these examples

1. Pick the example closest to your policy posture.
2. Copy the Annex A block into your project.
3. Replace the fictional metadata.
4. Review the active modules carefully.
5. Fill any module-specific configuration fields that matter for your project.
6. Complete the Venue, Runtime Components, and Additional Permissions fields
   if they apply (the examples show them as unset or `none`).

## Example index

| File | Main modules | Good fit |
|------|--------------|----------|
| [`ai-restricted.md`](./ai-restricted.md) | `MOD-AI`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want reciprocal publication plus an explicit AI-training restriction |
| [`cla-relicensing.md`](./cla-relicensing.md) | `MOD-CLA`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want contributor intake and planned relicensing authority |
| [`commercial-cooperative.md`](./commercial-cooperative.md) | `MOD-BIN`, `MOD-CLA`, `MOD-COM`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB`, `MOD-SUB` | Projects that want strong reciprocity plus non-competing commercial protection and steward alternative licensing authority |
| [`community-network.md`](./community-network.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Public software projects that want strong network reciprocity without the cloud-binary and private-fork extras |
| [`compiler-toolchain.md`](./compiler-toolchain.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-PAT`, `MOD-PLUG` | Compilers, interpreters, and code generators that embed runtime code in their output and want `Runtime Components` |
| [`compliance-and-notices.md`](./compliance-and-notices.md) | none (not an Annex A block) | Operators and projects that need Annex D source notices and Annex C Compliance Records, including the unmodified-upstream path |
| [`core-only.md`](./core-only.md) | none | Projects that want the permissive v1.2.0 no-module floor |
| [`file-copyleft.md`](./file-copyleft.md) | `MOD-FILE` | Projects that want weak file-level reciprocity rather than whole-work copyleft |
| [`gnu-alternative.md`](./gnu-alternative.md) | `MOD-CLA`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Stewards who want an explicit GPL or AGPL option for their own material under v1.2.0 |
| [`internal-use-a.md`](./internal-use-a.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Internal-use-friendly reciprocity with no extra internal sharing rule |
| [`internal-use-b.md`](./internal-use-b.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-B`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want reciprocal access for integrated internal systems |
| [`internal-use-c.md`](./internal-use-c.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-C`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want public release of the exact internally used covered work |
| [`internal-use-d.md`](./internal-use-d.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-D`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want public release of the internally used covered work and integrated internal systems |
| [`personal-use-carveout.md`](./personal-use-carveout.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-C`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB` | Strong organizational transparency with personal-use carve-outs for individuals |
| [`security-embargo.md`](./security-embargo.md) | `MOD-BIN`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB`, `MOD-SEC` | Projects that want trusted early security disclosure and later public publication |
| [`source-available-noncompete.md`](./source-available-noncompete.md) | `MOD-COM` | A lean source-available non-compete on the permissive floor, with `Permitted Uses` and a delayed Apache-2.0 option |
| [`strong-cloud.md`](./strong-cloud.md) | `MOD-BIN`, `MOD-CLA`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB` | Projects that want the strongest cloud and publication obligations without the commercial restriction |
| [`staged-preview.md`](./staged-preview.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-STAGE` | Projects that want preview channels or staged releases before full public publication |
| [`sublicensing.md`](./sublicensing.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-PAT`, `MOD-SUB` | Single-rightsholder or fully authorized projects that want explicit steward alternative-licensing authority |

## Notes

- The examples are intentionally opinionated.
- They are designed to be easy to copy and adapt.
- The v1.2.0 `core-only` example is the permissive floor.
- The `file-copyleft` example restores the weak reciprocal baseline that older
  MCL drafts treated as always on.
- Most reciprocal examples now also activate `MOD-FILE`, and many also activate
  `MOD-PAT`, to reflect the posture a steward would often choose in practice.
- The `MOD-SEC` and `MOD-STAGE` examples are for temporary staged-publication
  workflows, not permanent private forks.
- Annex B presets remain informative only; Annex A is the operative block.
- The examples use the v1.2.0 Annex A template. It adds `Venue`, `Permitted
  Uses` (for `MOD-COM`), `Runtime Components`, and `Additional Permissions and
  Alternative Licenses`, and notes that blank `MOD-SEC` and `MOD-STAGE` fields
  take the defaults in Clause 5.8.
- No example offers GPL or AGPL compatibility. v1.2.0 has no automatic bridge
  (Clause 9.3). A rights holder can grant such a permission explicitly in the
  `Additional Permissions and Alternative Licenses` section of Annex A.
- Open-source status (Clause 9.6): `ai-restricted`, `commercial-cooperative`,
  `internal-use-b`, `internal-use-c`, `internal-use-d`, `personal-use-carveout`,
  `security-embargo`, `source-available-noncompete`, `staged-preview`, and
  `strong-cloud` activate modules that are not open source in the OSI sense.
  `community-network`, `cla-relicensing`, `compiler-toolchain`,
  `gnu-alternative`, and `internal-use-a` activate `MOD-PLUG`, which may not be
  treated as open source. `core-only`, `file-copyleft`, and `sublicensing`
  activate none of the modules named in Clause 9.6. None has been reviewed by
  the OSI.
- If no `MOD-INT` variant is marked, `MOD-INT-A` is deemed active (Clause 5.5).
- Five examples showcase v1.2.0 features. `gnu-alternative` shows an explicit AGPL
  option, `compiler-toolchain` shows Output and Runtime Components,
  `source-available-noncompete` shows `Permitted Uses` and a delayed alternative
  license, `personal-use-carveout` shows the personal-use carve-outs, and
  `compliance-and-notices` shows Annex C and Annex D paperwork.
