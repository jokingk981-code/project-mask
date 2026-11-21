# Build 051 — Wet Cobblestone Material Pass

- Added a new physically textured rain-darkened cobblestone diffuse material, derived from a dedicated generated texture asset and bundled locally. No static scene backdrop.
- Tiled on the main road material; older alternate cobble remains for secondary lanes.
- Added 90 subtle, instanced amber reflection-like glints near four plazas in one draw call.
- Preserved masks, Hall landmark, player, markets, graphics controls and earlier buildings.

Limits: texture is an artist-generated surface, not a physically scanned PBR material; glints are not real reflections. Generated texture was edge-blended but seamless tiling was not visually verified. Runtime not tested on Chromebook.
