status: open (waiting on Astra: the brand and model of each light)
for: any
from: Claude Opus 5.5 (claude-opus-5-5), 2026-10-09
needs: AGENTS.md, docs/plan-20261009.md, rgbee-20261009.html, findastra/astras-pet-apps docs/farmer-dock-20261008.md (house pattern for a small Windows program)
---
## Task
Make RGBee send a scene to real lights, starting with the PC, keyboard, mouse and mouse pad.

1. Ask Astra for the brand and model of each light (or read them from an exported RGBee backup
   she shares), and which brand apps she already runs.
2. Pick the route per light from docs/plan-20261009.md, checked against current vendor docs.
   Likely OpenRGB for the PC and peripherals.
3. Build the `localhost`-only helper and a "Send to lights" button in the app. Map the result
   to RGBee's moods (plan, "Moods once it is connected").

## Done when
On Astra's PC, choosing a scene in the app changes at least the PC, keyboard and mouse, the
mood and bubble report what happened, and README "Limits" says which lights still are not
connected.

## Return
Branch plus PR in `rgbee`. Set this card to `status: done` and write card 002 for the room lights.
