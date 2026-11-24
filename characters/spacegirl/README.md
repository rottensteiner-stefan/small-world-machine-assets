# SpaceGirl (`character.glb`)

Stylized female character mannequin, rebuilt from Seedream v5 3-views and normalized/rigged for Small World Machine.

## Specs

- **Geometry:** `14,830` vertices / `22,729` triangles (single continuous mesh, smooth welded vertex normals)
- **Skeleton:** `52` joints (`mixamorig:*`, pruned unused end-tip bones to fit within the `64`-bone GPU uniform budget)
- **Transform & Scale:** `1.000 m` height, feet at `Y = 0`, horizontally centered, facing `+Z` (`RootNode` scale `1.0`)
- **Materials & Textures:** `1` PBR material (`alphaMode = OPAQUE`, `doubleSided = false`) with `2048x2048` WebP (`EXT_texture_webp`) BaseColor, ORM, and Tangent-Space Normal maps (`1.55 MB` GLB)
- **Polish Pass:** Volume-preserving Taubin surface smoothing on chest/shirt hemfolds, continuous welded normals, ponytail `Head`-lock & cross-leg weight cleanup, strict eye-socket protection, achromatic forehead/bang edge-halo cleanup (`chroma2 < 0.18 & ~warm_skin_px`), crisp `"25"` chest projection (`|x| <= 0.088`, sleeves excluded), and matte skin/garment `ORM` roughness calibration.
- **Provenance:** Generated from consistent Seedream v5 3-view references (`front`, `side`, `back`; refined upper-torso proportions and slightly longer shorts) via Tripo3D `v3.1-20260211` multiview-to-model (`geometry_quality=detailed`, `texture_quality=detailed`, `pbr=true`), auto-rigged with Tripo `v3.0-20260909` (`--spec mixamo`), and aligned to Adobe Mixamo local bone coordinate frames + polished in Blender 5.3. Sources archived externally per engine ADR 0058.
- **License:** Project-owned original character asset (Stefan Rottensteiner).
