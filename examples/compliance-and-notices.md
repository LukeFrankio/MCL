# Compliance records and notices example

Unlike the other examples, this file is not an Annex A activation block. It shows
the paperwork that active modules create: the Annex D source notice, the Annex C
Compliance Record for a modified network deployment, the lighter record for an
unmodified upstream deployment under Clause 6.2(h), and a machine-readable form.

All names, URLs, dates, and commit identifiers are fictional. The project is the
Harbor Forge example from [`community-network.md`](./community-network.md).

## Good fit

- Operators who run MCL software over a network and need to publish a Compliance
  Record under `MOD-NET`
- Projects that want a copyable source notice with a machine-readable module list

## Bad fit

- Projects that activate neither `MOD-NET` nor `MOD-BIN`, which have no
  Compliance Record duty
- Anyone expecting these records to be valid without replacing every fictional
  value with the real one

## Source notice (Annex D)

```text
Copyright 2026 Harbor Forge Foundation

Licensed under the Modular Cooperative License (MCL), Version 1.2.0.
Activated Modules for this version: MOD-DIST, MOD-FILE, MOD-INT-A, MOD-NET,
MOD-PAT, MOD-PLUG
License text: https://git.example/harbor-forge/forge/blob/v2.4.0/MCL-LICENSE
SPDX-License-Identifier: LicenseRef-MCL-1.2.0
MCL-Modules: MOD-DIST, MOD-FILE, MOD-INT-A, MOD-NET, MOD-PAT, MOD-PLUG
```

A project whose active modules exactly match a preset in Annex B can use the
preset-specific identifier instead. For example, `MCL-COMMUNITY` is
`MOD-DIST`, `MOD-INT-A`, `MOD-NET`, `MOD-PAT`, and `MOD-PLUG`:

```text
SPDX-License-Identifier: LicenseRef-MCL-1.2.0-COMMUNITY
MCL-Modules: MOD-DIST, MOD-INT-A, MOD-NET, MOD-PAT, MOD-PLUG
```

Harbor Forge also activates `MOD-FILE`, so it is not exactly `MCL-COMMUNITY` and
uses the plain identifier above.

## Compliance Record 1: modified network deployment

Meridian Hosting Co. runs a modified Harbor Forge for third parties. It adds an
entitlement gateway that is Specific to Harbor Forge and gates its features, so
the gateway is an Integral Component (criterion F1 of Clause 2.14) and must be
published under Clause 6.2(b). Its database and identity provider are unmodified
general-purpose tools, which Clause 2.14 excludes.

```text
MCL COMPLIANCE RECORD (Annex C)

(a) Software name:
    Harbor Forge (Meridian build)
(b) License version:
    Modular Cooperative License v1.2.0
(c) Activated Modules:
    MOD-DIST, MOD-FILE, MOD-INT-A, MOD-NET, MOD-PAT, MOD-PLUG
(d) Corresponding Source repository:
    https://git.example/meridian/harbor-forge
(e) Exact version identifier:
    tag meridian-2.4.0-r3, commit 9c1f4e7a2b8d3e5f60718293a4b5c6d7e8f90a1b
(f) Network service endpoint:
    https://forge.meridian-hosting.example (stable service URL; instances are
    autoscaled, so transient instance URLs are not listed)
(g) Cloud binary artifacts:
    Not applicable because MOD-BIN is inactive.
(h) Operational Materials:
    Not required for this profile.
(i) Extension API and Integral Components:
    Documented Extension API: https://docs.harborforge.example/extensions
    Integral Components list:
    https://git.example/meridian/harbor-forge/blob/meridian-2.4.0-r3/INTEGRAL_COMPONENTS.md
    (lists the entitlement gateway in gateway/)
(j) Primary Commercial Function:
    Not applicable because MOD-COM is inactive.
(k) Compliance contact:
    compliance@meridian-hosting.example
(l) Public operation of this version began:
    2026-09-14
(m) Public operation ceased:
    Not applicable; operation is continuing.
(n) Clause 6.2(h) statement:
    Not applicable; this deployment is modified and adds an Integral Component.
```

