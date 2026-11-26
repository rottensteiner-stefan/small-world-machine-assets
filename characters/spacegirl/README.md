# SpaceGirl (`character.glb`)

Stylized female character mannequin, normalized to the canonical Small World Machine Mixamo rig.

## Specs

- **Geometry:** `14,830` vertices / `22,729` triangles (single continuous mesh, smooth welded vertex normals)
- **Skeleton:** `36` unified joints (`mixamorig:*` core hierarchy + `HandFingers`/`HandThumb` + `LeftHandMiddle1`/`RightHandMiddle1` palm grip sockets + `Ponytail1..3`, `<= 64`-bone GPU uniform budget, `0.0000°` canonical Mixamo rest-frame alignment)
- **Transform & Scale:** `1.600 m` height (`1.016 × 1.600 × 0.413 m`), flat soles grounded at `Y = 0`, horizontally centered, facing `+Z` (`RootNode` scale `1.0`)
- **Materials & Textures:** `1` PBR material (`alphaMode = OPAQUE`, `doubleSided = false`) with `2048×2048` WebP (`EXT_texture_webp`) BaseColor, ORM, and Tangent-Space Normal maps (`1.43 MB` GLB)
- **Polish Pass:** Pure-white eyeball sclera, softened/rounded lower chin contour, volume-preserving Taubin surface smoothing on shirt hemfolds, continuous welded normals, dynamic 3-bone ponytail chain & cross-leg weight cleanup, crisp `"25"` chest projection, and matte skin/garment `ORM` roughness calibration.
- **Provenance:** Generated from consistent Seedream v5 3-view references (`front`, `side`, `back`) via Tripo3D `v3.1-20260211` multiview-to-model + Mixamo `v3.0-20260909`, unified and polished in Blender 5.3. Raw generation inputs archived externally per engine ADR 0058.
- **License:** Project-owned original character asset (Stefan Rottensteiner).
