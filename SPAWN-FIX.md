BUILD 044 — THE ACTUAL FIRST-IMPRESSION FIX

Root cause: previous builds kept player.position.set(0,0,8), which spawned the player inside the original straight Hall approach. The crooked district only began at z≈39, and loaded after entering. So despite extensive exterior work, the player's first view remained a corridor.

Changes:
- Player starts at x=11, z=113, directly in the crooked Lantern Market district, near the market junction and clustered shopfronts.
- Organic town begins building immediately upon ENTER rather than after an additional 120ms delay.
- Hall and mask mechanics remain in the world; the initial starting location is now the outdoor district.
- Intro line updated for new location.

Limitation: original Hall approach geometry remains at z<40 and can still be visited. This fixes the opening view, not a full replacement of that legacy area. The game has not been visually or gameplay tested on the user's hardware.