## Compliance Record 2: unmodified upstream deployment

Pine Valley Library Cooperative runs Harbor Forge v2.4.0 exactly as released. It
adds no Integral Components, no Operational Materials, and no Material
Modifications, so Clause 6.2(h) applies. The record points to the upstream
release, and the links that users see under Clause 6.2(c) through 6.2(e) may
point to the upstream repository.

```text
MCL COMPLIANCE RECORD (Annex C)

(a) Software name:
    Harbor Forge
(b) License version:
    Modular Cooperative License v1.2.0
(c) Activated Modules:
    MOD-DIST, MOD-FILE, MOD-INT-A, MOD-NET, MOD-PAT, MOD-PLUG
(d) Corresponding Source repository:
    https://git.example/harbor-forge/forge
(e) Exact version identifier:
    tag v2.4.0, commit 4d2b8f10c7e35a96b1f0d8e2c4a6b7391e5f0c28
(f) Network service endpoint:
    https://forge.pinevalley-library.example
(g) Cloud binary artifacts:
    Not applicable because MOD-BIN is inactive.
(h) Operational Materials:
    Not required for this profile.
(i) Extension API and Integral Components:
    Documented Extension API: https://docs.harborforge.example/extensions
    Integral Components list: none; this deployment adds none.
(j) Primary Commercial Function:
    Not applicable because MOD-COM is inactive.
(k) Compliance contact:
    it@pinevalley-library.example
(l) Public operation of this version began:
    2026-10-02
(m) Public operation ceased:
    Not applicable; operation is continuing.
(n) Clause 6.2(h) statement:
    This deployment is an unmodified upstream operation under Clause 6.2(h).
    Upstream release: v2.4.0 (commit 4d2b8f10c7e35a96b1f0d8e2c4a6b7391e5f0c28)
    in https://git.example/harbor-forge/forge. The operator has added no
    Integral Components, Operational Materials, or Material Modifications.
```

## Machine-readable form

Annex C says the record SHOULD also be provided in a machine-readable format
where practical. One way to do that for Record 2:

```json
{
  "softwareName": "Harbor Forge",
  "licenseVersion": "MCL-1.2.0",
  "activatedModules": ["MOD-DIST", "MOD-FILE", "MOD-INT-A", "MOD-NET", "MOD-PAT", "MOD-PLUG"],
  "sourceRepository": "https://git.example/harbor-forge/forge",
  "version": { "tag": "v2.4.0", "commit": "4d2b8f10c7e35a96b1f0d8e2c4a6b7391e5f0c28" },
  "serviceEndpoint": "https://forge.pinevalley-library.example",
  "documentedExtensionApi": "https://docs.harborforge.example/extensions",
  "integralComponents": [],
  "complianceContact": "it@pinevalley-library.example",
  "publicOperationBegan": "2026-10-02",
  "publicOperationCeased": null,
  "unmodifiedUpstreamOperation": {
    "clause": "6.2(h)",
    "upstreamRelease": "v2.4.0",
    "upstreamRepository": "https://git.example/harbor-forge/forge"
  }
}
```

## Notes

- The record must identify the exact version in operation, so update it when the
  deployed version changes (Clause 6.2(g)).
- Retention: keep a record for as long as the operation continues, and for 12
  months after it ceases. For an operation covered by Clause 6.2(h), 30 days
  after it ceases is enough (Clause 7.7).
- If `MOD-BIN` is active, items (g) and (h) become required and list artifact
  URLs, integrity digests, the build-recipe location, and the Operational
  Materials. See [`strong-cloud.md`](./strong-cloud.md).
- If `MOD-COM` is active, item (j) repeats the Primary Commercial Function from
  Annex A.
