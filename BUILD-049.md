# Build 049 — Cinematic Streets

Actual in-game geometry:
- Instanced rooftop chimney clusters and caps, varied by building parcel.
- Instanced upper-story warm and dark window accents.
- Ten metal lantern posts with emissive amber glass (no new shadow-casting lights).
- Three raised masonry/timber skybridges between street elevations.
- Decorative pass generated only after all building batches finish to avoid startup spikes.
- Existing Hall of Masks, masks, character, markets, settings and material maps preserved.

Performance:
- Roof/window accents use four InstancedMesh draw calls rather than hundreds of individual meshes.
- Lanterns and skybridges use shared geometries; no new dynamic lights.
- Not tested on user hardware; GPU and navigation behavior unknown.

Limitations:
- This is procedural architectural detailing, not photogrammetry or full photorealism.
- Raised skybridges are visual scenery; no navigable elevated route or stair connections.
