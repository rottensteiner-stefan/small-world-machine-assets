# Small World Machine Assets

Canonical out-of-tree repository for reusable 3D assets, modular kits, character mannequins, and animation pools across the [Small World Machine](https://github.com/rottensteiner-stefan/small-world-machine) ecosystem.

Implemented in accordance with **ADR 0011: Modulare Asset-Kits & Out-of-Tree-Asset-Bibliothek**.

## Repository Structure

```text
small-world-machine-assets/
├── characters/
│   ├── dino/            # Tripo3D + Mixamo player character for the 2.5D platformer showcase (concept, base mesh, Mixamo package)
│   └── spacegirl/       # Tripo3D mannequin (GLB, Blender scene, PBR textures, concept sheet)
├── animations/          # planned: shared locomotion and mocap pools (not yet migrated)
└── kits/                # planned: modular environment kits (not yet migrated)
```

## Git LFS Requirement

This repository uses [Git Large File Storage (LFS)](https://git-lfs.github.com/) to track binary files (`.glb`, `.blend`, `.fbx`, `.png`, etc.).

Ensure Git LFS is installed and initialised before cloning:

```bash
git lfs install
git clone https://github.com/rottensteiner-stefan/small-world-machine-assets.git
```

## Licenses

- Individual asset licenses are documented in their respective subdirectories (e.g. `characters/<name>/license.txt`, where third-party).
