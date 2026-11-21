# PROJECT MASK — High-Fidelity Production Pipeline

Status: PLANNED. This document establishes standards; it does not certify that any asset or render has been created or tested.
Branch: development/aaa-visual-pipeline
Protected release branch: main (do not alter until verified and approved).

## Visual source of truth
Eight reference images supplied by the creative director in chat, including:
- Hall Lantern Mk I: ornate blackened metal, aged brass edge wear, quatrefoil/pointed-arch detailing, imperfect wavy glass, melted candle wax, warm flame; approximately 80 cm hanging assembly.
- Fragment 01, The Forgotten One: cream horned mask/face, black eye openings, visible fine cracks, dark layered fabric, six-view orthographic turnaround; reference labels 105 mm height.
- Mask City: irregular, highly vertical Gothic urbanism, dense layered streets and bridges, suspended structures, warm lanterns against teal mist, wet uneven cobbles, mask stalls, masked citizens.
- Hall of Masks: monumental mask-covered walls, central figure and focal mask, lantern-lit reflective floor, dense hanging artifacts.

These are appearance targets, NOT existing 3D assets or proof of achievable real-time performance.

## Non-negotiable production criteria
1. Actual inspectable 3D geometry and physically based materials, not background imagery passed off as playable architecture.
2. High-detail source meshes and source textures preserved independently from runtime-optimized derivatives.
3. Assets include scale, pivot, UVs, material slots, and export manifests; characters additionally require skeleton/rig and animation checks.
4. Preview renders include neutral-light turntable and cinematic context; compare against supplied references.
5. No claims of photorealism, visual parity, playable quality, or hardware compatibility without visual inspection and test evidence.
6. Maintain working main branch; all changes are developed on this branch and reviewed before merging.
7. Android and Chromebook remain intended platforms, but the master-asset production/rendering workflow may require external GPU/compute. Runtime performance is not guaranteed.

## Initial production milestone: Hall Lantern Mk I
Target source format: Blender project / procedural Blender Python script; interchange: glTF/GLB.
Geometry: hanging ring and chain, ornamental dome/crown, forged corner posts, Gothic pointed-arch panels, quatrefoil bands, metal trim and rivets, glass panes, candle and wax.
Materials: aged blackened iron with edge wear, darkened brass, imperfect glass, warm wax, flame emissive component.
Lighting: separate cinematic studio and Hall of Masks scene presets.
Verification artifacts required: source model, exported GLB, four orthographic views, close-up detail views, neutral render, in-scene render, geometry/UV/material validation report.
Optimization: separate game-ready mesh and baked textures, with LODs and instancing suitability assessed.

## Sequence
A. Audit actual repository file tree and source; establish deployed build/version.
B. Implement reproducible 3D asset generator and validation scripts.
C. Generate and render Hall Lantern Mk I, inspect against reference and iterate.
D. Build Hall of Masks architectural kit and one fully realized playable vertical slice.
E. Create character source meshes, materials, rigging and animation pipeline.
F. Integrate into selected engine after technical comparison and hardware profiling.

## Acceptance gate
An asset is NOT complete until geometry and source files exist, renders have been inspected, and required validation is recorded. A syntax check alone is not render validation.
