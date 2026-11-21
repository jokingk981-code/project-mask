# BUILD 046 — Material Realism

Real geometry and PBR changes:
- Seven matching tangent-space normal maps derived from the existing source material images.
- Seven grayscale roughness maps for micro-surface variation.
- Physically based material detail applied to exterior plaster, brick, timber, copper, slate, and both cobblestone road materials.
- Subtle wet puddles and gutter sheen on selected market areas using transparent physical materials.
- Teal atmospheric distance haze calibrated for the reference.
- No postprocessing dependency, screen-space reflections, new real-time lights, or GPU-heavy effects.

Important limitations: normal maps are derived from color luminance and are not scanned displacement geometry; wet patches are approximate, not ray-traced reflections. This does not turn procedural low-poly architecture into photorealistic models. Browser/GPU performance and visual result not tested on Chromebook.
