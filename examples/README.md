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

## Example index

| File | Main modules | Good fit |
|------|--------------|----------|
| [`ai-restricted.md`](./ai-restricted.md) | `MOD-AI`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want reciprocal publication plus an explicit AI-training restriction |
| [`cla-relicensing.md`](./cla-relicensing.md) | `MOD-CLA`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want contributor intake and planned relicensing authority |
| [`commercial-cooperative.md`](./commercial-cooperative.md) | `MOD-BIN`, `MOD-CLA`, `MOD-COM`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB`, `MOD-SUB` | Projects that want strong reciprocity plus non-competing commercial protection and steward alternative licensing authority |
| [`community-network.md`](./community-network.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Public software projects that want strong network reciprocity without the cloud-binary and private-fork extras |
| [`core-only.md`](./core-only.md) | none | Projects that want the permissive v1.1.1 no-module floor |
| [`file-copyleft.md`](./file-copyleft.md) | `MOD-FILE` | Projects that want weak file-level reciprocity rather than whole-work copyleft |
| [`internal-use-a.md`](./internal-use-a.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Internal-use-friendly reciprocity with no extra internal sharing rule |
| [`internal-use-b.md`](./internal-use-b.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-B`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want reciprocal access for integrated internal systems |
| [`internal-use-c.md`](./internal-use-c.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-C`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want public release of the exact internally used covered work |
| [`internal-use-d.md`](./internal-use-d.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-D`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG` | Projects that want public release of the internally used covered work and integrated internal systems |
| [`security-embargo.md`](./security-embargo.md) | `MOD-BIN`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB`, `MOD-SEC` | Projects that want trusted early security disclosure and later public publication |
| [`strong-cloud.md`](./strong-cloud.md) | `MOD-BIN`, `MOD-CLA`, `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-PUB` | Projects that want the strongest cloud and publication obligations without the commercial restriction |
| [`staged-preview.md`](./staged-preview.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, `MOD-PLUG`, `MOD-STAGE` | Projects that want preview channels or staged releases before full public publication |
| [`sublicensing.md`](./sublicensing.md) | `MOD-DIST`, `MOD-FILE`, `MOD-INT-A`, `MOD-PAT`, `MOD-SUB` | Single-rightsholder or fully authorized projects that want explicit steward alternative-licensing authority |

## Notes

- The examples are intentionally opinionated.
- They are designed to be easy to copy and adapt.
- The v1.1.1 `core-only` example is the permissive floor.
- The `file-copyleft` example restores the weak reciprocal baseline that older
  MCL drafts treated as always on.
- Most reciprocal examples now also activate `MOD-FILE`, and many also activate
  `MOD-PAT`, to reflect the posture a steward would often choose in practice.
- The `MOD-SEC` and `MOD-STAGE` examples are for temporary staged-publication
  workflows, not permanent private forks.
- Annex B presets remain informative only; Annex A is the operative block.
