# Rules for assistants working on RGBee (rgbee)

*A pet app by Astra.* Public credit is always **Astra**, never a legal name. Keep work
information (including any employer's name) out of this repo.

Hatched with Claude Opus 5.5 (`claude-opus-5-5`), 2026-10-09. Record your model name and
version here when you change something substantial.

Draft sprite sheet and nine transparent mood frames added with OpenAI Codex (GPT-6), 2026-10-11. Assets remain separate in `draft-art/rgbee/` pending Astra's review; runtime is unchanged.

## What this is
A pet app for RGB lighting: room lights, mouse pad, mouse, PC and keyboard. v0 is a one-file
web app (`rgbee-20261009.html`) that lists lights, mixes scenes and previews them. It controls
no real light yet; [docs/plan-20261009.md](docs/plan-20261009.md) says how it will. Its host is
the Friendly Farmer in `findastra/astras-pet-apps`; the pet's registry entry and art live there.

## Rules
- Follow the Cage's [PET-FILES.md](https://github.com/findastra/astras-pet-apps/blob/main/PET-FILES.md)
  and use its [PET-WORDS.md](https://github.com/findastra/astras-pet-apps/blob/main/PET-WORDS.md):
  pet, app, desktop pet, bubble, quick chat, app icon, pet well.
- **Never commit** API keys, bridge usernames, `.env` files, backups or device serial numbers.
  They stay on the PC.
- User and device text goes into the page with `textContent`, never `innerHTML`.
- **Light safety:** no effect flashes more than three times a second, and every animation stops
  under `prefers-reduced-motion`.
- A helper (v1) listens on `localhost` only. Do not open it to the network.
- Say plainly what is not done. Update README "Limits" with every change.
- No pushing to `main` and no new GitHub repos without Astra's OK; use a branch and a PR.

## Handoffs
When Astra's request is unclear or sounds like an assignment, check `handoffs/` here and in
`findastra/astras-pet-apps` first. Leave a card when work remains. Format: the Cage's
[skills/handoff/SKILL.md](https://github.com/findastra/astras-pet-apps/blob/main/skills/handoff/SKILL.md).
