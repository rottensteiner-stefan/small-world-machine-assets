# SpaceGirl (`character.glb`)

Stylized female character mannequin, normalized and rigged for Small World Machine.

## Specs

- **Geometry:** `14,696` vertices / `23,687` triangles (single continuous mesh, smooth vertex normals)
- **Skeleton:** `52` joints (`mixamorig:*`, pruned unused end-tip bones to fit within the `64`-bone GPU uniform budget)
- **Transform & Scale:** `1.000 m` height, feet at `Y = 0`, horizontally centered, facing `+Z` (`RootNode` scale `1.0`)
- **Materials & Textures:** `1` PBR material (`alphaMode = OPAQUE`, `doubleSided = false`) with `2048x2048` WebP (`EXT_texture_webp`) BaseColor, ORM, and Tangent-Space Normal maps (`1.60 MB` GLB)
- **Polish Pass:** Volume-preserving Taubin surface smoothing on chest/jawline, continuous welded normals, ponytail `Head`-lock & cross-leg weight cleanup, nostril & face/hair-tip UV-gutter spot cleanup (`3,723` pixels with intact sclera/collar), and matte skin/shirt `ORM` roughness calibration (`>= 0.64`/`0.82`, glossy eye catchlights preserved).
- **Provenance:** Generated from clean 3D stylized front reference via Tripo3D `v3.1-20260211` (`geometry_quality=detailed`, `texture_quality=detailed`, `pbr=true`), auto-rigged with Tripo `v3.0-20260909` (`--spec mixamo`), and aligned to Adobe Mixamo local bone coordinate frames + normalized in Node/Blender. Sources archived externally per engine ADR 0058.
- **License:** Project-owned original character asset (Stefan Rottensteiner).
