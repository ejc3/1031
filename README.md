# Connor's Room

The complete design suite for Connor's room — an Ink & Grain design.
Three static sites, one per deliverable. Zero build steps: every directory is a
self-contained site with its own landing page (`index.html`).

| Directory | Site | Suggested Vercel project / domain |
|---|---|---|
| `connor-room-board/` | The design board + the narrated 2:00 film | `connor-room-board.vercel.app` |
| `connor-room-3d/` | Interactive 3D walkthrough (three.js, single file) | `connor-room-3d.vercel.app` |
| `connor-room-palette/` | Witch Hat Atelier paint board | `connor-room-palette.vercel.app` |

## Deploy: one Vercel project per site

For each of the three directories:

1. vercel.com → **Add New → Project** → import `ejc3/1031`
2. **Root Directory** → pick `connor-room-board` (or `connor-room-3d` / `connor-room-palette`)
3. Framework preset **Other** — no build command, output = root
4. Deploy → each project gets its own `*.vercel.app` domain; add custom domains in the project's Domains tab

The three landing pages cross-link using the suggested `*.vercel.app` names above —
if you pick different project names, update the three links in the "rest of the suite"
section of each `index.html`.
