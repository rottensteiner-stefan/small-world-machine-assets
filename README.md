# Small World Machine Assets

Canonical out-of-tree repository for reusable 3D assets, modular kits, character mannequins, and animation pools across the [Small World Machine](https://github.com/rottensteiner-stefan/small-world-machine) ecosystem.

Implemented in accordance with **ADR 0011: Modulare Asset-Kits & Out-of-Tree-Asset-Bibliothek**.

## Repository Structure

```text
small-world-machine-assets/
├── characters/          # planned: runtime-ready rigged characters (character.glb + metadata)
├── animations/          # planned: shared locomotion and mocap pools (GLB)
└── kits/                # planned: modular environment kits (GLB/WebP + meta.json)
```

## Runtime assets only

Per engine **ADR 0058 (Originals stay out of git)** this repository holds only runtime-ready assets
and their provenance notes. Originals and intermediates (`raw/`, Tripo `tripo-out/`, `.blend`, `.fbx`,
Mixamo packages, concept/turnaround inputs, unmodified third-party downloads) are kept outside git in
the maintainer's Google Drive (`Small-World-Machine/small-world-machine-assets/…`, with a sha256
`MANIFEST.txt`). The former `characters/dino/` and `characters/spacegirl/` sources moved there on
2026-11-07.

## Git LFS Requirement

This repository uses [Git Large File Storage (LFS)](https://git-lfs.github.com/) to track binary files (`.glb`, `.png`, `.webp`, etc.).

Ensure Git LFS is installed and initialised before cloning:

```bash
git lfs install
git clone https://github.com/rottensteiner-stefan/small-world-machine-assets.git
```

## Licenses

- Every asset documents source, author, license and derivation in its subdirectory (`license.txt` / `README.md`) or in the consuming repo's `REFERENCES.md`.
